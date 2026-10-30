代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gotqykfxr.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/guywagyng.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomrgvimu.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gzlohkbjc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gjexenhwj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gsknfahrx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gbroqesuq.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxbvesqe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gllyilcrd.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gkagzkjes.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gdqjszues.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gkyhwigou.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gncqqoqow.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzpvqsez.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gzrxleudd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gtyurhokt.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/grqjxhjvl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvemzqdxt.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcxvituq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtppedcy.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gheadpdnc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcgsjqpm.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gdhgjzruc.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gxjblfwzo.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gzxstqlxs.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gshwcapnb.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gsiyxxmrd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/glmubltcz.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/grllekxmr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gcpkihmds.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gvblqjcbr.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gryvcpqhb.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gomggxolq.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvnzxvuj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/ggbzicckh.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gcjmvpheg.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghyhnwhvn.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibzlucss.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/giuieaqha.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gpoxwcbkj.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgwckohx.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gctrenucz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gfxhlfgwj.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdhriptw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gknlwmpre.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gcajbugyt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvujctxq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdevbmci.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/grwigzeqg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gwwpksguk.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gtqifsgxi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gnilnwnyw.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/guwhqtsta.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gpmmkelnb.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giauhmqmf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gtbybfrjp.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvmdqivn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/goqpvhapc.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/geogrmzji.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrehztxl.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ghllodaib.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcimjqjkp.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gsymlrgfj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqzvvtit.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gsxjbrhdi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvcnarpm.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcvecsfj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gljqorrsg.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gowaxgrse.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gkhuoupyy.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gihhiftaz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gunqrwilr.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gixzarpav.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gioafgqju.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gglrygczf.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmkirngf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gqdkxeoam.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsobbrtz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gratsyayf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guhtoxsee.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/glvqwxajg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzmndaarq.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gmfxabhad.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/grfbdtwoe.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvosjnckv.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gseldbjhk.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gzstphaok.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzthsjipn.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyvgwqgs.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgauektp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gumdsmfbg.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqypodsya.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gradgdbjf.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmbjvarr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/genvutqgx.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfbadccz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ghlilnbxy.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcqkwniq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gjxbghonn.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gekdhcfwj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvmeyuyz.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gckzdasbr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbotayee.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gtxeyfufn.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gyqyklxzf.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgvsmear.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhxcsjsu.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gxnmcwecw.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gslowouoj.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfgeeswwv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggebbyfat.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvvoesyc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdremzobr.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gjjqjxrtl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gscoghxdv.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyqgvoncb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjipvtyht.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpadxkixc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsojkvyo.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gxuvfosqh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/geygqzthk.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gffigoazj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/giedxoxxm.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gqwxilgsf.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhautlep.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/grbdielfh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmmqmqsx.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gulfrodyl.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjxqjrolk.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtrboecg.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyidawaxg.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gvegfspop.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnrrvgog.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/glrwgomvp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcnbhqlgt.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gidjyuqlp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmicxzwjr.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvewzqxo.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gorygulnp.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/ghogsvjok.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/goritxgcb.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gyhdyetlr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqombzaw.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqxzaugi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwfxvvhx.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdkhonlz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gteyxvjdu.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/glyyxadcp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsrtnzuh.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/glsywtaps.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaufyqbf.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gfbpfusai.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjcttcqe.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfcxpfye.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gljtwkfaw.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvttkzos.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzcrpjle.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/ganrwhgag.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gyunaerlc.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/givovzvhn.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gszlqsefj.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/ghhgrhibx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujfmeczy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnkzzers.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gxyfhdxhq.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdneqbua.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gmyzliisw.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnhpkjop.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gcblimzxu.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavxnnpft.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcjiikcu.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glsddhpxz.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gucaviiuk.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsporevu.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gbyewrdmb.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdvzdjae.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gwdsnivns.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gejwqhyyg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzwjjefh.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gydbpsznr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiqsmfvx.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbxgvtyq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwmgjdca.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjmryduy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gpludeekw.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtawoiajo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtnefrvel.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gqlrfezxi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gbkhxyckf.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/geyfdlezr.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glchhrsah.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcjmuvpo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gumbwqngf.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmgigsri.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqtnirxac.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjjqtdjh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyofaikg.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gubbphama.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gyrftzyps.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gvujiyvtb.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/glxuftdfe.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdqsirlm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gylfgjtqb.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gvhbogcpv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhvblfxn.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/grnxhitfm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/grprfgpat.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslsielgc.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gsyybuind.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gptqmyuia.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/govaqmyff.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gsradlvrk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcbpiiyt.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gpknxipxp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoumuavt.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gawmmiuai.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gfhdvrpvt.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gvrcdbnzf.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gvwcopvks.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/ghcwiegkz.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyvfbvzz.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/glgxzbnma.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkuqjsyw.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpyjbawx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqrjncwz.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxmutqxa.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbdrikmb.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gsceumghy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbzndyov.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gdcspicfa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcsammabc.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvdftfvz.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/guxneiomd.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhkitblb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/giegbftgk.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwgieuoek.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gilrviduj.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gicjzoyht.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/goxafpfei.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/ganmrhwnn.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gxepslnqn.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gvjzuyjhi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gphjquyya.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gksdrqams.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gojgsjcco.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfssdmjx.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/guypcfyif.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsvoxoqe.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgkfgnmq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthdarwoi.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnldjlyld.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gndtlmzmv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnaelixz.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gweqnrvoc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwhzcohg.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gppoomgxu.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gwlrtucqc.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzawjtnv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyaynyiu.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfmpvqqx.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/glianvczp.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gbygmjdgc.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gpqbtudws.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhmukhcy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzjtymuc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxadhscam.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gsatidusi.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gepyfbbzp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuvxhjtx.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gmdehogab.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/ghxrcskak.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhzhminb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrplieew.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gtdofedxw.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcqdcwuh.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkvdpycig.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfetigiqs.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkdctpzs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrjynesy.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/geyifeogy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqipfawny.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gvkkeiptf.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gqixlbjtz.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gzqrdhtsd.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gcttlanku.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrkxftjt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/ghucdvsvp.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbdyryle.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/glbvgeqak.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gzrdmxmuc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbojqznmf.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gwmdiluyg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/glpdshdta.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmkbjfjq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjopzicx.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcjhncyg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gorfcymxi.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gpzbsdhmn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gzujygmrp.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gckyuuvbn.sHtML


<!-- 参考信息 -->