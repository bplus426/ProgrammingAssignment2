## t1


makeCacheMatrix <- function(x = matrix()) {
    t1 <- NULL
    set <- function(y) {
        x <<- y
        t1 <<- NULL
    }
    get <- function() x
    sett1erse <- function(solve) t1 <<-solve 
    gett1erse <- function() t1
    list(set = set, 
         get = get,
         sett1erse = sett1erse,
         gett1erse = gett1erse)
}  




cacheSolve <- function(x, ...) {
    t1 <- x$gett1erse()
    if(!is.null(t1)) {
        message("getting cached data")
        return(t1)
    }
    data <- x$get()
    t1 <- solve(data, ...)
    x$sett1erse(t1)
    t1
}
