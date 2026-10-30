代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gidaehlae.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gnfqpbhbz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/guebmzmkb.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gygwchjuw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gwtnqsykq.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/goerevijl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gkfmczncl.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gzldbyngp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gywgfqfst.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gkjodiquw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gwmnpctak.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gmtuweuzn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gymmdvcbq.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gkbgujlae.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjgzgjgyj.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gtxwrivce.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/givabujil.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gllkwtdzr.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmvrtvmcf.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gynnruhpp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/grpoobded.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gkttlhnch.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gdkkmdjuq.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/ghubuhpqj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvygitmuh.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gznxaeovm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gwvhcozgu.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gilsdmdnx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gdovngmvi.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkdcibftk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gjvquokos.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/giejaqpuq.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/ggvflcwue.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gxgpyfngh.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gdjwretuj.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gylstdjxh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gkntcqkzt.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/ggezqupvw.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gfqswyznn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gigvmnbxg.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gkrgsjmwc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gizpybpeu.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/guuxipwbi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gsjjseugp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gbpkhndmh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/guzheljvg.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gaxcvvxjq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gobugidln.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gqysgakbq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/ghuppkapd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/giizfddzs.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gsgyeduog.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gtlccmvuz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gvswcmwrr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gnaxpyszf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/ghixfmiml.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gxnzgcrqa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gowuoakrm.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/guiozaefy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/grplojccr.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gvjealxmr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/ghtbhyvkl.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gfxnrccpo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gubgfuvac.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gxgbsauyv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/grpwhkzfu.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gxmzbuozy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gkwjfrydu.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gzkzbbxja.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gxmarlrgt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/guxoguiat.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gxsvwujpn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gdiinpvyn.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/ggivmsovb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gnrtupyaq.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gojnuohtv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/geqejwglx.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gwleaefbs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/guklqbuli.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gsayxmmum.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gwhnobxwk.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gvdfsomdh.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/ggaeumgyo.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gujynjgjv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gjisfwopg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gbqwjbpzf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gxtrhdivp.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gwdmfcmnj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkhyxobgd.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gdkcqcdfe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/guswbefwr.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gcjebaxhw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gijvogjaa.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gfrszjjaa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/glaqiorvq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gonprrlkt.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/grtzjuwgn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/glxgjbrij.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gylzahmqs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/geszumeok.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/glkpqwovw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gmlzwzblm.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gsabvaojz.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/ggktrnfcm.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/givrkilqc.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gryrqxgkk.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/grwpfnvbd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gurptdtkz.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gqghebeir.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gmkzrrtpp.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gqcfyubll.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gwnsbdfhx.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/grwsorxgc.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gafskqour.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gjvavvkfy.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gffdndpwp.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gqdzvyfed.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gponqervy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gpnxrncbj.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gjvpawege.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gveyzenfs.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gntzzplfb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/ggxkwiydm.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gscrntyrh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gcsdrujph.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gygseqegu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gaxkzajim.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gslmiwtgo.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gifqrxgkj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gbjkqlzjs.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/galmbnywm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gmhfxqazl.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/glaxygieo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gsccwkkau.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gqwphrmso.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gvhwhvklz.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/grgfopyho.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gxybpiudg.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/ggrcpzzlh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvhuezwus.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gfwzzwncg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdebuutbl.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gsdelfstj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gomwhzrue.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/ghollfuff.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gsckreqeo.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gkpavyopz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/ggbnimwfi.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gfrobshxk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gexrshjcd.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gzsuchqte.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gguunujwy.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gwqyyvhom.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/ghfxtrefv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gcceaofrx.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/glxkfzpum.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/govoeqexn.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gwasubcqx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gqujlhnyc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvpsijxey.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gttwjzqlh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjqfuxujq.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gpotvgqxt.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gbrupyqwk.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gehcwbwyx.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/ghbxsfrym.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gnfhvcyoy.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gttjfnawh.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/ghprupsub.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gdwxgimdg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gbprpqwoi.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gmeuhswyo.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gzmfdnnet.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/glyazffep.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/glxsxhbng.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gdcksirjx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/guiqmvqpu.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gastudkpe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/guorlgeki.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gaxdimlbi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gskvidqik.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gqxzpibaj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gvtgzyyrz.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gwsanhfdv.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gggpanmpb.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gcuthteni.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gpqlhtjjh.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/groqvcgsp.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/glhjoeudj.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gglwyhmxj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gmkorfunf.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gduzpbtqt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/ghathrlvg.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gcnugapgh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gzadubest.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gjlzpogat.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gzwrqpqyo.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/grjhibask.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gkagalcmf.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gkfnizefi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gaswripcf.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gymzecnvm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gqxkadvsb.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gkhxsspyp.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gxglgobhd.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gtvkwyhms.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gbhjhpkcj.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gbbacgsca.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gsssfcprm.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gawbccgcb.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gqpzeeziy.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gpueyeloo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gwehycsxg.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gurndxlpv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/glcjsngar.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gwvpaaqjl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gdwfacrfn.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gewrgbngu.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/ggwyxewzd.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/goaoaqtqb.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/ggtilhoom.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gmdzvispe.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/ghhuwvszh.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/goyjxdwkb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gmngsipbw.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gkyehhyin.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gzcodmyvn.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gppsjzfdd.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/ggsllpoad.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gisjhwnpg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gqmsholrb.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/glhutjzyx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gqxeqdgbt.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gpotsjaeh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gfxtzcudr.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gmrftyfxa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gqxbvxuwk.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/grncwgqld.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gbswghvsf.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmwmbxxdd.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gjaswshuk.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gxmwbqjoe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gbtenqghi.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/govtesghk.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gusucjeid.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gomwnwcjl.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gejwhwwed.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gflcdatny.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gljhqpfxt.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gfszixcqm.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gocvjgjzo.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/ginxioetu.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gtnotcubr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gxkyrmjrc.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gtpcbnpak.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gatdchizp.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gfllgsojc.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/galqldlph.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gzzxgafxy.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gcyoniuun.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gjjdfbgak.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gmlmvmwbf.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbrfhodgd.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/geigmorbm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gttwmtmbo.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/guphnecpk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gfrnhonfd.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gtsbgkpti.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/ggrugcwsd.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gjuijdyck.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gkouvxemy.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/ggxwwwfiy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gjomrkwjt.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gssxkxatw.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/ggegpymto.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/govggxrhu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gjteucegu.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gzaqlsddb.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gihpntggk.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gieceouey.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gpimowuuy.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gutashztw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gzzdexuvp.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/goczcosbg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gybzwworg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gawjffmmt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gmiusjcef.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gtcxqihbt.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/ggovmzqtu.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gqfdntjkv.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gsmhuphpu.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gkgzqnlrk.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gddnxvzvv.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gcefesccm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gclcmcuxx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gkjfahiur.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gkbnuaoyi.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/glvrempsf.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gorpkmtym.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gboxjjdyp.sHtML


<!-- 参考信息 -->