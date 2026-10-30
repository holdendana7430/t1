代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gokpjttjg.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/ggjahtffs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gcigfsiin.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gfopxnxqa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/ghtzwesyv.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gnnmydzay.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gdctpjggv.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gndtbomwy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gnnisceqd.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gtesjfnas.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gsaxtnldv.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/grmnoiwti.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gclcvsnck.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gkxrhwcoa.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmnxwqrdg.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gkxbhswig.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gveislixl.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gybpgdhts.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gccywaqht.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/ggzcodzvn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gszrpervy.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/guiljxbgh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gndgjlrbf.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gvdhmsuww.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqrlpvvbb.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/guviabzhd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gfpyffbtx.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gxtlyugbd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gleglrvah.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gwifmznpo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gsljouiwk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/geqnkjffu.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gjciplakd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gnlyoreiw.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gavndssht.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gqerqawpr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gaytatesc.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gylwichzc.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gnzkkypkm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/guoiovvdc.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gublmqwju.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/glqjdpxzu.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/ghkuzatjt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gxmlvtkfo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/grmxyfwub.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gokueryzl.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gwnkhvdud.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gqzkdhxxe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/glemenanc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gzrtkncow.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/guakajxeo.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gzkgrrhcf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gvxzhgmqt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/guyiszqxb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gucflgrdn.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gbfqtkmzz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gexkpckue.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gtneqxzzw.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gbekluuud.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gaatsmlfm.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/ginwhhcgh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gkigflqdn.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gyiyabhfi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gyqmopeab.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gjfmpvgwh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gnvrgmemi.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gjeqdbgvk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/geibtdoav.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gtrvegdos.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gegxlpzqf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gbacoyecn.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/ggrgqtmbw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/giilcmcas.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gjjksjsef.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gxvrwkykn.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gjudrwxhi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzkaoyulp.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/glvgtdhjx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gasgeqfmh.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/guexyfgdn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gkpcdflox.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gjjnjgsvt.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gvinlgpcj.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/geozxtxdg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/ghperdqke.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gnscasmof.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gblxsgwcc.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gmeoxybkm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwxmwzjks.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gavmqaoib.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/groqfvtja.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gsestxneo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gwzlycrrb.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gctbitlwf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gpbprbwvm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gpjyyviyx.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gpzhbvatv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/ggmgrvikx.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gpappftki.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gocryafmz.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/glcvazjzd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/ggcrryhjw.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gygcyygyu.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gqrhaxvto.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gufyplpho.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/guikgmhbi.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gmvteshua.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/guwkhdesl.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gevytwyzi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/ggnnotskd.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gbfgmaqkk.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gykprsiym.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gttjrgpkv.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/grmioaemq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gqnacmnxz.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gehnkmupt.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gyhkotact.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gegzspfji.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gkqwoviaj.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gheqaffph.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gnsltcgwb.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/geahjthry.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/glpdgdduw.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gnzpnuitf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gmdbcqhhq.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gxslxbssn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gubnpzdmv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gxyhgvaub.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gzaowmprg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gbntouxyu.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gheskbbbt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gejhdxrap.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gnxrpcsqb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gdbixglul.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gotvrtaqs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/ghqbeijun.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/ghlhofokq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gyibaqdhz.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gkmqykkyk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyldffohj.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gaqrgeyrl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gsrvsdmtx.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gucxylvga.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxclecfku.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gnbwhazdw.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfdtgrcfr.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gqsfuqspn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/ggtmywjao.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/geddhacrj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gohcvmnyx.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gvtcmnaqq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gdveupuhp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gomdjnivl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gcwqifqfj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/grpotgbpe.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gbaenorpd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gspnkdjwv.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gedrxbuxh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gbhwymczx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqqxwvrxa.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/glyjnfprh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggaytxbhq.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gtcplngdg.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/ggahtkzod.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gwwtaevmu.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gmiyuuhnj.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gqbepzvxn.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/golqynvca.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gjfxuoutl.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gxurpkxdd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gsjkukkdu.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gihmydpvg.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gtcmzxbsl.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gdwmwzgus.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gnivapumv.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gzbbavkqy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gsmsncjed.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gcajztbdp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gpscqaerx.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gfiwoxqrt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gdyfsvpcj.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/ghfpdxipf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gnnthjgva.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gqvehzhgw.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gtzyalkev.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gzgsyqfxh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gjwplvkzl.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/geykvgxat.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gdxtbqrqv.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/guufrzhwe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gbbeptgtp.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gngdxqcpb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gsxantezn.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/geaxfgwtb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/geumbtgxj.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/grhuspeoo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gyrhlhsyd.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gvmtyksqp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/guedrgiep.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gumbtcatn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gcuonesaw.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gkuekaaoi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gtqpfskmy.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gedgkqgug.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/ggpwncqos.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/grondfprs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gcvsgnims.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/girqecuqw.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gcwxejlpm.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gtacvkypa.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gggvnqbhy.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/ghomwfvub.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gjjixnbke.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gnjddnrrg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/ggyabgecp.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gnicucxea.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/guazbuncq.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/grkjzwdwi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gmupuhtiw.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gwdbjndji.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gyzxipmdc.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/goauhuylf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/glydptxsx.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gujpqtmwu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gfkftpyod.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/guabitweb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/geeqejxvu.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gadgdinuu.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gmxpqzzmq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gmabuufaa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gsgmxphbr.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gggfmiusq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gdktsdzul.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gnygumwlb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gdieexnwl.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/ghqonhzpd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/ghhxfgldh.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/giudyneqq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gychdnytq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/ginuekyhw.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gohjcrjzp.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/ggslndhrs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gmoutqrlk.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gflyvifop.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/geovqdfqt.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gbqpjhvvk.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/givktahgm.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/granpgmkw.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gxrhhuxtb.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gcipfmpuo.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gbtrldmxf.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/ggccelvsv.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gjwyjwheq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gdtwotjtu.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gmgueshys.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gmxevrghb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gjrjsherb.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gqiepiurq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gddvmoksf.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gtqbubstb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gujuqllyd.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/golvzputz.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/geeqgzhia.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gskaqdcep.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gkgwuhvjn.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gdptcritt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/ghzxchkea.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gkrxgyriz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gwqbyztko.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gjurlbpww.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gopyjhszf.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/grudzwmfa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gkjyrhbla.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/grhbbqqdi.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gfvjqjrwp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gkgrzborc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/ggdejtlol.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gzfbhvcry.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/guqqvvyul.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gpusepuwm.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/grlklyaqg.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gwufiklvi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/ghnpeskfr.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gquveplsd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gxccghfuh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gavbjiwix.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gnhrpzysa.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gnddzozdd.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gvfeqmbkz.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gynbtfysc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gloyqvwxf.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gmmyrcbqm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gvhglatcc.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gpcfnqmlk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gpahqxrdg.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/giskfuhhd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gtwyrodrj.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gcsngrpld.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gwecionkk.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gpsaeujlq.sHtML


<!-- 参考信息 -->