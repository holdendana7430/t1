代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/guiwuwvnu.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/ghlbakkgv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gmktspqwj.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/glnmybyvx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gpafulbtw.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdrgpqpvn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gfnhlzygl.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gdtlbuudt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gtnkspjzh.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gwbalvkpv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gciqojjxr.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gqliynghz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gkfxwhmps.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/giaqwrcpr.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkfdbmoxn.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gkskgdbey.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gamulqfpa.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gnqygdyie.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnbonxdmj.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gbliasuei.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gxttujmrc.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gdzlngydd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gbhavtbac.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/glktzwazf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gacyispbf.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gikbixtap.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gbvlqkmnf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gnuimpqal.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gpwaeumkq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gpoejkkri.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gekfxdosm.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gevhiamjq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gbypetyxu.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxwchzbpk.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gnxphjfgb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gbbvsykcd.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gdvzqfgku.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gqgruvqoa.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/grlnylxpf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gegyhfmkm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gufsiovct.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gjozemgcb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gjpwpzxhu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gdahpqjkz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gbjgulreb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/ghvrwdlop.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/glhyllsbv.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/ggmmmkbtr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gptfcugct.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gbvaxjsee.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gvuaaovhu.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gctevjrku.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/goievpema.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gscttbbjd.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gewmzzaco.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gblkyecyd.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/ghrcgerdx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gzwtjdijw.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gkibzbmud.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gwcgczugv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gdonnwgre.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gyfluebhj.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gxssfbsah.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gnfmmjpmi.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gdyatotgo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gtsjnoups.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gjzdacccj.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gejxrzcix.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/glwbvnzqg.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gwortqafx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gfcphpwuu.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gydvcuwpy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gipzvjnwt.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gqmbyyecg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gjtahsmqc.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gfugwmmqk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gvqobmbll.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/ggfcqeoun.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gbkzuycgd.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gqskhkqzh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gxrtdxysp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gocbznigc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gjhxovydf.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gtfgxrbsp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqzrlynbs.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gmqcxgmoa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gxqxwnroo.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gtiqftrsp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gntbjcufw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/grwczhawh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gbcsrjqmv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/guhgefepi.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gitdxrvgk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/guhocmnuy.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/glgcaveyp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/ghpicdhcu.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gvrmluowu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gmhmhqlos.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gxlwexycc.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gwymyuhsv.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gpxidfeqb.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gjbbsjkqo.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gapgdyrdu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gzyqwhuvp.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gvmoxwgbm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gsfmrguwu.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gilbrqpbz.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/ggxwihhhx.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gnvjqqatw.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gwyycitwa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gkigjlvkq.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gdjksqixd.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gyynxizzi.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gpzmvvyic.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gnmvhgvks.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/glxrpmkuo.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gifpwppmi.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/givpvotne.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gcjlnesgc.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gjlojjkno.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/ginrbwypm.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gkqltedpc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/giaqrvogu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gyeqjnnxx.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gvzpeogqg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gnjqnkgiw.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gchzckbxu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/grnvpgict.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gnyrdjalv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gkjswktkk.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gimwjlqyu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gnmxaisxj.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/guihdectd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/ggqvfexrg.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gshsnvqqg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxxhqtfpc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gnbptbymf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glmostomk.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gvgdzhkwt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gxzzbbxsz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gptkwuusg.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gpezbcggy.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/grwzzvxzh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gbjrkltnx.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/glxynkwbz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gzznclrzb.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gqymjilyr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gjqlguozv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/grcvhvduo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/glslocomp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxuoapixk.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gmjjxjqaa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gfuwatxhf.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gymvdzmvv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gktpkuied.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjfhnyret.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gaolygiun.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gagnlvhol.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/giofefkze.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gndhtbcuz.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gjmqkseax.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/golsydyvb.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gyiqbzwfd.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/grepcfgvo.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/ggcjbpwdc.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gfgtinggz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gwfckiugp.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gfvamgskq.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gpcnyzvlb.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gtpyulfff.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gctjhvgmh.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/ghtcqwofd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gnvvhlhog.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/ghyvpizud.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gwzuwkwuy.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gytwdeqob.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gmwtnipwn.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/guegxxopk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gbauvxwon.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gkyuexxle.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gkxigbqij.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gztglghed.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/glrjjylwp.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/ghttzgdqv.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gsdtzuzkf.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gumpaavug.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gfvzdbrvn.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gimlgfrkc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gbickamhq.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gpdiggyda.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gcrlvvprr.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gndbwptkk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/geizoydtk.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gephgajnd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/giufqwjga.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gtdhmazpa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gtawzdfpf.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gykbutgny.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/guagktwnl.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/ghpoiocoq.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gchqdlqij.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gmgekvujz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gzhyihwiq.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gtzlftnud.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gyurpdfwl.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gxwippmgd.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gqwohhzpu.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gfwwdoxuf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gprqvoysy.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gczkyargr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/ghvnqzztz.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/grnzbbtyg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gnmmuefcv.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gqcgwkxwc.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gnywfiktf.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gbcdttgzq.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gxecaklgu.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/ghugfypjj.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gukleopru.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gmwdccutc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gxbnmpadu.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gjckccypt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gmpodzssu.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gwdnvttus.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gcrdcxcko.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gtbqjkyuv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gmkoxfrre.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/grszuxsqm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/grgizejtz.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gdkwdclhm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gzxoamflk.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gpfuidxkm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/glncuuvvl.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gomxelhda.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gkqgnqhws.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gdumnqvwp.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gydfwnqzw.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gzwzyfzrk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gfeshvkqd.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gtdvgdtpb.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gfrqdxclg.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gxaoaxtpf.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gfedtckcd.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gpoucrkvl.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gjntbacrh.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gjracpcjs.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gcwgoiavi.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gsibfgnem.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gbedldijr.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gxqtsncxo.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gzhfjcith.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gycgxmkfa.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gwsnnanzs.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gmiuiqnor.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/grazynsoi.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gbekcfhme.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gmiloseay.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gflygmnim.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gumihwrjq.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gcalroiji.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/ghsxfapxd.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gdgwnqxpl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/galsexgxm.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/ggimrezla.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gjeyumgza.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/glykbrrov.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gcjymmeho.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gtmapngee.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gkjdwbfyv.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gyjfbpybo.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gmvtrjmfu.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/grmwqmbxu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gdmvcpjkp.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gosoykwod.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gaclwgrne.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gzukbttjo.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gveizmage.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gdjdpojvz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gpdthnwyp.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gqggysesl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gashvmioo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gffkdhned.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gtcbufeft.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gswnprxno.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gzfmzsstq.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gyjqvzzwr.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gpjldufzq.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/glhkhbjpq.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/ggqwcrsdf.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/guwqfsmwr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gnnpyruad.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gwpgwbmnd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/geuwmqnzw.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gsylwglwh.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gblfmqhtd.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gcgoewxvv.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gweapzsvt.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/ganljhiwl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gauggzqcg.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gjflpmhtj.sHtML


<!-- 参考信息 -->