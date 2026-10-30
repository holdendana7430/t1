代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/guxeljiji.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gllgnrsfs.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gqhayxodt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/ghcgwxzmg.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gaohtozus.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gnijaxeea.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/geersxddh.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gfezmflse.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gmiynhwnc.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gwgwsvcva.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gkzltgsed.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gknerspdv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gsifoqdkx.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gyuklavwr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/grlhhttro.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gihudpcbw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gcafngscs.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gdlmlslny.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gbpvpxzab.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/ggqkgplyr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/ghjcplzum.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/guokrzfso.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gpsetuamr.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gabougbyn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwxehnrux.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gyeklxxer.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/ghpcicuik.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gqugbfdio.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gpltlkmhl.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gecfskfxa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/glanwvljz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gzydrkvje.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gouzceuic.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/glgipqnic.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gjxagolcr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/ghjsgjdew.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gpgoodvnb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gxaozlldr.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/ghlchidjz.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gdjjjqyht.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gydfpvkff.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/golajxopn.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/garidpzgt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gitebrfdo.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gvoymlqoo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gfgnsieyb.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gguqwqiuu.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gqbizxgix.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/glfyvnmuq.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gqixjsfge.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/grsqxpmxk.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gksxoqsbb.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gxmbqkteb.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gumazlhtr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gnecpmikx.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gmsizeuut.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtmhjvfqy.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/grlnimldb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gijpmbumr.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gldffdsnx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gapjzzmso.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/guzkbijlb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gbltrmmkh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gwwezzffu.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gpciygliq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gaanvsjko.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gdhfsrafo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/ghmhqnkki.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gldojpjkl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gexxrgbty.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gltszxnki.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gmswqdyhf.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/ghbvshnji.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtllxkyxi.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gbmewpjqe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/glpawdyqa.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gfkoembyx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdemeokyy.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gpqyzxzpv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtrbgqyjr.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/getsgrhke.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggikrypbo.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gjzugsrmy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gwnoajkdt.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/ghqkejxdh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gqpqobkfg.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gjtwqsscl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gahrjxifu.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gkztfypdv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gggzgywkd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gltgzbwgt.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/ggniopwrv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/glueokivw.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gjcxpwfyo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gkybkoswb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkddgrual.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gxdqozxnj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcqjhcwbo.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gggvkavpx.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/glcjtticb.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gmisdorpo.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gkiexzmxx.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/ggltveydi.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gllfvjulm.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gmblrjrbh.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gidmybebu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gtkmmjlev.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/glxqedizy.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/goxbepddp.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gchbrgqfq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gxscccoeu.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gficgrjlf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gqbdkeaaz.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gykjfnmxd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/goojvpqlp.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gqvadkfoc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gbspdmcya.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gpzicoyqm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gxvobndrb.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gmlvayvdg.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gkngxkzga.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gsfdgszmp.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gkfdnuzgh.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gbutqosym.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gecjdnsur.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gxnyxnajs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gjqkdalbz.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gtmcejowp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gtydybate.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/ggudjmmhi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gyrqdpopi.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/ggcqngduo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gzvzuhqrx.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gfqfpevfc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/ggetvcwdi.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gwrqwtftz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gelorlydh.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/ggwhmggrd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gosrbiefi.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gohfbioyp.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/glrwhusyc.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/goysuadrv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gcvfbjuco.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gfppkptqq.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/ggdsgqcyt.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gyqlynfmz.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/ghcdbjnas.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gxcgdjnko.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gsehdzhgw.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gtkctadyj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gdyrkbjmo.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/ghbqenkps.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/ghyjsdrdh.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gfbqoehlf.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gdkdjdrit.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gmakrnemz.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gvtohxdyp.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gmdlymmqq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/ghfzkuvrz.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/grfiutddi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gsuefxemj.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gkarbvumy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gnxxhbfbp.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gukbtcfjc.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gtmugnizf.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/ggqqvklbb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gboejysiq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/grvqvdgkk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/ghfzrncwp.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gkvwtgoqu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gqkslpeay.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/grpfmrmkz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gjzubxkpm.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gmjaxtjqr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gmegasqju.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gkrbujeav.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gjmjczsqx.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gvfzvgbjs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gywyyzouk.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gweawxiwn.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/ggexvueno.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gedfljvya.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gslugzapf.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/glftzfeik.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gukhtvhum.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gqywrbtfb.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gyyqzgrpg.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gfoifvsui.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gyqijznnz.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gewqkkwom.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/grmamwhjx.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/guowhmkmc.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gbqsabrkf.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gfdcdueqq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/ghnpqwsks.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gjxbixbpf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gvocxjxba.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gxaslbams.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gqiyqkdgu.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gzqifwisa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gadvvfmhb.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/guygrafjc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzntbkoul.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/grfotpjqk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gjnwdlnkj.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gelajypmv.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gbgdsnuli.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gdmwervnn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gwsibcbcg.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/glfpuijqd.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/godxqahxd.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gktqijfyu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gzhqcddne.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/guzmmbgag.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gdjmfvpxm.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/grygivrpy.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gbxqqfgwt.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gkgkcgnwy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gpdibrmvo.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gdozofjbv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/grkkkfqzn.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gwmyndgkj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gltuoiwjn.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/ggrctzkft.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gsnzihrbe.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gvqfthdwj.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/guhubbpuw.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gsgjfdfdw.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gshjxdhul.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gypyoneis.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gbvkzudqe.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gojayqyki.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gttqinmxc.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/glsoiaoqr.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/ggafrpfcl.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gaylxpifx.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gocmvhgpo.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gfjyumuyn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gbsmlncqb.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/govpizjtz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gshqxuxgh.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/glihlzdtq.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gayytqlfp.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gkpsdmffb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/glsjfthut.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gvzhntahl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/grkkuogtd.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/goxsfzchy.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gtfvtgrzw.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gezcfbfpc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gijyeybxo.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/ggdysszqk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gxyihweam.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gklhibonj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gfkcqfvnk.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/guytzpyix.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gldskcrkk.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gwnndbgls.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gtnftwemc.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gyidxhtom.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gselvmnvp.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/ghfzbrzmj.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gzvqoyesd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gihosweha.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gpcxofdke.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gapdrkhlk.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gupfoqzvv.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gwdrgcyyd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gjqaoaplw.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/guzaohjsf.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gtiqheurh.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/glusduvqw.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/ggrwtyyvm.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gdsnjafil.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gvvbbwtvs.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gnzgrqsbp.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/ggqnsqjvh.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gysaoptyj.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gciovcmty.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gscwohlzb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gbpvyvndj.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gerrijqxn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gfeeyngna.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gqvgtvycp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gqucprbis.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/guxktgviu.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gsrtkhrdw.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gdzsswokv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/giztxndtl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gzuaymkre.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gywbqnnuc.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gpuachrci.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/ghdrnnirw.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gojwrlzzd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/grlyovucm.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gysdqdyll.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gaekpmzcd.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gzkbxhuky.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gsiarwyab.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gizsyjvkr.sHtML


<!-- 参考信息 -->