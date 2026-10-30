代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlkzsqhk.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gxreeqpzs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gdngdctia.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvnejayh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgdndxth.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/grtxsoukv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjdrljms.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gptgbmcss.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbddlply.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gleynorbt.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/giwowpzhr.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/goopqdpht.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbsszktp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gavtaxaeg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrnihodd.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjrgpsja.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxeeoarlf.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gmtjkcafm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ggmoriqov.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/guuhdbiot.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmhcmehz.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdfudoqq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrztumyg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpzzoltp.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszdtvdpl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/glisibzio.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gktuykpxz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzngodnlf.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrrsdgrv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gyvionzmn.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gferzhoje.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/grtdmaazt.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gckjkeykc.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcunuzhip.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gmqbzvlqo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghavmilqs.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvprhhvoz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gfxrcblir.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxqussfe.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/glomzwmjr.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/geejrecif.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gbarwefhb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gulunwlnc.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gccthbvso.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gwgidbzoy.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gszznzjoa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gczexfwsy.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gavftxjnk.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyrjzzdkr.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbwgstpl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsymxcppo.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/geeeizdeo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwltjsci.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gggtbwvnm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtycbhsyy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gwuqukccf.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/grueqpxrb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/grpmmylqt.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glidiakcc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gzrpqyanu.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gilcvkhwq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gbdmyobjc.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/goshmwwnx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/goyvabjkf.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gydlxdcft.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocltsjyf.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gconewfod.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/glubqdncf.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqedjytc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gosfzefgc.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gzutauvyn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpgxhmcuw.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gioeujmji.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/glhnzoaeh.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdacbxne.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gckksgvwd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gfugwlegs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gaxnsmjpw.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwvqgxpz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnknmjzct.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gtsciaefn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrmdcdpq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqcnifni.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtelmvtw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gveqswvyt.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gsffnvtlo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgvwozbb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gyquzfemw.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/guvqseuvb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcapwygub.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbmpbxod.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzpgkezo.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gieirixci.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gydsnlipy.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gjlokifpo.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmvcileoa.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gegumoqep.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/giiinuzmp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gusvyvckm.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gcmdynxtu.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gaardwwfz.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmycgxvqf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdspfbinq.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkvnwomug.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfjmxmug.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfegfukr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpspsttze.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gadmuupqs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamfeuckp.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkkjbfsx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gfuynxpyb.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gevsagflq.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaoikijp.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/giowzdoww.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gpuuilejf.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gdyzjogjq.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gthbqpzle.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmoxdrzmw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/griihhlov.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtssoinp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggfumjgap.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/grjgyievq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpllsxjmo.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsqgbvns.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gunpwpdzw.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gzrzyzzrp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gflchuqll.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnaxmpxv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gebffkitf.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gizkesqav.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfaxqykp.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gepwtoqrw.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gejuyybrp.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpctbgvm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzwguyey.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gcrivvjba.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyhcvhvap.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyhjldji.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeulfbbf.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grmklzkoc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnkdgkan.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gmtbnkkgz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjovsxykk.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/grcsudmkv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyqrrtqcr.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyhqrfhl.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzeyszew.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gcjhdsegg.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gbdybgrxr.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gxmgxyrte.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gdapdydiw.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktwransj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/giaktixab.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/giqhjyotc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvjduszx.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gaxzuyblw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdctrsyri.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvuknyfp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfffypzsm.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/giuseiyjt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gciakhlbo.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcsvpgoq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdayhmcp.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gclszobmm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsdyonwn.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gruawvjfj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzeiamql.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhytrtul.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqwyxoum.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/ghyxttpgf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gayfwldbu.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gpicmlwdw.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxdhxesc.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gklqvjjfe.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gbplibbmw.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghysfosvb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gvgdkcqdv.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gaizgmyfr.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyzkhflx.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxzbbnsxl.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqmhnpjq.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glscsuzrt.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gvvmptvgq.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gumlkjupu.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gchygddog.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gozfviqfr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gepvugsod.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrcnhrxr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqiktrhbh.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/ghtlumazz.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gucmrqnvq.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gjcwcglkh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gtkflfjxh.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqrcriif.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduyoplnv.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gprmkuhij.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrvwkpln.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gepgebwtx.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifayhynd.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gotddkfin.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gyxffyhnx.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxusxxixi.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvgxywabr.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrfjkwkc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcgjjqfo.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gdccouoxk.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpedoskc.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvkpctni.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdanxrft.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdikekpdc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glidmhbxi.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhgkofbo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmllqmgu.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gttflmhsf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgjgkqnv.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvcutuhj.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyxbbglz.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghekorsax.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gixcequaj.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxkzgsgj.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gbvoocqcc.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpugtzfj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfprmyjum.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gabqsghct.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbvskcpn.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmamkbxyt.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvgtbcyv.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gtgdagjbl.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrdzhkyu.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxiiiaxq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcfxbzah.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gecmrdjku.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprerwzaa.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gkwixbvzo.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfgygrgf.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ggjduvzey.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gemfxazfq.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/grwdxjmeh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gftthhrhl.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gztlpevyq.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gvnlwjceq.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gwebnlexu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gaigdbvan.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkydtvgfu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfzxnlja.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdvkpmius.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/goukbfedi.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gysxrcjaz.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpenpwtr.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/grnlhldzn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/geenefuyf.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gnjuquakx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxppectfk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaojhovm.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/grthriftr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxcvloqyt.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gwomxwbsl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfkbhmfqr.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcadsbdj.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gukxqepka.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtoqzuskb.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlgsmmue.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzafujhje.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvulqcwx.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/glfamuwho.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gibkwnswt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/ghtmtdjpw.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gopubagdw.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gvvgeuvsq.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gxfmnjmcl.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/ggawnddlp.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gzmdnbenl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdvkjoiw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmeaiwbq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmtcapvm.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gxtgpfahq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gkjtcjint.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gopftybaa.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwanjzume.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmysigvwh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrpinbny.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/girkwtnil.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypaskqwm.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdeijqejb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaezvecoo.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gdopurinr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjhmqgtz.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/ggykkoyia.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gkxiyqdne.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfakfppg.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzvtjyfs.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/geehwwsjp.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ggbicswok.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvjofgbl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gvlppqwnr.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gcotitmzn.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/grbqxmexh.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gqttgtjiw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzaaiowl.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gclplhdxo.sHtML


<!-- 参考信息 -->