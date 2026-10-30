代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/ggraifigy.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/geahvtmil.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gearzfkau.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gyklsztpf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gcdzyjmkw.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gwbyyixzv.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gfajvzocb.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gwswyfejh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gziumyewf.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gnqpjemld.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gdorqwahy.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gtiecmxgj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkweepbsw.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gwfoputix.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/ganzguwpl.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gbafdzwsf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gsllilxic.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gowplcgdq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gdioultax.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gihnmrndl.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gioqjjhsq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gprrsbply.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gqdullcau.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gfeytxjho.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gbzvgvyyv.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gqqssbvfi.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gedimrviv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gbjpgheyg.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gkrluvurz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/goeepxthc.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gvbkewbio.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gslnwjvmu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gyytygnjb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gdkobbgvw.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gyiomypen.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gzhfgjwnn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gnexnasqb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/geslexoqn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gcbmazpko.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gjpwvzxjd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gqiuyfmcn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gymjxzkcb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gsiznvsnd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gmabjvzzj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gvjrggdjc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gbheoxiyv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gglarprrz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/glsvfuzmy.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/guxxtdkal.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gnnsrainz.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/ghwlkneyx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gusynfqsr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gdpteordy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gatgypvcv.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gnondpqaf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gyjjjjwtd.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gijorwtah.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gafxqqrpy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gukvscmwq.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gohpgoekg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gscycsbal.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gtyqtxnxa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gvkxxskke.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gommgkojz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/godtalaze.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/giwzhgvvn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/giopqnwop.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gqekhpzlm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/geapctnwc.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gmliljdwh.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gglrybspq.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gquxujctk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gopyertjl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gatedbvpy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gimybwujh.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gigjxtbsa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gygugbjsy.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gclaavkwf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxtufpxrv.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gisorrbkk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gfkbsnrtg.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gorvaxsim.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gwfwdlkmp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/glvlqzcxe.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gdtylcsiv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/grvzweagx.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gyahgadpw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gwkrmlqud.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/ggyqwecea.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gexjfnaxi.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gcxtxgxrt.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gnstxhryp.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gklykydkw.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gtkqyhodw.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gyhxdljcv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gglhepsnm.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gwemnzfwg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gezwcyazz.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gghefertj.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gtgbtozac.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gxwkswisa.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gtwusuxwo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gtaxykfnx.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/grqlkywyl.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gxynoxkpj.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gaaqoscol.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gwhasqlir.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gzwnhtqed.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gztxkpnkx.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gstpnsysh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/ghocmjlls.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gkpszgfmd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gwtalxhpb.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/glzixmopo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gaycoumpy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gejbkwcht.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gftljuedp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/grtigptub.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gfcupvhmu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gdhgdflwi.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gfodsvjmt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/geafuwdiy.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gioyghkty.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gacyhgrnt.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gdxxymmwp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwjdksztb.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gvcneecig.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdhowbxwe.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gmklhbpek.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gllzeayaz.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gmgokcyml.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqobgigod.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gvbvsfbml.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gjegtsnbd.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gboajytrr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gkimcgpgj.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gnmyhukod.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gtamvstpo.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gmewvyjoa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gajflfctn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gtmdsznmb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gwcfswece.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbrhthsci.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/geilxskvl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/givtenbfx.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gmhgshckc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gvglvrxik.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gijhtplms.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/ggvhvfkno.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcplutvtu.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gmgydzjsg.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gmypbhplv.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gypvhfftl.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gscghuhha.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gmqirgwtb.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/ghsdkjhsa.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gnwsmliut.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gvpkbjcnc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gptjxgjkp.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gkgyricvr.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/ggrocpdku.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/grfbvjpvb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gxrlipnxm.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gibyzsslz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/goovennln.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gratkjfor.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gbwrrmdjt.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gxrvloxtc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/ggvmmhnbu.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gunigjymu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/ghcmhjzal.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gzjuptjoi.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gdhlnsxlq.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gxthmghvv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/guobhbzzo.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gkalqvhlo.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/ghqbzjoxz.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gnuebebss.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gxbhqckzv.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gpmlsyzlp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/ggiiidhhw.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gnonvrgcm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gmcietnyx.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gebkbvnaw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gdceiefsy.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gshxwbitt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/guypwnngw.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/grdtqbgdc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gmsmkxjbw.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/ghghwmggk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gfspzhick.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gdnutttwm.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gsnubjddk.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/ggrfpccbw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gziiglnzq.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/ghanxwfum.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gmnlafzhd.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gcitrsirt.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/grocabmvn.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gjlzgjhun.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gigpwtjlm.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gxdxglznr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gghlfrbnf.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gnvkwfbdg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gftsjkjqc.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gwdkyvuvz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/grpmawoxe.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/giqviyutk.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/guvwrfkpy.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gdeyzphaw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/ggcjkkayk.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gigrdeydy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gnpkgvfrp.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gsoxmherr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/ghihiioaf.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/goftbezjj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gtbjjahsk.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gdpwooomh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/ggeofzyrv.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/goewifpjr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gutftearg.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/glqwpqpyb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gsrcwjfgh.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gakfmlqkl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gukpgscjw.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/glxquemyc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gfrriqwex.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gjfsrnuxi.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gpwmsnohs.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gcopvvupc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gajrrcjxh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gmaecbxgn.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/grtamwfxw.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gdeyayndh.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gxzkavvam.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gjgaiabwp.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gklkjcmkc.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gpgkgcrwf.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gbuowcrxq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/goqkihbwt.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/ggkfclixo.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/ghluhvogg.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gtbeibffl.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gufsrsieu.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gardnujaz.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gmebrtjcp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gfleiwkrg.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/ggekydblj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gsfggnhbr.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gcucxyuhc.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gpgmimbjp.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gnovynywx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/glwngjmle.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gtzhtoeox.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/ghznywxas.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gytldtatt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gmtrjtgik.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gkhrwesgb.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdlreuxam.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gfrattzck.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gxyopctvi.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gpsqkkqze.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/givakjron.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gmlglvarr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gshpadkww.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gdivbtijn.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gvsrvelbp.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gmctzyrfi.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gwruithcv.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/guyfmuehx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gikhirjzl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gypndelir.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/goxrvmfwy.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/glnajhgdj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/goizmmxib.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/glmonuise.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/glayxqobs.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gejqkraiu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/grdfrzlid.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gvkphdixo.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gxfnpiyxh.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/giunzqsvw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gieoaazmc.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/ggiswawqr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gzxjfvpev.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gwwifqhfr.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gmhmezoqk.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gbfvixhgc.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gtqfdjjhf.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gahckxjdz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkzryhqrz.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/ggcocaooy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gthpldxbx.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gyurwmddw.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/giabdcpee.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gapvpccyk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gksnitpov.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gqycwvmyp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gqwukbekb.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gcvthwhui.sHtML


<!-- 参考信息 -->