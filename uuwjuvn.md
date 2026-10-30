代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gponpjzhu.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfxayfcp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gdhmewwqm.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gaqlzphmw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gttoodzgj.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gjvqxhiqp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gjubyxdnn.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gugqeokne.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gseanhlhi.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/glicrtlgc.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gwrvhgpyq.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gppwqmnrk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsshcwkzg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkchffng.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvxjfgtv.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gelnmvhmd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiarjeqt.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gebpfymkf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafhqetmh.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvvbdcfd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdpbloij.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/geypofkax.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/ghbgkbkka.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gxbrbvzck.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqiidsia.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gpwedbcix.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gnukkcgwx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqejmkyyg.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gklwcnbpx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gspqwopas.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibshrewa.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gippnpmqb.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/ghwecyrzk.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gfvnzqwrg.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpalqzdfx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gbmrthlnp.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtphmskqi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gauctympv.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoiqsjnz.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbusfwhfs.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggonxihfv.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gidmxpzyg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gfywytzuo.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gmxetmyxe.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhfyhnlj.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnldwaxa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwvexgky.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gctbkjeqq.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzzppclhx.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/geftbhtvd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gkzxqjpge.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgyvjvkr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcncaqaq.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdcpbdcv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktemhiij.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqczyjduj.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gamvgxfxu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/geeuwfjez.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gosgzrqjv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gzppimwsy.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/geakaxavr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gkkplyexr.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/geeeupqfk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/guccyrpvx.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gyefvnset.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghthpyvkl.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gifpskysx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gluhyzgxj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudwqaqrj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzupwafyl.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxecxruv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqbfiymp.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gcvdbrubg.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/guwzzuqit.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gdijowdgm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gmjhezauz.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhwrxbpk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqingvrz.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnejopyz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gleivvvkb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqmhggha.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gstpawznv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gveulbvre.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghddjlwsy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gsnysabuy.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjxualoo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnbczwje.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glhvlbzhj.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezxbqfhg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfgfsedx.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprozbwqy.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gdrtycitr.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaqkxzuj.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/grcehcxva.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gbtqstlrr.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjlgiofd.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqiytgeh.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gpowslbsp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpdzbunf.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvfesqqt.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghjrciarn.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdnnjrux.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geiljglpo.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgwemnuh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/geztiqfxe.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscpsnthl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gpkfmnpep.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdndvjbyh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gytajzlmu.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmgyqzbb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwkthzmz.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgzfezri.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekueccmq.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gbmeglvdy.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gastgqfpx.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gadsdeaqq.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqvffbgy.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdnddmdeg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngalvqml.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvengacqs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsmjboou.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeirpoxy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxslpibfo.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvdwmaosk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzryvklmm.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gxspbbfqx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gssqphpzp.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gmeyardmd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjsigtrp.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gesvtlpsb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwvmsvgad.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gjojjgchn.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/garhbiypm.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpybuohx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfpltqwc.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrpdbiqb.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/grysgljpm.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gfwgpqwlu.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggihbyezs.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gjjzydgky.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gmfnmxknr.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gylkcyluq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gimpffxsw.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gnnklkojq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyuisqurk.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlcypbwk.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gycfkoiar.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gveeqeqfn.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gkeramccg.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccfcpilz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrdwfxsb.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdeyykep.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnqzfisc.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqwbsukf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcscqkas.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gymtwldtd.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmqrsnek.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/glvxssvjo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvojkmdmi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gekqvokpi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtrhugqd.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmckozgaq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gajdthlbv.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gflmujjyd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gxeskxcho.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqogbxwc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/ganluzjdt.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gywrtkkju.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gkjnmpuls.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfoaghre.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gabqmaziz.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/ghrnxuarp.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/guxdfxgxk.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gyejdjxdx.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrxeoamn.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gkwctasqq.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqzsbyss.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gljhcgzfy.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpwrlisd.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gulnibkzj.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gvocmetpd.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gczhmvwfm.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctwxfjho.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gitffyehb.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/grezfikbf.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/grfctgaoy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvprlmkmv.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwbmwqydk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gofjxaxkb.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gskeahpds.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnrymivp.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gualyllgr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/guywjlpjr.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/grrcrtqqu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwuthxsf.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhsniqio.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gitiyrejt.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/grkhbnuuh.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkubdnndp.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/giqxanpot.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuigylof.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gieqmjhwb.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfonvqiyh.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmxcgbjw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/ghsmicuyv.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyoxpqws.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gthivajbc.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/glcznuigd.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgfwryxd.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxulmqqz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gcnufsgib.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gflvbwain.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gqkwxqort.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gevgsdkaf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhoseowh.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gzaivvyht.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/ghonxwywr.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpqjkdlgh.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gjyxxkolz.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkwrpnfo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnlwmlun.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlzzdyyd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotxwsbip.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfyifpye.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gwxgvvyye.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gryltsjbj.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/glkakuobu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/geokcbapd.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gcflixomc.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gjoomdqcc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktfzlphi.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gyekldfpb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvvbjnwu.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gntytqeru.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gbssmyijh.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspxjtlml.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcunhknml.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgbijesy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfecytlw.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gomoohbam.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohuugtxu.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojueuieg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonqhiwtz.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gljmfysnl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqigtfrh.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvnglgrb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gibaaygcr.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gteajzydb.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gngkwnpxa.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqwhlmaj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gesupomxy.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpyavumc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gboavtvlc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdqnjath.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/glvfxxyzm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbtlmdmlk.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfkrvmpa.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsnltawu.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcyagfnw.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gnxzzktby.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gimubadms.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gdspzgzfu.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gvbqjluks.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gszgbhjvz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyihqwhv.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gsitiutrm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gzknoalna.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcwpqtpv.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/godqneepq.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/glmzhtfhm.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gnezvegmk.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gyxrlyhxb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvqomvyr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gjwcumrvk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddximbxe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyippcth.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdbwlwrg.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gkdwwynyd.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gtjvjbegn.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlbnwmbz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/glddbbdlb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/grqgzkayr.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqlrnxka.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwusqxjiy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbpkmgss.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gequzzntc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddzwdhos.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gvoisvhzh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gjfdcxksb.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdrgbngu.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gtnokyuvb.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gphschecw.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjbaryzn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwxndnrq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlfvpwdi.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnevdqry.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gsrccxulq.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gkbdugjhw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gebitgkyd.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmqgajys.sHtML


<!-- 参考信息 -->