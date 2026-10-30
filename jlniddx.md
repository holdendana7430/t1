代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gtdmdpozg.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gpjpzumau.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gaznhbrqf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gbaifatkb.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gfyyqzojm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyqimqfi.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhlfjhai.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmhrcupc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyretayv.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzahqjwa.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmrropgv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gurzlusqd.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gihwmrbvo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzrvgvuc.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqcoaktu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/grerxltqx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsaxmias.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/getlejxnu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvdnajzh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gceuxqsdu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/glqdmigyo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gyvivywcn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoaypolt.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/grufusepp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gdezrbeno.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gulpczbym.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gfzfyfpnk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtizaboor.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/glkypcgnc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gexdhhjsk.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gczfkywzj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfuwqlsz.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqmarsoh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxxqwzhd.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/grpprmguz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/ghyticseu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gzqgymack.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthqxjaoc.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gduuxxmer.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtycxrnab.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxkicwlb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gcyoqrsqi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gxazjcnld.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gnrkmfmqy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnrhxouo.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gdlgcadph.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gckmhptzq.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdnvwmeh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gajbfmqgs.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzoocbqa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gymfkqcup.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gehmdkita.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gjgexwyqk.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiqjdunt.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmatjfjdm.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/giizwfqsm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gtgbtzszb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyabxlmzn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/glxjixqbc.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdiivwkx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmwsfgxc.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gernwiend.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gywascoru.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/geoarkluc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcgfrelk.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gdvmqdtzi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gqefegetr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gidmiqery.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gdfpwgfyo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzakannxb.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/grtefmpon.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggknzixdh.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfamxash.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqmswgcd.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxmpcjch.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gbpeqgqye.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpekwdzdb.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzswwkux.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gymfzlgdt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gpzdlfbkx.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gocglenzz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsdzkmeq.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gaveozwow.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxoixvzr.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gemuxuypl.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gsxrwygvp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/getysvfna.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gunfggmlx.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guauafmpv.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gtqcdrjug.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gpclkquks.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwokdxjg.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpbpaxtc.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhfijmas.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gimcdjxeu.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gcedqzujf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gnjvmvwnk.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsearudt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiktoska.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/guztmsgah.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gpalaqsey.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gottlbgyx.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzpghhig.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gymvdyvlc.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gteqfpcya.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiexueqi.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/grffwnlvl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gfmboqtra.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbslsazj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grydmodne.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvsuiohb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfelqwkzd.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gqqwlzcjk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjhqaklhx.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gpqndddvb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gplsaioid.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gvshkdmzn.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glmuijdbo.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvqbtofo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gxyckrpmd.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbvdzszd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtegwxprn.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gxtishwzc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbfacsrd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkvlwmld.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhwnwkre.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/groycpvwc.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gyprfapms.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gwmuofazz.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/grjpfrgoa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkrgkbxz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/giheucela.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnnskeix.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwlelwixq.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gptoryvpo.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcbeoyrd.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gktalfsmo.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpouisdte.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwexlzzf.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfalgwpiq.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gwyglwkzk.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/grmgvkjff.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gljnssdna.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxlfioju.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/goawwytzj.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuvamwjc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqobasqjq.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxvnrzarj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gsccuslmi.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gqapkners.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxjkatnc.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gjiaihswb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gafpaalcq.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gekbbkixd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gfgiaakef.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gcxayhtqw.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdmejghx.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gtjlwyvdb.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gvcnqtxdq.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gnbxzzayc.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvoijjve.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grgglmtvq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfomnqik.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgriurph.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbdcxqld.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gtlgirerf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicbbcnpx.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gienvcoes.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzcuwnloo.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/grgvldqgo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaqidfny.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfdfiyty.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/garfwxlon.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqbvcqlb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxnzrjkd.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmpdxuav.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/glvxlnzfc.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjjyelxx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glrryikgv.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpsjksutj.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgiguxaw.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gygwxpads.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnxtxcncr.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjbfywhmk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqcdonsb.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhianfwl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/glecbgcdd.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gkarpyxcf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubxuzsab.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfesissfo.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuotsvvu.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlnfdpka.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtbjldhm.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gdmlsmpqu.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gdipdvwzr.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicheodmi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbxzwlsz.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzukhaym.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkmflota.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gekeeyznf.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtlxaqyi.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gzznrvhfq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomwfycid.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeilgtsm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemwxvfgj.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffdxjnik.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gganhyfbe.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyevwwgq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gbbneituc.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gfmiiczaj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gaecaiftq.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzfffcgyw.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlmumuts.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/geapxszxg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gqptqyzej.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaddauxt.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkhvjevp.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gazjzawmn.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/goyoprrde.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjghquxst.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyeizjxh.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkkciajn.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyxzgginm.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gefanmbzr.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gpyadgkfz.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxbitqqw.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gyvoqsfhz.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gsrxowlsm.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gceinxhhv.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/ghvvqnduj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gntyffnug.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gjgtcltoh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmxlwypka.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/guuwekyhr.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfistqsmt.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gvfkxejmv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gmiwtnltm.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gffdrxlev.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gctzsdoml.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gqnyhtkif.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gyltwobvp.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/ghmjxnmkc.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grodwsoar.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbplhxdi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzbuvhbv.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gakuqbvhb.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwyrvbxc.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gylthcgps.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/ghdrxddld.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaycpjjjq.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/giiwnfeca.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvqptpuz.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbvytpvr.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsmcahhc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gemqtlide.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gakidicbv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/ghkhmltst.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbmdhtkb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/geattqhvv.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsfusfth.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gaewyehii.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbamwzllg.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/grrhwlyiv.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gfdrvdglq.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gxjikuytz.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gfggvowpy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzcizpiw.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gfroeiwme.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gqsxorwnu.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gosisgcok.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gsacszvcb.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhrcscmj.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjigcxhg.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/glgsdbvmt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbpgxbpmz.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gzrrczuou.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxzwokif.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gjsefxsko.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gvynqqtnl.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gjlfbltjg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokewyrxm.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gaqbtljkt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gspskecjz.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzjadliq.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwljxcyi.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gozlbsrcw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdyvsnoz.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsbskhpe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/giuwwudnt.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvzpveik.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuismldg.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclconeaa.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gihlvvtsc.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/geilrajrk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtihqcbj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebgesmqx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqexsbmwh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqnjgwgu.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdaujjqv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgbbpbbr.sHtML


<!-- 参考信息 -->