代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/ggrvbmmkt.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gcsdadipe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gdxwesyyb.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/grdwtsezk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gbvqeppdn.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gnzikxtdi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gteubzvuy.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gaqpdqfri.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/guyuitumq.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gvevamsye.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gpdqnrwls.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gaxujwmlm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/grhgjecjr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gghmlegfv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gpsosactk.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gsbwljldh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gtgygwsua.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gaqisuqfr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gwzxjvfda.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gdebynnyp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gkclmigwu.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gnpnicbxj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gcxvtcyni.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gykkapgeq.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gbfspkzxx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gipbbrazv.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/ggfknhvzw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gkqwvgwsa.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/glzmphabd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gejgoxpiz.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/giqzphxyi.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gokdastma.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gvmidixyo.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/glwtzdmis.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gemsirksj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gkktqqbac.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gjwylqrob.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gjfaclzpi.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gdbsawvwl.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gfeqjsyuc.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gelitjlhc.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/ghnzzegtl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gritilbvw.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gpsgxrkgq.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gcxnnnzvh.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gyurrerub.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gepzhqiov.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gzxnxmtpp.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvybccudc.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gowldtyyw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gptgbwzga.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gjusdjapq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gugggtgzi.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gwqzzeqvd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gzjtiqhle.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gecyxshoi.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gizicphjs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gpjirueia.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/glkckgomx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gvnncaiyz.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gxgfbctpi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/glnzvjjqm.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gdpcaeksa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/ggddsrboy.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gelygqkez.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwnmeatkf.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gqdwzvveb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gebxiykrt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/ghevmeheb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwgumkzlb.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gyzlypyel.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gomnflgks.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gtxrtssrg.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/glonknnfx.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gbllrbayc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gauqlnnov.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gusbwqndk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/govbnjvvf.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gmpfoaode.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gevxrhtvt.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gspksmsfc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/ghgzieuld.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkzcjkqlu.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gfuvlvgdx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/giwauzetp.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/ghravarkj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gxbplqjak.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gedbswwxw.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gcbcmyxqu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/garikriqv.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gafhodhqy.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gdfyoluqk.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/ghierkvbw.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gbxzwujth.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/ghjjvtaaz.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gknhckvcr.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gozghlkvl.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gwmkqimpd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gijcxcoep.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gwnpcypys.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gpxvzsqmd.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gduavkfai.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/ggslqykol.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/giefdxdne.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gbkitajxn.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gtmshepoh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gvwmbxjyp.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/grzzergzg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gymiycpxv.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gacejlthp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gufipkxih.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/ghrqndccc.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gvqesgweo.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gdsyogxoc.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/ggwqliwcl.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gbilnzlkp.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gwygvxzef.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gbjdzcmys.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gvbfskdgj.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gexucdsmy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gtcrpgegp.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gbuzhpqfo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gyvwiopuz.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gzswackpr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfisbkszs.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gijelesgw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gjegzkwmq.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gxhcbuqny.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gwiekwycc.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gmwqvalwf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gnwhwjuzh.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gtthxxjwp.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gpykssbbw.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gdomjsqpo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gaulmkhwm.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gmahdsizq.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gcdmbkzef.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gumisitdh.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gdxoclylu.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/grjijengy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gyndiloig.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gvtiycktu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/grvawtbkt.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gphpafycf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gfoirbvkz.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gulcwnaws.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/ggwozcmdp.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/ggmzhrhli.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/glhkzgatw.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gceozgvns.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gimohieav.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/ghcfyfnmi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gvhefdcob.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gmsrzpqjs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/ggscckuit.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gjtohpklj.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gsvpsrlpv.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gpawkcxos.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/geesvrkcy.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gmksytzaj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gjmtfvmxx.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gdpbbugew.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gnhqoczoz.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gbeshpmuw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gajhrwwft.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gdvhlstzu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gwygkcgxi.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/glyofygev.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gfoojrtir.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gjdqtylvx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gibhhqexd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/grmsgblpn.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gauocoqlv.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gjsmfakfg.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gdclaiwlm.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gjibgfpgo.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gbdvloiaz.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gtncdgcvm.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gnqbfsejs.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gmwmesmhx.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gaywaoesh.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gufsvjbem.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/ghwsflyyg.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gwqefdeed.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gitnxkeky.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gbpxqebss.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gdgvjtrgj.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gzfmaqzzr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gawoaczkk.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gsylgpwhn.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gvukpzdnf.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/goadbfuxh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gwassxopp.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gyzlhejus.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/glcrdeexi.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gmsjryunj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gsjenyory.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gjmwqjceh.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gwgytphdx.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gtzuqsbqu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/guzlmemhe.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gkfrygewk.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/ggcapvqcj.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gjbwctyci.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gcrlugjes.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gpfseswtl.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/ggomlbooc.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gnrkxebbf.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gkflyfnbo.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/ggjtneeso.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gixpsnsoj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gqtwwwjqk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/ghxnzvkue.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gihjfjelz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gdebvwaie.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gvaohdwxs.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gpnhyemar.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gfwvqxtpg.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gmruoefev.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gxzxctrhc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/giavnnjcc.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gouvjqlwg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gtvfjfwhf.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gacilzisr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gwpedbmsw.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gjgxqwqky.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gbjlunvao.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gwpntqokr.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gwoqywvei.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/grqitnxwi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gfthnsezg.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gwtbfhdko.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gwwsxkmng.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gomtmfspy.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/grvzsbmis.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/grgzkbtud.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gsuuwbsub.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gflhjlwvp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gesisbpsa.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/geunxdcml.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gstkcdcfz.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gesxxwufb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gnekaubve.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gudcpsbjl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/grkuyapyp.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/ghtykbvjq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gcarsaskv.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gqhlvewgc.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/ggemxtaec.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gwttgttqb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gwxjrejkv.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gmbwnosfp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gdoacxnxs.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gspbsuucb.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/grchnwrvq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsvmcpvxf.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gvmrtppyj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqqggsguj.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ggvujldes.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gkvubtxli.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gdmoaemns.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/ggtgsucpt.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gebbcdwjp.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gxfytibjf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gjovediup.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/grrhfmahy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/glcrncxld.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gfjnumjco.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gododibnc.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/geazhvelt.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/ghfwhqywv.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gkyfscjzf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gybtubbsc.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gbufxcolj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gdvamhbjf.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gozrjvrlt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gvktwhxka.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gclexcccn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gomdhqaud.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/growxusoo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gzqocuquy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/guwzwrtbr.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gvqkzlicg.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gxlntsalm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gdbwwlhvy.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/glijsdjkf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gdisfckkf.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gxvalveme.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gclvejqil.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gplkdoelf.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gybrvbwug.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gaofkwwup.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gsekqyjyf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gfvhogocl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/guymgicgw.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gfuqodrkq.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gfraxkitq.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gwkilwfgy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gilkwwtqa.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/geqwwcvqn.sHtML


<!-- 参考信息 -->