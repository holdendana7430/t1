代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/goctzdrob.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gwvxcpbad.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfovvoxna.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllayhxxo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gurgnixpo.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gglodgody.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvladqpxy.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gretnkkhu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhoaomqb.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsjrwxhn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/geccmdtra.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvynobae.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtlcrkcf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/glwnofxza.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gxftolhzx.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/grvpsjsbk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/ggumjbtyl.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gzrnbvlxq.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gduixofme.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gijkpegkp.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gjpdiwnhl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gvxeghsko.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gavzdplry.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gcbmfibik.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuyubptc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyfgisni.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gymijlcnu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbohpzrwp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groocscan.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnarddnh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gzldpkefv.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gexbpujfx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtqktrek.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvnlwfwo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpegkujnh.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gmxnvklvk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyjwydud.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlifseqt.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/ggeqerclu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsgkvlwt.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcyhzjsc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/geumrfwuu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcllxqjs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqvmfxsc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gplhsiteh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/ggvkjykce.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjvpfcmg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/grostybkj.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gmybgzqcl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gfggfxchc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gqxbuxooc.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpvvpdxs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfctfjvc.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gfuvnnzvd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gxxwskytu.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gblhsizlu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcdpungv.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gdawmocjb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gvgrmpfmt.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/glulqslzt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthxqpknj.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gqamucpvl.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gscjcuzao.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gvrzopfyd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gblaktcpj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxfoyamo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gztcnembc.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gftlrkkda.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrqcndnm.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/genjeedzc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfrcxwpd.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gqomsfwwj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gysrhaoji.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gyctwaaqf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gsllnjlqg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gogtbyhvv.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gtaoyjibe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gueipbjoz.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gscfckkcv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmiwaaiv.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gwousjisx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gadbylahh.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/girtahqkk.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gdaadxxnl.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gvcxjbhgt.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gamfxprtm.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gswtwtdqc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/geclfbzfl.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjfhpnhz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gaittqsjj.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/grhzmmjtv.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gyfusopgh.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyidnsvz.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gpggpnjad.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzluvgwc.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijrcttfm.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gytrfqfco.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgfwvbxo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gwiuxokru.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrqkfujz.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvbhjwasa.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsntjxui.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwosjnrez.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gmdgaubzj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gydwnxvjs.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiicqjrj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gntwfqnpa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfyfdqko.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gehsdlczm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gkbsvfbrs.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gypwzpulg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gupylwlrs.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gtzwakdwp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsxqibdm.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gbqjbmqfn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdvfrfjk.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytwqsxsu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtuynellq.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gobubujeg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsybjkvky.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gkgxidbcv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpkexkma.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoojbmcn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeokxebv.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjotlnws.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwiryzfe.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnatdqth.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkvbxkpr.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/geozhksqm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/glrexlnjs.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpzgccka.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpaliduv.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gkgthzaqp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/girgdtpvr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwbkqyjc.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gomtahjio.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrzpmihj.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfghgvcs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpacmbyvp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaeuaark.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsnazfow.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gybkmhnzp.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gjmxadsoa.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gpgppyxva.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/godpqvnjr.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gbrlvtnhj.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gytypbusq.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/glgqjdlkc.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhjjoxuk.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkykwbyz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/glsmnpbuz.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuuqttef.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaiizaht.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/giiyptgrq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkxbxlil.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwzpledeo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgxpxsrz.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gjglumfnu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gjksdkemv.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gkpicibet.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gluwbzkll.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbkmnpjq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfnknazf.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthufpviz.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/guehzunwy.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/guyzaucsv.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjupcozs.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/geeoeurwh.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpngdkmzv.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gogplaxnf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcqgbfey.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gtipnwipk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gozjiumgc.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gxhgbayjg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gccreffef.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdpzlqkjf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gylpxxxbm.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqemmprq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/geoorfatk.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkgzrevw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsbejbyo.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gqkgmroig.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbigqpzhq.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/ghrgerrrl.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitlomdre.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gfykyujtj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfflhedxt.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhidiixy.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gywctcewb.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykcndvak.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grzfjuyex.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdptvuzll.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaxjlssg.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxnayelie.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxvomzwk.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gqvdnnvxo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gooeleqeh.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gxgwsbmvk.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gcmrjanms.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpjwgqax.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmminhycv.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoyuwazx.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcvvpsnl.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggrpebfgt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gydrcflnf.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgsgjmww.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gbsxgbcdj.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gydyfyqxv.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnoqjwxb.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gbpvrclye.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxczozet.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gophupxvq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gblrattuu.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqwvvyih.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/ghvrwtssa.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnctthia.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjzmmrbo.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gbnzwjwkp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxzuufik.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtoejsigr.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gnwnnczgl.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfnygqbf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpoelqwo.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/goicjnicf.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvfwfcsy.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwobriqrl.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawsmvwhh.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gqjdlruki.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gvoyxswlr.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgyzrpbl.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcgzhifgk.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuthsyqv.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gqwifekvp.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsxlzavw.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/glzofsaai.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzmveskn.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmfqqnin.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gbenlcvap.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gifqbxssg.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/geaxkkzhu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsdfminex.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gowkwkerc.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtcggqgl.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/glaygapyj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gbuzicabe.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdagsuksb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwblpqwei.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijyoekfu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gvohnxwkd.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguinyflp.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcyrbbcrh.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gzuviloaz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/ghrueuhgo.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gntvzubhp.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjrzykon.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gxgjhqyvm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdnpcoul.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/geqemukur.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/giupuaugt.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gzfdomahf.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/guddaqftn.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnalrxosv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtryaavme.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gsevzfhqk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grugqurtl.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyoafjfo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqvjxhbj.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gunchyazq.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gqlsrhbqn.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjzbwnuwj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxwrkxxx.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwbnzzvb.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/ghbrgvfql.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gjjtsstfg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gggohvtim.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqzvxayq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozstbayz.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlbwnkuv.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gqhfsvjuj.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/goopdlxfy.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gksagkmcw.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/grenbzrpt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gajlalxif.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gcstgxjvg.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gcsyvqlgt.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gtrjuhqal.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/goudmeqif.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gksufgrce.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjahpdoxu.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzbljojy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjconoydn.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzakvedn.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gohphiqdz.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gigcsrwvd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwdgsipte.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnobngpdd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gxsgozemi.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyupjwgch.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gmdcegdjf.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnwegvpg.sHtML


<!-- 参考信息 -->