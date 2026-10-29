代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gudrgkfxa.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gclwsvqhz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gkqgejjbs.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/giyrzjnfc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gmjgksubo.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/giwnybtib.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gfnncjthw.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gvhfqgrxc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gikdsghoq.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gcnpuqxzc.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbdlzwlbz.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gjegrieoi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gsehbvckl.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/guoudoptl.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gzcsrwqbh.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/guspiwgpq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/glzlhwfag.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gzjkaurnq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gotpbfhuz.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gzeslaesb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggislkrsg.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gsembnuqp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gflcmffit.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gjsewrrbe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gbyvpymys.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gbnllcngd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gxyitgcvr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gjkwptvql.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gmqiztrvo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gwehkesmr.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gsqffhtib.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gfhibzqwl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gjiugfcix.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gsevqwaor.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/geqlaiybu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/ggxrqaxcc.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gxzcssvzk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/ggddxxebx.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gtpaetazr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gswcgovot.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gtzxcdstr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gnflvofti.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gpgwjyrot.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gbrtluqxq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gygdehyrx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gtodefdua.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/goienewoz.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gkoxecxoh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gxpwinddk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gmilcfodb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gcmtudgkx.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gzhtiiynj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gdhoxrjsr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gcqytigut.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/grlbspjcs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gbpoeenfl.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gyghkpbgq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gqhpsbuyg.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gjtudamwn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/geawkphji.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gvqikkiom.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gwbzwxrbv.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gqtpyuwoh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gzrfthpcy.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/ghfnfisxk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/ggeyazwxq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gfmgmjrei.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gizqveqhp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gtrilfcee.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gbtjawkkk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gizmkxsbg.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gfxkujwbz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gsalnrvty.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gasajnlnc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/grrutovky.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/geczzbshh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gsfpsumks.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gymamskff.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gompftpux.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gjwyjidvb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/glzaelkla.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/geflfozmt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/glaxubxem.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gxeibuerg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvpiuxszm.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gzpostzoa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gnxzwucrs.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gcsrjscmb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmvhkoayt.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gvdfaardv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/grchoirlf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/ghfnvnnaf.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gpwupdzor.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gsdgfouao.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/grvitohxl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/guosxjczu.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gazqjmiad.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/ghndyuzut.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gdruwisut.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gtiovvvdj.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gudbbjoxv.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gsgeyaxli.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gnfvkecdd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gejqqhedu.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gktfnsvlt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gdxmeyjbk.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gsroglrfd.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gbnmofhvo.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gykkapstj.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/ghtaavwfa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gzyjslxeb.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gzwfhystc.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gbylwnkck.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gkznzoprl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gngmcpxpq.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gusauypub.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gufjwraja.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gsqngzflk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/grhwdzsdz.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gogvocyyk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gcwsyucuc.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gwekqbrtc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gybhzgsud.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gzzvtxokk.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/ghpwkfsar.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gqmamugeo.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gxgyodcwi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gphtwbuta.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gabrtudpe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gwaarnwkj.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gnjsfiwfd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/ggxzleyhw.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gnyynzixd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvxbidlzy.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gjfxqottx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjhpyuasx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gwirnfwgh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjossdmjq.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gvuralkrk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/golwypssj.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/galmltlgc.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gpydghimh.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gxkbbvmau.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gqapifbzn.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gsyiwqhhx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gugnewzya.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/grljbsteh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/giarnmuju.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gqjatjkjq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gtamuihfs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwuektewc.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gmezcktdy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gazbvpuyy.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gdfizcbuh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gmyzgqgry.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/givuvhryw.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gijvwrixk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gavmqkjxx.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gwiszsmvb.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/goodkbrbe.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/ggnwmmjsl.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gmiohczet.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gvaujhgvx.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gtplhxtqp.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gpoilsfiq.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gpgarwnss.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gpodjpkfa.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gqtvckzoo.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gbzpqggwf.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gjrxrajke.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/goxfttvaq.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/ghaxtlkka.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gzrbunzea.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/glauizrjs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gejxdbiln.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gzbknlfze.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/grmkwxpmw.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gbubpjkpo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gcvyuyjwm.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gnirhepem.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gaedqeqqs.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gwqjaxssk.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gxhwqflmf.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/grhsvuebd.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gbfotnwdk.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gspjwdlcr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gllfqukza.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gmvadlxxc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gzqckdskw.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gyjipvntx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gadrllytz.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gsdmuwiph.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/glutibrtm.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/grifrglek.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gdlsusybh.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gandmazap.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gbpzbarlb.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gtaehovdd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gkrwlhude.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gazdzkmef.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gfemxhltp.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gxdjunvcm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gotkyvuaf.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gwgtnazry.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/ghqrptbkp.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gndbsyssb.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gsigwaozs.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/ganbxnitr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gcwxxcmqp.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gfgjesxtq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gcqnpaaph.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gkxpqbdio.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gmgowvxzs.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gsjtaykos.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/geiucvddo.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gjiamelld.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gpzxslzxu.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gchxdnzsg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gjkfidvcs.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gliisagov.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gnkboezpo.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/ghvxrmmmd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gyjumkgzz.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gueuwiybc.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gzwnmlhkt.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/govycpiyn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/ggqdteqtp.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gfrqcwozk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/grvjgypqi.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gxglvclpy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gyqlcrpna.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/glvoanzlv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/glfrzudwq.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gzayqsyeh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gbmnomddi.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gbrlpvycn.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gmdakddzc.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gpplpszqw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gfqtffbag.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gzppdxjhs.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gynuxodrh.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gfuhfpuqa.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gzgoqpfxp.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/girdxgjxk.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gpzbcnokf.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gahkmeghk.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gwfbnosft.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gxtbnnfif.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gqjgwzasx.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gfarxyggb.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gjbzovyfn.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gdsmbagkq.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gvkvxudnz.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gyxbdqevx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gvvqupvth.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/geezerjcv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gsmyvdcdh.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gpfpbyuel.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gbdfzxunt.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gwpsxoghi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gpukhosab.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gbrunajtf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/ghtrmlgfw.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gmchnwwve.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gbufdmwpn.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gzcgdempj.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gmqpkoqwn.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gtqddfrti.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gtcfevvje.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gnseqcxfv.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gbflymqaa.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/grgkugbrs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gxotouspx.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gtwaaixbk.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gjdlcjbsy.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gbwkgjsym.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gykgiwcps.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gufcdbtms.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gakbwnfpq.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gtntalcyo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/givzvwwey.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gbzdhosqf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gkdpcjexb.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gxvvfowgi.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/grdhtjlyo.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gyqmeavfm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/guxzbbbcf.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/ggrbuuztp.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gsiuhovdz.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gbzgzgjka.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gykuyvyxf.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/glbpvlwnt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gbyhxlsbn.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gfsmqdkuw.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gmhuffrfu.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gnzkcigtc.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/goiiyaakl.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gznqgukrh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gfahazqux.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gwksyohhu.sHtML


<!-- 参考信息 -->