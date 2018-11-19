
# HIREDIS-V

hiredis-v is a C client library for the [Redis](http://redis.io/) database.
hiredis-v fully contained and inherit from hiredis-vip:(https://github.com/vipshop/hiredis-vip)

## CLUSTER AUTH SUPPORT
### ADD AUTHENTICATE API:

int redisClusterSetOptionPassword(redisClusterContext *cc, const char *password);

### HOW TO USE:
redisClusterContext *cc = redisClusterContextInit();

redisClusterSetOptionPassword(cc, "your password");

redisClusterSetOptionAddNodes(cc, "127.0.0.1:6379,127.0.0.1:6380,127.0.0.1:6381");

redisClusterConnect2(cc);

## MORE INFORMATION:
more information, see https://github.com/vipshop/hiredis-vip/wiki

## AUTHORS
Hiredis-v was maintained and used at wuli1999(https://github.com/wuli1999.)
