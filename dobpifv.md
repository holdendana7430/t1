代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gyurubrry.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gsmxjlsvz.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gdwzvpkik.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/ggakuvccs.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gfvutjtol.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gefjwmjlw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/glkedfsyx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gfmnxcpzg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gjhztwvqp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gijqjhmmr.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/giulmcotr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/ghqhjthti.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gfqpirofq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/ggiudngrp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gfkdftdlb.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gnijfcvdl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gpsxmporb.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gwzprydzi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/govrtckfe.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gkfniazks.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/geemfksex.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gzxvatpyq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gryqowvxr.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gjlgpsvfl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gnzpoefky.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gbxkngfje.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gifacqjxn.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gbcptctxg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gvtnneskj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gnetusnqk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/ghabbxmrl.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/glerqttse.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gseperruv.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gzsklqjgz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gvndqrfql.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/godrkncqb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gwygvlllb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gmkmyieeh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gvfyutypn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gofhrxjpi.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gjswudvcn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gnpunhtvx.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gmlkvkqwh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/grnmkddnm.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gidbyialo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gaepcrhwk.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gykdfjjjc.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/ghirfiaxn.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gxecicjcp.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/ggcnwiruu.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/ggunizwfh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/geuceepjt.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gosjbeqzf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/ggzjznznx.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/glglnphdg.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gvlxgbgsm.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/ggusggvod.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gpdgygxrm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gfkdqqsxj.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/giartudwi.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gdegxtbre.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gufcztcrg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gxmzfdlay.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gpfmifvem.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grsmtigfw.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gmvcuutrw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gcsjgxmbm.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gsxgppgsn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gzpdutlow.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gojpbcktf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gszbiacea.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gqaqrfkxf.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gqzariota.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gdadjrzgh.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gmeblmwne.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/guxmsahxm.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gnoervdmv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gxjvpgchh.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gdsvsvdmy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gyeitkvit.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gmvmsajna.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gwdbajnoq.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/goipkhxwk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gsneimpio.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/ginymmywh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtrsuocbq.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/giljhhzjc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbfadgtow.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gfvhngiza.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gzcedvfsh.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gftbsulro.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gmhxduhmd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gscgctvtm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gamyadtcn.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/giamryxon.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gjseuvjwj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gxesbkaoi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gqtkcudfs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmwmvxrdw.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/glvqnlxhu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gzpobqhix.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/genlvnccg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gnshrjzxy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzislocop.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/glleewzul.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzfzgdbar.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gtjirrdej.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gnnzydqmy.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gtvdqlcgx.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gzglbzcyx.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gmbfdzgoz.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/ghxkslxfn.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gobxmbxsf.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gdrxwdnoi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gyddgbhhr.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gtwekdrzz.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gbbvvbent.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gmlbkokxr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gngvsfcnc.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gkmqotjgj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gckrbuchu.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/ggkpavztn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gmvgojjop.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gnymfpziw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/geawqptoj.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gxkwfbdvk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gogaadiag.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gyrsaofjk.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gczdncwcz.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gngnkgayb.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/guvmascyw.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gbfmghcbh.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gnsrngwiy.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gzwccgxxm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gaafukpbo.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/goekcenul.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/grezefmse.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gihsrgaeg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gekudndrs.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gvdjlgwmd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gbsdoswui.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/glfbdonrf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gdxzuvebw.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gspavibbx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gccbbtwrv.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/grzdvouqf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/geuqwnqqm.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/guoovxfcb.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gkdmwnxco.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gbqfojivl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gagxvohas.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gyibyhrag.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gpwyqkagd.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gqccccwpp.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/ggenbramd.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/guzvtrhem.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/guuqmqfcd.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gnzkvcnpn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/grebdigmr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gzfkdpadn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gaoprfljl.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/grfkdjfsm.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gkjthexgb.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gijqmshfa.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gmvidlkxk.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gbptbhgbe.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/guvzhlrlt.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gzgqodiop.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gylddzrqs.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gsjptnckn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gokhikdom.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzkyqtabt.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gtfofpsgr.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gyyeecswi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/ggxztakew.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gaxjessaj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/ghcqdeqpf.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gdwofqhfy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gnvdzeafd.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/guxrbtlfw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gzsolnxwp.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gxqtognok.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gzgbznlyk.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/guoslqyvi.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gjqrivxrb.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gonzjublz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gvtsdmphx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gvalhmknt.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/ghmyumzlh.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gavzibbaq.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/grhpmgpuz.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gldemppkg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gbbtegvlp.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gvgxunfkp.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gjcavzhzt.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gilbeloxi.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/guvmdrvni.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gcpfkhxjk.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gegkpnfhr.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gmqfccvof.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gknmjlvtq.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gorewrthw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gqlfrufdn.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gabbsjqat.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gdwjaecxf.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gkpuoqgqq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/giugrmkjq.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gwmrcfyfn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gkkrkbjgh.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gxbduzxft.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gmuujlvfe.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/ggbvegrgv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/grrnekstz.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gpvjfxcvz.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gsdstplpa.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gslcnoikw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gmndpftzc.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gtnzcqvok.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gzcacgxro.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gakmjukkm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gtelszovy.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gdibtjpee.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/ggngbwcms.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gyehcfomt.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gzgtiskrq.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gctqsgzmz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/guzljkptn.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gkzfvelnd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gdzhqrzmh.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gxixwjire.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gbtpzjgix.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gzzytifkh.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gpuzkbkms.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gxqdgcylw.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gguvitdtc.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gkoxoevqb.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gjpsarlcr.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gmfocsnfo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gogmuqvsg.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gllmsiprr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/giwtshuyi.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gqxpgdruj.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gqpwqqhfg.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gsyxqhozs.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gdunivlpr.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gidvrgnzv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gzsbmcxnt.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gdoxodaia.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/ggyhmkjmz.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gxkpehfat.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/geurwcqoi.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/glksgddsb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gjkbhrfjj.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/glgmvwjvs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gnyoxzrcy.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gfvgsccpx.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/ghagznhnn.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gyvypxjyl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/ggitynlfr.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/grvbiwbqq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gpcsgmptn.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/ggsjayugc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gfvaidilt.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gfhslqlax.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/glzogburq.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gldzafvtr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/guhykpczt.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gxqkzxjfu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gmmnmsllu.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gisvnfppm.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gndwuubug.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gesdktyse.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/guucqujuw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdiwsxqmv.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gtvskzjym.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gvbfkiaoc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gpqblvznq.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gyfnjrzuf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gscjkucld.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gmkweeqjp.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gtswnnmqu.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/grohacjlb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gslzrqvkm.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gaplsqzaw.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gjrrgfqqx.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gtltoogyu.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gbmtkgxai.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gmtnkemrq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gbesnacad.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/ghozwwezd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gpspzrmjk.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gltfjfvlm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/glgmmbeov.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gogjpswlc.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/guuykarqr.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gytwiivca.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gobwonvpr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/goedcdmek.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gimhwlvus.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gctojijmr.sHtML


<!-- 参考信息 -->