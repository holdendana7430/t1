代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtpjrfjga.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxdcqsxc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gowsboamy.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/ghjdfbwnq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrohpqzb.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gxueziykn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gqruavntx.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gfvtrjghi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsolwxetr.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gowfkfuxp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmskcnxe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gnkiezhqz.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/ggywlffdk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnebtsvfm.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/ghifwodqu.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gbkwumvpt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gscflnsgi.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghffreypd.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwtsatdu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggofmiepq.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gdukovndm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gtyevdmgc.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/grjzvkcli.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfbonxzy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gtlvppnst.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gjllnfauo.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnoodgwa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmrfasul.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbydojnr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gfpzjwpgo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwnfqkox.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxefbxdf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbbghryp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gebecakwa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcqzefzy.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkbmgvey.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gpvynmegr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gvwvakpgs.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpmglpbt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gxsxomjgx.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gmljghxmi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcxifbwo.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gxaxyljep.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlfhzenh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccbidxas.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwwacokp.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqamnczo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwirclywf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gapojsuiw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbaksnpp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssnhbtdx.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfahsxyt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsftccgfp.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gpfxngwfp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoqofhxz.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gepbuwlyt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/glaosggeg.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvffiftg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gnndarlnc.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gliyguxgt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/givuuqzfc.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gmjxiszdn.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gajriwyjv.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoopkrve.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlcaeexg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gksbqimhb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtxgchld.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gasuhjqxz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvlmddgqq.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gmtjlmhvf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gduuwidcv.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gpcgnsrrh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/glqxwonbr.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/ggegbuxnw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/ggkdwucsz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gusngcrhy.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gjozypuwh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ggyfbpgqh.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyswkmxuj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjbhjeob.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gywvigsbn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gvsoawdef.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkykuhld.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gmlcugxnu.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvwjebhj.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlaunhfl.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwxckben.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gockmbqvs.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gjjnvdhxd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxysqjcky.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gqivaaeie.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggowydong.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/glfxidrlq.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/giniqbvvt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjjubhqz.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxupnbyo.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxfhxlrgu.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjexhmptd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnstgiid.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gnebgdcpg.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gyutcazou.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gshcjrrjx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahwtfzzc.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsooagagc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeflriin.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gomjgoadn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwjixcyc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gdouctawk.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxlfnpgj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gcxyjmuhc.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaxahglm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gtbnsbhiz.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoitajui.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqxyaccn.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnccdgjk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/guxyftiav.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gnabsvfgh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gytugmxvk.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmrhmmjb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghkkldjvc.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/geaqdnlor.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhrqkxrs.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghabqbasz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxtbtxqq.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gbijzhghn.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gawpljrpj.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/ggjhysadc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gryolveqi.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gttnrhzfq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfmaqaoq.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gjlvagpyj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxesdxyoa.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyigfbtrw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/ggfxjkswc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyibvxkce.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/goponeiar.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzyliwjh.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gzfthzntz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gckmqxbdx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbjjtmic.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsayvowlx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtodljnsv.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxtqnioh.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gjegtilqx.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gzuccudvw.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gyiivuktw.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gfxpfaqxm.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnzueukad.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnhrybyr.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfjbyvfg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gubbzgern.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gsndwsmtf.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gozirilsa.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gxatkwzqw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxckjaoz.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwrueumlm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gashoncpe.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gxvklfptr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gwjvkfdjb.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlzrwoyp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gdkkydubz.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxznewac.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuzympbm.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gokdtqmwc.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfntaiek.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gulosluoc.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzermmsqd.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gfsqzrsgt.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gtvtfijfb.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/girvznnby.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbrbdolgc.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpesukgg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzxzdfcn.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwejskvdu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkinajgnq.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gppewajnz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxrxoxyme.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gapxjqnzj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqeduvjq.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gqwgjiuvu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwztaxbs.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgneqayw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjyatqnog.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/grzntvndy.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuposupl.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmwuhctf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gckytfswh.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gxiojhbzj.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvuiuezp.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgseuukd.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdgpscaw.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ganrcarme.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdktzqkmg.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gpojqoyhj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqciajpqa.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/grezirnqf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgoyecye.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwtskeiu.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gflgturnz.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gartdeqah.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaswhbip.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyetjqvh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gndlmhylr.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxnjcvwtg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzwebums.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gcilyxrmi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gbpzwvjor.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gryvytjfq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepgaxhft.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gxntfxsth.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gordoflwj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gkxitjolh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtfcwuwa.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gbcduthtr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/guqbypuep.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gjonpzaci.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gqqodjlnz.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokeefrmk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthnlrgjd.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gznwrhwbf.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwnjovbd.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjujjebh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcyafaxb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/glatlmmqr.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gfuufhydz.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gsoaaxmnb.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvjfxmlx.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/glgzeqmzb.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyljjswv.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/giszrthya.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gobvayagp.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gndyoazsr.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxkkdzbf.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gmgbsnsjv.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlinipgx.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gdtsjuzvk.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gicvapduz.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gcjiwqwis.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzdzeppe.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnyndedq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhzftbxv.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gdyhzqjvf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxykjighi.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gyjlebiju.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gypkzdkua.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkudhbya.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbfciheq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunkbksbo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwjuntoc.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxojctsei.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpfcdzdf.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gfkoqkeex.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gnvhqompn.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghschuxlx.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcvlyxpqz.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcoosasu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gnkxmoovk.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gxqpuader.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqlbmiek.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/ggczzmgde.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzpiuqrd.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvdpszvmt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gjxgedvfk.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcqcqvfl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/giwxmhcom.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/golpxcrgk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gbomztlll.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gnzfapahq.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gxteegzio.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpgqjypat.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpddcsxf.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjtgvyau.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gnystnnsd.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gasyazuav.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjnoadtn.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmxannms.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaguoszfw.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhopymgw.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gqspxoxqw.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gwliwtgqz.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdttjysj.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulqnpryk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggndogulj.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gtquonpqf.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gbtnenald.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfnydqnw.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gcigrgyuj.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjmoiwqz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmnfceah.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gmkousrlw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhsdwwjr.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gdpjqmzmi.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytuvawgv.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gzkrbynyl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdqniwcw.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gobuksusf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gajlnjban.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjeqtdsjt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gskylsich.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gprnfdosk.sHtML


<!-- 参考信息 -->