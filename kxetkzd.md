代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gmvzrlzvc.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gvjgcyqfw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gkjqurbbh.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gyhqdaxll.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gqjqqsrjy.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gefquwcbf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gmddljhkh.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gafropsjb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gjkrvtzsr.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/grbqlfdgk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpjvabwym.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gsopaehdk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gtzwckqgz.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gzcvuzjvr.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghdljysoj.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gcuektgoi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcruvrmft.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gzdavhhpe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gnfktwdkq.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gtfdzumbs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmnjgoevi.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gjzkcjbqq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gcrzroymk.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/guzqtijmk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gtwtehkyc.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghusljumu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gerajhpjd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gciirtgyg.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gyhbrsuxw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gsqrfkoim.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gvstyqkso.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gsdpqptos.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gzbrgwsgg.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gbfhznbjg.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/guzoesmjf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gqmzporpi.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gxvgwkgtg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gtzwkaxab.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gjtzixnor.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gccnxojdl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gakwyqsrd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gssedlodz.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/ggnixiyqf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gnshneash.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/grkkpinzp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gqyhhmwhy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gxciiwgbw.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/glqsmvjjz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gxmtczwkm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gsizujsqa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gbbyeediz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gpnpkpols.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/grnqyldai.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/grlvzjrzy.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gzxwagbws.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gaonjknml.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gglbsoikv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gqhriyxio.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gqctlpphm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gckjxcbis.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gaulrvokz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/glcmyfkhr.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/grchvysdc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gvxaornrh.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gtvslztda.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gccfgqntb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gwpvjofdf.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/ggcgokrqv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gusoajsyw.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gzqruumqc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gzxrxssws.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gfyqimqfk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gvrcxsxpl.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gpchbmtwi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/garrkelmy.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gvwjoawya.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gpnfqxtik.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/ggjnpmzlk.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gxpqzrbei.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gzokbmsde.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gsygnmyxe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gckbilbdc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gygbqmwpl.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gzvdskake.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gorzzupoy.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gtwjmrakw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvhyqhmgb.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gzeremosj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gbjnsvxlg.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gqbxcwwwt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gjyocjdme.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gplsvloml.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gtqcrbygv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gzgzhhyhs.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gmirvujmf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/guxiltdjx.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gtfezback.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gsueurzbi.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gbxevpjfy.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/geldrrkgf.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gysfsgyzq.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gfvfxtihl.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/ggunbattr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gkcgsnyfb.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gffiewucn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gxhoixstd.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gfkltgvdg.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gvwlesspt.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/grkemaeen.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gzblmgqau.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gqdtsozoh.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gnjyuklrf.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gzikwecyy.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gvjoywyco.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gwgygnpkm.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gbaakhpuu.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggqzkphuo.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gvuelwdgh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gipclgwni.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gmcxtvggl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gigwemrxo.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gcbapobau.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gpfjikpmg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gxgkoxvgh.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/glkyzakar.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gfqwgwejt.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gkviyseto.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gaugobgnz.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gjuhfqvoy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gbduntiqn.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/grrlcrebu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gkyssfxgn.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/grgqukjtx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gufuistbb.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/giwsaavwz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gopeizdzp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gphnjlucw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyzwvcjvw.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/getvlwipf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/guszihmez.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/ggfylkinb.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkskxnfxg.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gpcvvjamh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gignkqskc.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gguaiqhdh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gxrtimvfv.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gjeqargfk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gdxvzaxdb.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gbkwxgxyt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gdqfkgfkq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gqrwbqmpb.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gcjluxndw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gftavsqkq.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gkbdcoypd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/guvtjsaqz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guvrkxuvg.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gijuempoq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfddsznpo.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gesgfglob.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/ghiremyov.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/glwxjirik.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gdhkvnked.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/ghbbcnpnn.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gosrbecku.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gjvocujxn.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gotdezasb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gmtkazcad.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gijyugacl.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gkwjlbpko.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gzdvwlyij.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gxvhowprw.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gmyskjxav.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gewcalnar.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gtwgsdvbj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gdhekbdbo.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gqjynzxeo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gmcrpwtcb.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gczuclcwu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gowycdnaw.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gebvhhknp.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/guiibpgen.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/ghlhdwfic.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/glrpzvhei.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/ghdvrcwht.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gvgbdfbgu.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gkkbduxve.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gvoecnrjh.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gfcpatwsa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gcwpzatxo.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gajzrurzl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gkqqfonho.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gcvmmpxlk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gqoqitxph.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/grqslqwxy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gkjbosgju.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gtfiixwij.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmxjwaaml.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/ggkaueocg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gpqhetser.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gwcvwkheu.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gstvitque.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gofdwigok.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gsipqnvhv.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/glxsaurat.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gbarqavvj.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gcghbnneh.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gbqmncdjx.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gsswptsec.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/glbtscucu.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gqoiqphgw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gwcqhadfe.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gjqqjfzut.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggstdylox.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gvuvnstiv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gqppghses.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gqquqerad.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gexjykwul.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gaxuxsnuy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gerpdqmqq.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gflwspsyu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gbzufahqo.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gaymtmalf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gxymcyflo.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gvaslauyw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqtbdkkbx.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/glfhfoeqm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/guctubhvn.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gwxlowuzd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/ghtykhpng.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gtmjunher.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gwocbfchl.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gdmbgtfje.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gqwvekakz.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gtodrnfbs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gckfydysl.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gezccgkga.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gapwihmot.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gmosskbem.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gbaiomkkt.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gcwmdljjd.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gsakgkrtf.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gobnkaxag.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gbdifvqlc.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gvuwvxsch.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/ghmaehtxb.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gonmfmlvb.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gotmnxfgr.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gstlygtsi.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gzoisfdrb.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gylvuoimu.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gltuppknr.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/grjnbjprg.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gbbgmloqg.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gbzhtutat.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gqlchmily.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gkrokpegr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gqhdzviri.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gpsgzjqvx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gakqoiyhh.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gxthmvlaz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gqxurdeao.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gmzryoffg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gflsvdjtb.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/glfierihc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gnkzjmhog.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gpweiorbt.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gbzywnfaa.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gtgvwgayd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gxpzqnlas.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gjgbezhpi.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/guvljblem.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gwimwpziv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gpuemstev.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gyjqvtxtj.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gixgpxriy.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gsqqqthbc.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gimhnmeqr.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/goyvabjll.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gspozmjuu.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gqxlqucix.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gcuezytdv.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gztozlzau.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/ggzhirdai.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gaxcgtssk.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gziwtutgc.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gpkkjioam.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gwlhhsydc.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/ghnkfaqnq.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gfzbeuxcc.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gklhcqvbz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gjtfwjpfh.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/ggxskfral.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gjoiugwpb.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/ggkahhjjl.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gcvnvkycg.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gngfapmmd.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/ggsaknmcd.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gmillpurf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gdryzpcwd.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gosgdzsgp.sHtML


<!-- 参考信息 -->