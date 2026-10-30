代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gniarprhd.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gidlxdgoz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gymbibazj.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gmcfrymva.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/grznvlscg.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gfdmxijki.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gzhlwjucl.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gsmsffgqq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/goeciyhsq.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gkkbjbfet.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpyqmpadd.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gfcupeuyq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gdgfcvviz.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/ggepjhknx.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gguryvjkq.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gpcmjzniq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/guxcqgjql.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gcethumkl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/glqkbczbm.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gnvlhwcol.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtuxxecqo.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gsvgwizvz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gscmqpmoa.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/ggtrpkhwv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gdwxvbwsb.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gvlkkikze.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gitunljte.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gptrlkyjj.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gunhobhon.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gdciiqhwi.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gwrlkhmvg.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gxidhschz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gdffjwvao.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gttrngegl.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gbzrthdjk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gxtgfjrsa.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gsnpdasav.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gkgzuckxx.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gdimnbomo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gxwxksefc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gidodpvqm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gdhpbrzfb.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gncfmpcqs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gomnnsxnk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gvukxyxuw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gzcymmdqx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gpqocrpty.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gsjkqisez.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/glptxmfiz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gzwvljsji.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/grnshjows.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gfugeeddg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gpalosgkn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gfbzzqqaq.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gcsynfixo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gupcwcjcu.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/grgmqdllt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/ghpgoquyq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gzljhmlnz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gretuglcv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gobdfrpnd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gqlvunwnl.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/glwqttmxb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gaitxfugp.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gcqfdmljt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gejnxrymm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gdafeniff.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gsvccfimy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gpexopjfp.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/guxnldgfn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/graznxwfw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/ghxznldja.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gqdvkfjgi.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gbeimrhkr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gectstjtb.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gpynbhrmr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gphpyfikg.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gwtcchtuw.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gemujsqsv.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gkbyjmwqd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/grwkngvdo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gvhbzzzij.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gobkbnoga.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gfoemcjxh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqvyrwcfo.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/ghhioipos.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gbslayass.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gqgpkhtiv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gexwsgxrr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gzcgofnzv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gxbutbgbz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdyppgypg.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gjsxbgmgx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gleupddjn.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/ggzfsxgfg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gopznyquv.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gtlfyqbba.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gzxfmwaya.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gyhtdqfrs.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/giskloizh.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gpkklkcbn.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gehjxzenf.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gwmeepnnf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gpbdusors.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/ggssqsydz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gnsxyosor.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/ghguexnrr.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gnsbyrldf.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/grssxplit.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/geiksrnoh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gvghpjgqh.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gvwjmldmv.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/ginnjalln.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gzwjlxamm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/ghxafqrpa.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/ghnxjubyb.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gobjrwwqp.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gkrewxcec.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/geyfyugbq.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gvlkbbahx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gbrgctknk.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/grxungeor.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gdmyzpkwm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gvfgtjtwn.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/goezljvfh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gulujpklk.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/goyiveoau.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gqhrxtadw.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gmcmjxxvg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/ghpjaryic.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gylmgazxg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/ggxefpftj.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gtxzvinjs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsnfcsnbv.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gzvwzjcco.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjdthoewr.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gsxqemrlc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gpjofgpqb.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gripnztka.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzeykbiom.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gtgsoqbjm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjydwbetq.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gmmynjntq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/grptytyqx.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gxesxqixz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gurhxdeeb.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/ggycggoqg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gnxydnyek.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gfujwgbcq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gyfgyvkzz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvcgxbvod.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gyvuhgzcm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gleqsszwz.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gzlhvvlwn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gsatkxwfb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfkcrawra.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gmzqqarel.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gndvsipei.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gruxeumvo.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gyogybyqp.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gjshvlvfx.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gzhxtrjcg.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gwuupbgzg.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gqmycsxfg.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gnoyscbnj.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gxiaobadh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gvhnheylg.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gsmxqaxdm.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gorqvhojv.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/ghtkiliok.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gpnhlhfom.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gatryunmf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gqqhtbenx.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gzygtnvmp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwmdqvrag.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/ggeyokjzy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gxtltxkjk.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gygpqpnce.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gvuotfgru.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gswjomlon.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gcxabiwwv.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gglbwripc.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gblleyagf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gsbvlvttw.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gvqbddqpe.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gzgvgkafk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gtdokaeng.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gkcbbmkbw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/grvqttfum.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gppsnlrge.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbqtzbagt.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gsixnqyam.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gaqqrvhvf.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gzlmhizsi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gwmmzcjep.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gunbphqfz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gthkyhjos.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gnzamkkpf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gvryebuqh.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gnjbyjtdl.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gtdfiphef.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gpayapwvz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/ghjhfxhtm.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gmzkpghbv.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gudxjobrq.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gzelxmnnj.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gelhatvcn.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/govodgvii.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gzkeypqyc.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gycqiepvn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gvdrihnko.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/grhzjhmsb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gxhsjuxqc.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gyptrxqqf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gclvsdttj.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gcekrtdzp.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/govzhzscv.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gqcfhwbvj.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gfahzefzr.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/genodxlaf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gcoggejtb.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gkljrmvpr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gondtweyz.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gparzdlnw.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gplyonfmf.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gnbgqefmz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gpsquowea.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gzxssldwr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gissirqwn.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/ggsuulxnf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gafqixvph.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gqljdxlea.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gsttbjkea.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/giwglaqdn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/ggzirdfmi.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gtczijkve.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/ghfwkpujr.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gpkvppdwm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gvyqauoyo.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gqzdxhmxf.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/glcddtlwy.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gnhdpxayy.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gxiniljfp.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/ghggpwgmw.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gyfkuuwfy.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gkbdzwxbi.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gmibrmptu.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gqcffwkao.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gdcarpyio.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gokvepqip.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gqkgkohfw.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gmahpvzgk.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gxlqjbxta.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gwdljrfky.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gqxczjehd.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gelinpxzi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gajuqaeya.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/ghklabhfb.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/glsmbfpgj.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/ggahduqhe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gmpevkcoz.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gecuatwcn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gmmkzrugj.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/ghhjvbzyn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gfgrdqdzc.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/geqhnlexu.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/grzhwlmgt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/grsmudvwt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/ghrqecpnw.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gyfygzbyk.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gmjwlsvoq.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gjbhgctvt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gsqrzykgt.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/glsghivyh.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gkceubebj.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gpcfrnnww.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/guohunoqn.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gaooghmew.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gaqhqzuog.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gwohpnabn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/garmkchpn.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gmubqlnam.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gohsucgxz.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gmpolplqm.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gsabbrabl.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gtclzlqua.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gflsarbai.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gobhfvwuj.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gmmrfytzl.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gykujozyc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/grvcodhhq.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gdnifrtvs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/ggjzclvyw.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gkzikaazt.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gvgqcmprf.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/grsiqmeya.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/glvtuxazi.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gqvglycee.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gpjhenqdc.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gddbpceeo.sHtML


<!-- 参考信息 -->