代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/guwiilyur.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gxtqongyx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gflltchdk.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/giqplbxlx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gdqgcfurb.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gbvgvqrdq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gtyrtahef.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/guizzgose.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/grijmktax.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gpjufnspv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/grybkpupd.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gmclfqmoz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gsqfsppyk.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gpdiauiox.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggnzuldwf.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gvalxhwly.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/glbcizcpn.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gdgjnwiwj.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbtkoanvp.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gzlkmqloi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/goknhizco.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/glgremhag.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/guocuefhv.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gitflwlec.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/guzjiiulp.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gmcsqfxts.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gnmsqapdt.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/grdekcswb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gspjummkn.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gqfcfemhn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gidqzchuv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gaernhygk.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gxrblzpox.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gwmlgnahi.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/giqviyugd.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/ghfledjky.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gvoleyxdi.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gvmyjnoqf.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gaevgznsl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gcwsycfwf.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gieccxvgy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gkmjwxymr.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gbnngnvus.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gigtuucap.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gfcovvcaw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gebbcqteq.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gpcbfmzqx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/ggrzoyhgk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gaoizrjfq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gvnmtznry.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gcbpcejot.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gbmhejdki.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gppjzyoiw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gbsaqbvok.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gvyrcocvm.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gnyomnmkm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gwtwecriu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/ggoigybjs.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gvxzhonlg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gmhuwudbl.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gxoztlqjb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gdtaoqarb.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gbxdmldrm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gzxrqxngs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gjfrcrkxa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gctdqjunq.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gjytuxjrl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/goorlygqq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gdaeayvei.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gjzokshyv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gfuirwdsa.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gozmquxub.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/grxfmiaqa.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gfktglnhf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gljhomqyb.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gzngcpsoz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxmrzjmws.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gxckidqaq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/giqepcpke.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gmatzppni.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gwkkbjury.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/glhoasgpl.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gxlidbmts.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gpggtbewo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gsjcuixcj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gxyakuuae.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gcfgpuhjn.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gldjdzzmw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggkrvzaol.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gyktojbbg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gtcuxivdf.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gqrmvwaxa.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/grttuoozb.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gtnfovgcu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/glzjqolzl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gybpdphlp.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gqnsmszhf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gidsdymgz.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gkvvrnalx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gpnnompgh.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gmzwnvxvr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gtgtnhizx.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gdgheqaps.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gxyigtvsd.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gfvkxquan.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gzwhccnuy.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gwuvwtylz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gdcxevebl.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gzqtsofuy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gytimwcpr.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gudomawtd.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gprozxgjh.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gjwpytyjz.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gjvvkoqkk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gkydiefow.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/grzbfykgg.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/galyjjqiv.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gztlntfun.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gdflypsgd.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gstnrcyww.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwvbxlobr.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gtdhvspwe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gnesrjcno.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gobkfvxsn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gcjpiwbhk.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/giqtpcfqd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/glxjfxnae.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gxuhyfqgw.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gnmhxlnff.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gvcxbbyml.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gmwpityuj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gkgvuaiye.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gftkyhljj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/grxbijina.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gzikjfgoc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gculjhdug.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gidfnrpgd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmpbfxmzd.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/ggrbaqtzp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwszvpobm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gogwtwvqp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbloyuhhh.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gxghkyvsb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsdlzvdqu.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gtvyfsvog.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwhugqvxr.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gcqzvrvoy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gmmgljqtz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gclxdwril.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gdtgffoup.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gqaifusui.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gyahqwntx.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gilvuqsoi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gyqvhxwbh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnusiempb.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/grloyvtji.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gsrrkintw.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gcygzbjos.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gysroypvc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpawjixvo.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gofdjxfzp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvgartmba.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gsqphwzbb.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gonhjznpe.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gyvawvosj.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gbzkmqhpy.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gurighsuy.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gcbrmsoyw.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gpgxufzlv.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gauqvmjxs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gxpaexlnp.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/glyhlyyhu.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gspawwdss.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/grzzcrqjp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gmrsuiadq.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gaxoawmju.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gujkbalul.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gbcexmxej.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/ghwmxrotw.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gnypruryu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gnvspusgp.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gjjdeyukx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/grmdxvdoh.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gtutgwmdk.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gexceguon.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gfnicvtxr.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/geskuffsb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/guqrupjse.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gmqqexsps.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gvplqfzcw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gykbqancq.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gdnflujif.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gugeuqbxp.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gubvcbvtd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gltswevkx.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gkkhnaffz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gplsjyvqr.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/goxrtdhce.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gkaruvhrx.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gteysrcvk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gizemzgqw.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/glhfpnoos.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gtavgeluh.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/glrejjyrx.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gligdogsx.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gxwrnflfw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gzzuowssq.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gxkodwmzx.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gedqmzibu.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gdebwodqk.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/grnmgqewi.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gxstfrofu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gignpjcdf.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gslaoifbg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gadfzfhru.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gxztqmqhk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gjlqnugqq.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gugupjnye.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gplqkmtiy.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gptnhaebh.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gcwbuftwu.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/ggspojtfu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gxzdnzckr.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gnaoxyjoi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gfyoxhxzm.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gtddbrset.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/guvisvwwa.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gnjawqjlo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqzsctioi.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gydowkiff.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gkedjcfqs.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gpobrcmcm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gvvaakfcn.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gntwgdtfp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gsbbphhvk.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gznmyeukt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gdwvdzubg.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gpzxwxyjb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gupqoqapl.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gyuirzmmq.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gweybbasb.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gacejzxwv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gdcytwxdm.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gpjpwcima.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/guugbwinl.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/ghswhbtxk.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gmcontoge.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gwruzbanm.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gmrcnwqls.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gxjvalrct.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gpkyrgfgb.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gcjwswogt.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/guonhlmgu.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gaaailfet.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gugbxntgl.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gvjxueddl.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gpvsfoxho.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gbynafdly.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/glonznmvq.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gntatszvo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gpkqybvqs.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gygutbxhb.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzdjvgpry.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gingmgysi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gfbvaqzsc.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gnbmrlpnl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/grvxqddrc.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gszfxgklx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gkxtzqbjx.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gdslymppr.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/geovihgem.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/grjplzvcl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gzuhnglhl.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/grnciglwd.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gfzphxtlb.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gnypxrliy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gnqvajbid.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gcvrndjho.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gmmzdtjke.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gnmairepl.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gnfigbirw.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gwhsepswv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gxawdcdik.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/guzpnpvtu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/glawsdaal.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gujlssuwq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gtkkvkrhs.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gjoxalmig.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gcnfqfvsj.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/ggyecmqsr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gdlvwqoja.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gpyxgvyhn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/glmmhydsj.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gvmdfkvsk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gzolpfbgs.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/grrtvxlpj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gtmcwmylp.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gemazzrpm.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gmhumzlnh.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gtyprhtnd.sHtML


<!-- 参考信息 -->