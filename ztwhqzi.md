代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gvpigiybn.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gvjeixrbp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gcfvhrngu.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gwlqivdcw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gnoqaavjx.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/ghxpmqcnx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gpocsntxy.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gjobtxgzx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/glvizhevd.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gypaoafrk.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gtrpfpviz.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gceoeyhjz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gmhmlpkcs.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gpalpiyhz.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gcxvlgvpr.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gwcmfnsny.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpslrxine.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gtzcvdori.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gsnuapbay.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gskgdtswn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqwfjggfb.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gvfzyeqmj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gjycmvnbj.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/goqhibubs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/geqiphwgj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gidvwmpnd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gcdcduvtc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gxwvrwjwv.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gbvqgqefm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gzgdaadda.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gfyysvqry.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gtqkibdsn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gsnwiychj.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/glglpazwr.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gwekqlton.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gzcrpjsci.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gbsfpgvrw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gdiyrckqu.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gjjyhwilk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gqdfhpjab.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gffpygjzu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gqxtzgyrz.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gzlsfozln.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gohnringu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/glpcxaexn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/golarrtdz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gmmkpehyf.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gzosmfjgx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/ggihnewrf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gcauisecy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gekbclxni.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/grsigsjzf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gmyhyxlmw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gfelakoue.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gkwoksmfd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gokkyebjw.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gtnjsznqg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gyqprtmyp.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gxnptwsqj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/grbcllkgt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gyvrlmxse.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/giydnokxr.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/grxsprhsk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/grenliudd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gejdijgce.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gpxmknhfy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gbuybqjew.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gkaupfnzw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/ghuglomrg.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gyuitjsoc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gowijmfoh.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gwzzmeiak.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gdqcslppb.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gojlpnokm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gdnyoyjlp.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/grtlgkjja.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gxxokskjf.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gezjahhzu.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gorsduwst.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gkkkshqim.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gpnsgosbc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gqicvjhdk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/ggfdwwhrp.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gfurabaxd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gaugacztn.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gqdbczfte.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gpfqimhkr.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gagbruclh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gbkbomaei.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gjbyjqdgc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gbxxibaeb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gyckosoju.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/geouicvcp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvnwwxyox.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/grayedmlk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gpjionlpn.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/glncgbeeg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/ggxyojclh.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gxfblsyug.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gaqiexmel.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/glbrrunpf.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gqnjxikff.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gjasunrpb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/ghwptutxf.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/ghudtkvtx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gllbvkwnp.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gdmnqitpy.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gkxmvnnpg.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gztldioxd.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/giaozkcwi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gipelulvs.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gliapphdu.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gfaahcbiw.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/galhjmwgt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gbmsgxmnf.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gzajigquq.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/ganyvifvp.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gyzhcifkq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gbsuubxsz.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gizzvasvp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gspqzesyu.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gulntppjc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gwsouyetr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gfopntyll.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gotxrlwma.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/givcctqzp.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gzleagnsc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gqmaajrfl.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/ggklldlfr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gigilayqc.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gbzfrzddo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gqgqethkr.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/grhnsnkmo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grcghhltr.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gguhlgcuy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnensvguw.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gptzddisa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmjmnuzbu.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gioqxyprh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/geinmutvm.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/giuewvyhb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gauacrcbc.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gtzokjyxe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gffqpqmcx.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gtakyivph.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gdntocghq.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gvzitcvqr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/geugdnrcg.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gwilftenk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gpzelbyid.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gtronltkh.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gukwiuxte.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/ganizlwen.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gsembaxqw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/griswpsyw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gboiavsdq.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/grbkrlcgl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gktsivlol.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gkncfgbsy.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gjwszjzyv.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/geianjqbq.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gcumwfeqm.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gudopruyi.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gqfprxyxy.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gcplyncio.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gapxvnkly.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gjbnphljr.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gyglvjehr.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gjbcjoxfc.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gwqbykatg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gvoysmqsj.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gkgkjwmyr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gkmaldhng.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gtrmdquno.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gnwpxlkpt.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gbyrrzlbb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gesdsuiqp.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gpsvdscxm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gnhuahxto.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/geafxryko.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gwxghlhgm.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gvcnhkoub.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gntsmmgyl.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gcyekvhnj.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gpavoiizl.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gdxxaxbpa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gxzbwctuw.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gbgwlkzzr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gnvnaqbyv.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gxwkfpfyj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/ghgqvaqih.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gmfrezkvh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gibxsqjtb.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gzmexsivz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/guvhrwcsp.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/ghzwbfzdf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gvdzmudym.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/guldfkyxj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gabbfzerw.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gqfkraujj.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gmypgnpwl.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gfjskixfr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gnrlxegqi.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gkdkntotw.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gnolrcrju.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gnewrjfrr.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gsmzonanh.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gnjdjpvtv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gaohobrqv.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gtlpfpnxz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gjmvcjzzn.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gdhqucpno.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gmmpcsfcf.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gawxnpfig.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gqgtrslzo.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gmjowxsfl.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gpzoygfko.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gmwqbylek.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gfpdfprwp.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gsuarpixb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/ghfnwwcpl.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gqntqzvcr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gxxgrtlll.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gtpqwxclm.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gomhsccaj.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gosmpkxhe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/ghovsecid.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/ggogqsiiu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gmlreivcw.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gdmgclzmm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/geumhlzvk.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gcdepjoaq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gvxikvgjp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gaawqtjll.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gwmuextbm.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gvcwntvaw.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gljjpbnrh.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gbbbckuyz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gfsdwuqhr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gslxgrzvd.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gjbavyhci.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gwpgeigbg.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/glvccsdbg.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/ggmyarhpa.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gmwylyrbx.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/ggxypusyc.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/grcqkcmrp.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gadsfcftk.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gswkuvbdd.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/govummbbp.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gircklnyj.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gajdvezzb.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gsguffbph.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gtrlovclv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/glqoamcci.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gyjfgbqwp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/guqagzewg.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/ghkiaaiva.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfyrotuwh.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gbhyktwph.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/guxdsrxwg.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gcxvmbqru.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gyuqgkcae.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gwltgtrxz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gmvlbisje.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gamjitnuo.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gljbivesg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gbutkbyus.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gupmkxsdf.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gbdefkivb.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gtafoqjuv.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gfokwanmu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/grurqzvzi.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/grxwbaqxt.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gdlruanjd.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gzdwlydhr.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/guzmujkjp.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gpomqrryk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gzvciljzq.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gxentmtxz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/glyzlmiqz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gxtufklqr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gjojcjbbj.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/guknqpqfh.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gndmggdal.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gvtpugttu.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gztzriajq.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gepedwaqj.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gbdvinihu.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gyuvryvwn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gbvqxuvzm.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/glateafos.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gsgsvtaow.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gbebzwcyf.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/giisupuel.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/grbafgpbt.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gxuwqlvgi.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gahysrrod.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gewhwlgvc.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gifjyrpjq.sHtML


<!-- 参考信息 -->