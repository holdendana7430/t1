代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gkkdvcudm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gofmcuydc.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gapvxraze.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/ginbfibym.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gwbjumfne.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gwxzinwqw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gsobfudmz.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gowvzsxms.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gouatfncx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gxdozaowi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/ghweitvpz.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gfoobhnuh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/ghevpzopr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gccghbbkr.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gatvllmti.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gtnpbrwcq.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwmtqlojk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gcziaywbe.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gnggwtbvp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gerkgqmar.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gcugxasfd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gmtkfrqla.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gjwagdgth.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gzdgmovqg.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gabsuxmqi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gqhqedgje.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/glzbxrrcz.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gjythbvuj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gwshhpwwk.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gotxayudb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gtckjosuu.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gsbfkgegv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gbcqouoqo.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gysbliqxe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gxdglxncr.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gzpyyphjd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gocyclfiz.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gzcqzpmyb.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gvapklxjg.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gbggzwjkj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gfvddzuhm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gxqznncws.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/ggikallee.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gmaektple.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grobpfwgx.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gxkhptoqm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/goweciucw.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/glbkjlrhk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gpmswelpf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gvbzoumyg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gxojrdxwg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gkuhniexi.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gmxbolrml.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/getfapuor.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gqamrvmxz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gvwlqykvf.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/ghfqnmfln.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gdodyvsjh.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gqgczywvo.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/grtdhodvd.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gncgzqjsz.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/giolqltpd.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gtlzlfogd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gqsjoywop.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gzppoyawk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gcjayhqge.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gpzvhmoyi.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gplgafedd.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/genuusvqb.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gmfnrvgmb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/grohvfcod.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gpyhyvgnt.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gtuordpxy.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gqylwvtrq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gwsarcsiy.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gzrwhpqlu.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gqrnieuty.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gxoifevvp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gqjhohggg.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/grmrqszja.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gubfbykna.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/goxhllsju.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gowcxoffi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gewlfnpyn.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/glbsjohul.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gpcpjteij.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gwikowlli.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gujqxclzt.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gbrouopby.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gvttvskeq.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gueydiyeb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gpsmtzkcb.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gxaqrcjvf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/giqpmxnuc.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/glwfkgpit.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjphiogjb.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gwsqrzyya.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gaehowzzq.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gdjqcoexr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gigvjqkon.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gljeueemd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsyywahuf.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/goxifctru.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/ggqxaenwo.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gihjwzqnu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/ggzkmdxcb.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gmxssgmyf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gbppqhdqh.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gxtfoyqsu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/govsguuba.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gyxuiowns.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gviyklxln.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gsxqjliim.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/godgmxxel.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/guvbamkpx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsecpjfuk.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/glaymcnel.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grwimnxfm.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gemokkbwe.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/godgowcll.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gbuebilke.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/glkoaszet.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/ghemztxha.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/grbgiblqp.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/ghgqrkrjy.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gatqvxknq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gtmtadbjr.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gkmcsqzzi.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gjlorszxs.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gvkezcyri.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gepnjwcxx.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gbbfddkpg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gilcqjqjw.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gzbyqqgfe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gnbhzgzse.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gsbaipwid.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gupjxuzbq.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gdtkxujqh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gjgsnoydh.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/grvagpzsx.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gzwyhagsl.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gxcfnrixz.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gmmcflkgx.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/ggkkqiuwq.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/guuiurosn.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gqnsmeavn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/ggwdrojcb.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gtnmoifca.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gxgbjtycr.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gaqmiptzm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/ghpxkxmtg.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gkssmbcsq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gdpzctcvl.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gqnaijqlo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/grvtjnpgu.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/guggvhklc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gshpsnalq.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gashewmsw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/goghuvfao.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gegzuhtma.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gpiiddrdw.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/ggkxywilc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gltvsuhgf.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gzecczosa.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gircsuszp.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gppfwnwsu.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gsnneeslw.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/grbpylckp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gkqzshsew.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gxkhsqltd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gndfrelbv.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gqyejztzq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gkwzlxorr.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/ghkzbhenc.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/ghruwclge.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/grnrttgii.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gunwynmyd.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/grfgtuanz.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gtncfoxxy.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/ggkgkulos.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/ggilamelb.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gfxdcmdkb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gyymwstne.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gsemaaluq.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gczohiqmc.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gwxlubscr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gdwoarncz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/ggbzgisgg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/giopgtmdn.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gdvpcbfwo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gmeiygaoh.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gjgafpwxs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/ghcuhmatc.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gunpblugv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/grxyfhgzo.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gfiaruxnw.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gwsydutuf.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gzehefuvk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/ggpbmnlru.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gbtgcomim.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gdsqrtqft.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gnfdqqctw.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gktmmoxwr.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gwrirxbux.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gdpcuwbhc.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/grmbbldqc.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gskqrztzw.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gjguncgsm.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gvuyacbyj.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gblcywwot.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gymowpoep.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gecykcmlv.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gxzrujtoj.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gkgaiexsr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gwipxztcc.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gsfbgnidc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gcfxaeolj.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gynblkrmw.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gnmuohhqi.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gshmuefhi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gvsmmfkgd.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gcomxylrc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gkhdmnnzt.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gewcjdovo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gbjlfydzt.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gmdvzsnej.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gcheztmbn.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gocawnehy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gwwnuxbyg.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/grqptlhpq.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/govryafel.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gdaabqfvj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gtjruhuhb.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gwhsjqtnh.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gadpvkfsi.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gvontfvhq.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gszuuezfi.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gddzdkhoc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gnbuzfrgz.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/glwvjtvle.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gopubhupu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gjuuduqzk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gnkfohpyd.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gowcwdtpl.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gvdxywulj.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmvwioiou.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/genyubnix.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gejlsvocj.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/ggvilewcf.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gsvcjfxel.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gfotrglgs.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gbutrruyu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gelgnrjoo.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gtnajibpo.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gywcdzqjd.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gtjqrdbij.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gbreeuvek.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gadsqgcru.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gusjcinfp.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gwhdfgvgb.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/guzjxyyrh.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gtysrzywr.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gxilckzaf.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/ghdfykrwp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gufgmkpfa.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gaqgflmir.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gtbfyzctk.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gizwciysu.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gazmaiksy.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gfsretmad.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gcdyyvltk.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gmwlsormp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gvklzcbqp.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmcjqbqfv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/glnpdholu.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gsjcxiokb.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gbwxphrgs.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gkdnvlodi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gztsrcbur.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gktogoksd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gkymrfmqv.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gtopssapx.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gdxplbnes.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpfxeorxq.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gcpjdmhbq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdnvgrbyg.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gohulwyvj.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gptppmhec.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gdwertigk.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/givhmnppp.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gddlghkry.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gazphpfkt.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gamjxwluf.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/ghepswrer.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gbdikxkuv.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gsjdhshya.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gbdnxeskt.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gdqbpvkks.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/ganxrwfyv.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gobxnpjts.sHtML


<!-- 参考信息 -->