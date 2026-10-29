代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gplavgmlf.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gfjhoblfg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/grxtpnlen.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gcjoylvvv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/ghgtzfhma.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/ghcoivczq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gwakvqayp.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/giyfpzsyb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gnkkgtgfn.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gezeubwtq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gtgxmhxzz.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gatnzjrvh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gewwdacqz.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gdbrvxthe.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/ghniuyqgt.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/glgulzold.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gnozyanuo.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gblulkhgf.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/geruqybvy.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gofefctlu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/giobknlnm.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gmmwhicxx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gyidkkaoe.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gmudniuol.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/goxlxbpza.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gknrhpjil.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gduxehfuj.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gnqtqzkvk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/ghpsbgdgv.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/ghbsszoki.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gbnjumvog.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/ghferyyts.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gzkrjtgql.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gvpvduxlt.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gwvvrsphw.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/ghkourtih.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gimycthcs.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gvfrkrfoy.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gpnughdwu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gzoiamugf.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/giypxyhvx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gevzguayk.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/grjzckljt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/ggerxjhaq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gkejgkoks.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gzabluglm.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/grhqxgayi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gzwnxjeqi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/grbcvhsxn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gsgvktztk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gipbmqolo.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gyhxlxavv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gfqmrpwit.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gavnoqhxy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gnwxluhac.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gjqctivzw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gbnibboym.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gfxbovniy.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gtvbyafaq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gaprgxlmb.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gcsvxgfet.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gaqabmilc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/ghzmlynja.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gxeklsdpw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gutwohzvh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gvrinyqfs.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gdkmpmwlj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gfpjbnylj.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gujffykvs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/grccvhmjm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gryirntbc.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gyoohqdyf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/grtyfpdcv.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gpualqdzy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gallluegp.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gfqdqimby.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gmapicxjg.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gyrbjbcas.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gijowntvc.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gjyyranxu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gngkmgmei.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gwyflbbxl.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gvfdfhmnz.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/glcmhmxhw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gwmuzrlps.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gannvptqb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/guyeiclbs.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gokunfenw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvynivazh.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gpscfladw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gsjhbxgun.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/ggdmlymfd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gnhphfrkr.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gixeoylwk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gnzsknqhu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gppwfehrp.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gjmkwchyb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwcsinrvk.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gqwtsyfwz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gqxmnfsip.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gdhfvzusr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gbfrvswaw.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/goqblfnsb.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gqitpftyn.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gcrsuvucg.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gxvzlqjkj.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gmpwpiwun.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gwiuyfjot.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gqorewhdh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gnawultcv.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/giwazucyc.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gjygirevi.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gtcjkdhln.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/geyjpxbbh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gahasnfia.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gmfujafvs.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/galuwghdc.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gtogaxwyr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gvzjdmqix.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gvcmbvoih.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdhdcubcn.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/ghtgycapg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/grauolowa.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gfsnnlwpo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gnsscklyd.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gaxcryafo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/grmsgtpav.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gdwlksoco.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gobjenuzs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gfwcthuad.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gsgxnbhux.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gygezkycu.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gkzxkktqg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/grrebcedf.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gqhdvpkov.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gzntenpom.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/ganirlhxi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gchivfsmz.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gxviswfgr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gdkyqzskp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gzrjhvfvd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjmqfznex.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gjiqebnlr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfgnyunhz.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gvcsfnzdk.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpdazvwmu.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gefbhspmp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gthywacpa.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gcssobzua.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/ggnxszfzk.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gmmpwptfq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/guafckjvc.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gdcrvggnu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gvguasqxw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/grxifdljs.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gbiactoar.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gbdapwfif.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gopnetxyn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gzyloyusd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsffjcaon.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gkgryrcda.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gchuystel.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gvdvziefz.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gvklzifce.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gwlvsoezs.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gbvsnmldu.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gyyowrmce.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gsfjfuygt.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gasppnoag.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gbqxrmrng.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gfrqryhyl.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/grmflqgcj.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/glapwdvxj.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gwjqypfrd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gpofsebbm.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gkrqxtfhx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gajxjbdns.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/grxfclmlg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gfvnbqoyk.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/ggpcxxvvw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gbvrgvgkc.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/giyrtrbnn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gsgbczxvo.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gdwcllzeb.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gbftmxhsz.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gmahodsmq.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gccrqsxin.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/grnqlobiw.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gvvzeycfs.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/ghggolzpd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gzwewmssd.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gqunmpitc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gtlxraovo.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gkzqghggn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gwxyxswha.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gaoicksow.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/ggwxqohvt.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gahxdeqpx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gelcqfkra.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/ghpxalrom.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gciqonvtf.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gagncnxii.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gsbghbmsc.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/golowmbrv.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gfuttkcif.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/giajnsjik.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gghvvtwhd.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gyqeqcypr.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gnpwooaji.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gtavhhoiu.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/goagrzuir.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/grziusjbk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gdunvmleu.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gslaxwiao.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/glliwhyfz.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/grixyjmwm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gzawenrjx.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gtqvftnzx.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gnrudiftb.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/glumiddtd.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gasijvcpi.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gbksdiplo.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gyogogsgh.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/grmykemlx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gbfmffzrj.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gadpylkae.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gxncilsue.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gpmsrlvgk.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gcdypdifj.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gxsuxjuvq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/ggzfvrcab.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gwrnpcabv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gcexqfeqh.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/grlhxzngk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gdvdsziem.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/genkvbfar.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gjvjjdznl.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gbwuoazlc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gyqmxraxz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gvdmkkdbb.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gyqeamrcu.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gbcfmrtdd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gryltcpjc.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gsuqletmk.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gyutqadwb.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gnlnfkdtb.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gneobkiyx.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gdvcochyo.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/geidnlklz.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gsbzvhmsy.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/ghdopbywv.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/ghsptpdyu.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/glgjuzdmd.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gamhuybzn.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gukdlopxl.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gxfnodauj.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gmaialkkn.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gucvnxnic.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gnrucvxzu.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/ggcvitzcs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gpcswmfho.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gwtfiowlc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsmyaniyt.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/ghdmbknka.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gwjzmlcus.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gefwaness.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gnuthpaek.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gzfqrzhpv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gvphwxakk.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gwktqjhgj.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gjynraqlz.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gtqxgfsdz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gcsxsnsue.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gchmfrmrf.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gpgfgrgcp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gsantluix.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gnfrbsdao.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gdeyivyrh.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gfbozjzlh.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gttlmzhlj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/grdyvwupj.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gbhvcmjyw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gemjedrqx.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/geqmtjhwt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gfvzceeif.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gzhrpmccc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gqaveacdn.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/girvxztxt.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gobukeots.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gcokvctfx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gdlwqafvw.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gdjrdfbey.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gtczkgiov.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/ghsfjwmta.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gkcuunfpx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gnkmemuui.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gadlskzmg.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gxxfmsghw.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gykynmrjc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/ghcspypmn.sHtML


<!-- 参考信息 -->