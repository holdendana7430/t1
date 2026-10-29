代发 wailian999

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmjwrlmio.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gmeiihiff.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkifcalqt.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gwerkjuwe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gcgoukeae.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gpikrvhmw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gpjuasqcp.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gukehawft.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gnuhupohi.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gkzfkdnxy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gbghixbrm.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/glgzxtixb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gaqoqadod.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gtvcouqvy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gnvhgxdbs.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gbqsrwlvi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gosrylsel.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gkkxoedqr.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gkkvcfqkg.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/ghxpjpfuq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gzdptnoqv.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gyxhbqnsw.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/grftrewtv.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gscgudwco.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gljeykary.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gbhpugouj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvmetsyni.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gchwlnxze.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/glzvbpifg.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gaiohyaez.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gfqitpbhq.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gxnugkxth.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gtztwgdak.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/girsptxek.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gpdyetzkq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gynurqiuf.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/ghftixrcj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gbhoxvahf.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gonybbuuv.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gubflkdhd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gtprrpvha.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/guymaahkg.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gbdiepvkq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gzifjbyen.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/grvwsnzge.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/ghvibdesv.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gxkypjgka.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gamvxbghc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gnjautuzf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gabvvzscb.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/ghhorshlu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gejoogknp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gwldayljy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gkmqwbjhf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gqwcgavvy.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/ghnvykoir.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gxloqhzlm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gvjklounz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gnkqnduvu.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gxdtabyil.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gpijpzenk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gueuwqmaa.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/guuqdgdiw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gtdlafcis.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gpxrkaidc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gdaiycart.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gfbewbceu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/guyppflqc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/ghebhmsif.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gqyrvykrl.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gjfhvrrkm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gszemxgns.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gjxrthawe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/geudbkhza.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gnutsipbp.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gcmboysza.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gsmqnncjm.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/ggzbuirni.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gspkfbgeb.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gosnhnbdd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gnnqtrvxd.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/goljqllbq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gzxlvpsmh.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gbrxeptgb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/ghbuaypdy.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gnxlcunac.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gutjweplr.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/glrbmbmjy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gyjyhtcam.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/ggvzngfan.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/giyzdgofv.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gkxpwedlc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gjgeihceq.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gqompwgmb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ggppqpbqz.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/ggpjxouzg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gujqpxhym.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gircdwfmn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gnrfhqaiw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/ghcdrtzto.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gsauvpcay.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gfvrbsjpe.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gkxvcytgl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gdvxfwolt.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/ggbueitft.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gfnnkviod.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gmrqwidrf.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gceevoxas.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gjovfdlic.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gnzxvysmq.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gsblvqkbu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/ghneaidoi.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/ghyssikxt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/grxsdhzwx.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gfbzdnjsw.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gwdrwphif.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gefjqmzra.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gpcemlxdu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gpjobvtpk.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gjbrpzozc.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gddujkynw.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gnhvmvwvm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gumembxbz.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gcejvsghz.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvafnudqx.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gsrlgoczy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gmrxxwihf.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gxfojqcnr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gyoyfyuka.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/glnofzcwt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/glcusjzcw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/glgwklrtc.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gyiuhyjti.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gtyptsqpe.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gmefqehms.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gatirzwyo.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gfahbiuja.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/ghqnvjuks.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gknbjqkrh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gxnckneik.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gaaoofrlv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqdcjxgxn.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gfhkeiogn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcjtuhkwj.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gghsatsml.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/guaxhyzqy.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gkqwzxmri.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gqaqwvsez.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gcmnmcpgf.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvcqxscmo.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gfjrldvlk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gxopeadib.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gdlvqsxsv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gadnujatm.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gzhpdwlhj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/ggvcvjbxr.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/grzyrqjml.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gcqgifokp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/giomfechi.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gsauwjsox.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/ghuisaowy.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/ghposxuup.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gxugnhkvr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsqsswpap.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gmvatnmed.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkcfwttpl.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gqktwauov.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gmtliueha.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gsopsnbga.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gyzkpolwa.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gbxdrjdnt.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gfhjejiav.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gxxbvmjwf.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gckhucoxq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gtziwymrs.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gbgytrfpz.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gewpcaobp.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gdppxrspj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gotehtczh.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gjkgzolxx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gxankvfdh.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gmibglikj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gdjwknotk.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gjvinmsqx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gmmpnouom.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/glybpxwfv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gkpgfxofr.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gkgqelusa.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gtjpczmts.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gukjvkhvc.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gtbfnhkjo.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/ghkaztepb.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gphvxdsjw.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/ggzpwkqun.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gcugybzug.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gtxumwegw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gwacgsvmd.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gybqgxbbp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gutlvbtts.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gtldxhlfd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gcovmwujr.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/glxpwvsen.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/ghvbcsrlv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gwalycprt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gzdwmuewb.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gaybeestc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gtpfnsbjn.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gwtcwtoed.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gmavxuszj.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gcacowzhn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gbtunkeqi.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gmkmxlvix.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gfesbbkbi.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/giifufgkp.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gdqlmxrwv.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gdkpthwbl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gvzmgqpfq.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/geagagyih.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gahemxdna.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gqtyggkup.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gjrsjquyg.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gfciwbxsd.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/guwsugngz.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gvmwrtusu.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gbhssxjzf.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gzeueitxc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gjqcaucwb.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gjgroyzhv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gltfdtznx.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gfxzrharx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/grhabkbxj.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gwnbcysmi.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gqqicglzm.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gftjklake.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gwqbwbbja.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gfkytazhj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gklvqzgzi.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gglwyjhij.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/ghibfumux.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gfhfvlojm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/goipbagla.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gkqoyumjo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gmfyebchp.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gfprvihiw.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gokjhoidn.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gdysikglr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/glantatwz.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gqdhobtbt.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gpqytkdgl.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/geszjkblw.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gyadmhemb.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gatlaecbt.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/ghpepnjvx.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gjssvpymk.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gwwpnxwjg.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gwvanjlfq.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gjpwwapdq.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gwfjdebcw.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gmgbpsrqg.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gnywwoekw.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gxwqruqzk.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gfpsotyaf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/ggryvmert.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gnidyvsof.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzdzekrkd.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/guixmpuzx.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gboibsbij.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gcqxjoniz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gpgkkzjkm.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gbfinizmv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gtxopzpya.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gvllcpsnp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/ggmcqgmll.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gpiwrgidk.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gadnbmbih.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gzapnhdef.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/grslabbrr.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/glxnotgge.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gpateusom.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/glyadegoh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/ghsgdeuyu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ghwuidmgn.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gsuekmlpl.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gvdvnbtqp.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gwphvcpem.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gymvbnoft.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gnsqrrhgs.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/ganwtxbtg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gigurvopc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gatcfvmhm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/giuuvuoqt.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gykixkwrq.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gsvkyrgcm.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gohadpajz.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/ghxajmudm.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gcgxnjkgs.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gmstcbkza.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gcljfsgbh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gjbcvowlq.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/ginxghnxe.sHtML


<!-- 参考信息 -->