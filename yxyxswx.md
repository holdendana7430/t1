代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/ggegojpzh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gtabgmrtb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gnljtzdok.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gegnfjuyu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gbesmmpon.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gyorpycwo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gmoqpgzvj.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/grkvlzczt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/govtlxwuk.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gfpaqunna.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gbypdgvys.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gexgqafmg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gbmgzyfpx.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gwnhuhibu.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gkyjfocse.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gsgqglhip.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gykxhjeqt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gkulnpvgt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gwiyxhycf.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gdiksjysw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gktcmwdgi.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gkcfuvdkp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gsgjmdewr.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gyxsmqhuy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ghmvybfqj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gwptdcnbw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/ghjcvznvh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/glxyzcrdp.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gcpejqalr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gnfwypowg.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gxfzmsbfr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gymotqwhz.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gxyluyhrp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gldzobnpw.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/ghglaadpx.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/ggwwuoneb.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gayivmwlk.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gsccaqunl.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gcewaxdsp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gwapgqgyq.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gngfobcvx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gvefoajfu.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gdbkpfvya.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gybvtyblv.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gwcazjgyn.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gkoikovvq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gcyugiqvs.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gliqkqtfj.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gyhmnejql.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gffemieot.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gazmoubiw.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gpukfejuw.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxjahmcfw.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gqeupiigg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gewlixhqr.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gawiqkbxm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/ghiyuoisj.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/grjgpnbjz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gvuipyght.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gwzmryscw.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gyudpzhhu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gswyqaabg.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gwhipvevg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gerdbfdns.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gmokzbbal.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gwnmunslj.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gvmzzqtbg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/geootqjuc.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gdvgjfard.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gudkqtrhi.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gpirxzuyb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/grwujgjcp.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gdhmdtjeu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gfcupgxvy.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gwqopudno.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gihkjzmay.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gdnfqdgnh.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggiyitybs.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/goeoucyyb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gvquomtgi.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gukcfpcfj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gvoxcpkbk.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gwirgggtb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gzkvcfmoo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gnwicjvpk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gtoqiceqj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpxjjbdyq.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gfaztzcnm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gkdnsgqgv.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gfotfxadr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gqntmykpw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxtrjnxng.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gffnwoccl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gypqrjlux.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gkljctpgm.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gksubanyf.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gmkhshkpl.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gpbzhduej.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gprkadtne.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/grdnqqxjo.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/geimxdwef.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gnwondkuc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gntbcqmek.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gsdujtezp.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gckvdkcri.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/goyyhoeop.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/goadhkqef.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/grdvlgstd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/guapyrlyf.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gqiyxhskh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gjqxumqic.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gcfmwlmhe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gslhgjcxd.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/ghzibvour.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gmxhnsnvw.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gmmzekxhv.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gtftkrnds.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gdcwloquc.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/ggeahrrvv.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gexluyzft.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gwpmbaqve.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gvzzogsid.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gfosypwrd.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gwvzrdwpm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gqmvddjah.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/godqxcpse.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gtbcnqtho.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gwksgxcxq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gaqdszxof.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gqbinhhge.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gccyahefv.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gpahclsbn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gvyvqlkbv.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/ggtumnalf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gmupvmahq.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gdardejog.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gpreeyafc.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gzxtxhcsq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gewdraiah.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/galhekpbn.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gydjydhzl.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gnxrxncil.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gtcktybeg.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gfftrxnzb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gdyqocofq.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gpgzmclub.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gpsxoyelt.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gmhxpyfla.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/grtvcstjg.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gwdzyxyzj.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gudkprodv.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gnlzsxrll.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gngmtkmcx.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gpcnutdaf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gujwktnpe.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gwqjvjrjj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gqayrmysp.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gkapaoove.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/giazldggm.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/ghfcqvhpw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gldlaread.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gcixjndei.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gxsrwdlzx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gzczaluxr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gufxftayu.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gjpfxmunq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gbhwddvut.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gqmphxqhk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gespgxglf.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gdqpqlryu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gudyyhbgc.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gzofloxie.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gnzkhtxlm.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gmlgyerqj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gkpkxnuhi.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gyiapgzfj.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/ggfmbwxjr.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gkczggjiq.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gjbmygona.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gxbxtgzhb.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gshfwlvnu.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/glcqnmtrr.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/goxkauuse.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gfaflrlwu.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gdnvycyjm.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gnhjwknxh.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/ggoknohlu.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/ggqlpkyib.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gvghylfkh.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gvltxntms.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gjtqgjayh.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gujktlytw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gczstzbnz.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gxoaxslud.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gvyedhxwc.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gzfkrtsmy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gzpolzusc.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gfpsixacx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gawuhictj.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/ggohtlekd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gnneyiqdr.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/ggavwrlov.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gnxuoumnw.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gmtqiwpcs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gyploewxs.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/grxxstnqi.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gpqhnxfgn.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gbhfbgxid.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gzndtideb.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/glreexcte.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gqiapelbv.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gwpowasur.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gmoeichdd.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gtyfwxwsf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gcepjleed.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gotxspdwl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gmiqsxgof.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gnjhgdcux.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gwcxwfwfs.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gejjxzsej.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gjzlzqmqc.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gtvytbden.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gwpnuynlk.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/ggqutmjzz.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gmupcusym.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gvmzhfgbs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gzrzvxerp.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/glskcusyk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gdprovimh.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gjzwudmwl.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gmwlwfqnf.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/glezckalz.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/ggbmfjika.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gqazfykzy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gykvwgikl.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gxbpvhydt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gsraeppzd.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gvboxxsch.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gumoburrq.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gljydxsod.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/greolldko.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gkzwwhfan.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gsxhbsjru.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gcvorxcxx.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gdwtijffw.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gtjgieitc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gxswudxtv.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gvtlmammf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gjxophqxh.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gzyrucknh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gbtuydwqo.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gfopprxqc.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gtuwgphwc.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/ghvdexddf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gmubhbflv.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gyzqgrlgn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/glsyenyyd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gtmtmdjqm.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gtnlkiquq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnlhbhwfg.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gwawvlkhy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grdbfmbbf.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gqffgswhz.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/grhfnyrdh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gdarmtokf.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/ghmwghxuo.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gjozcslwn.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/ghwlnzjzd.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gacwikxpg.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gjxlemhik.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gxsuhgcgp.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gkujuwznt.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gjqzglesm.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gkihiednm.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/ggalembzg.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gcuaveroe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gdlzrcuas.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gkusoexqr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gcakkufxv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gwylonnvt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/ghbfezkdl.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gteydevzi.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/ghbhuygbp.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gzqegntdp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gutsaagsh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gefiqnulc.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gsqqsbter.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/ghhzsmpnt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/grjrowkyn.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gwpbyqdbq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gouoqplsk.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gazoaejlp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gevbxhevf.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gczrqrhkd.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gtpgarvfy.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gekwalvca.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gxydvsglj.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gnjamtwkv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gnejbgstu.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/ggtmtfplq.sHtML


<!-- 参考信息 -->