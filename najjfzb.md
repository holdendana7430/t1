代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gchduibfd.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gnqoluhji.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gqfcemnwd.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gsvmdgaim.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gdwbvqkci.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gsubrfxuy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gfjhjxdow.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/ggooixpxv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/guhaugghc.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/ggxigvjit.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gakqerozk.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gfplrahcq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gaxkohnmk.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/grxymuphg.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/groidjqlj.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gptohajbj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gihhtrish.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/grdvsqdsj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gppwyvcbs.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gypmzuuit.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/genccketo.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/ghejvtdpt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/guhifaumj.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gfijcnubt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gjiapbdkv.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gposfdcno.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gjgpcvozl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gjuhmcamn.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gafcimdkz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gtdpkyjao.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gdrgocthv.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gebiqqxdd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gpmpcshcu.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gzguomjwe.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gimemyxup.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gscnuomvh.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gupqnuapf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gmvmxghyf.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gaeqenfsc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gdspgquzy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/grpgmroer.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gnwtpyvao.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gsszlhyhy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gmajozpyg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gjoombtkk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gumelvozm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/ggmjjtadx.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gpsrdutpk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/ggrttglwp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gkasafkff.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gdbdefloo.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gkadwjeue.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gltwrguxw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/geckfnrnj.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gvcgjtdno.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gbmxawpck.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gmltqwcxj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gfiddrdru.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gqxiuqekf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gcuhujdlw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/ggkdugiur.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gwoamptrb.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gukwkosgc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/grmjclllo.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gbrzjinjz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gcdkfyljo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gvyzaltug.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gtamcgkav.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gwfiwwkga.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gxzqyricq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gotoqhgyw.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/ggpebhfei.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gmquzsxsa.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gyflxfodl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/grduhpmjw.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gzalpduki.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gaeqemguv.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/grdvplaln.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gdicobudg.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/giprlueas.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/giwijncgi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gurkxhnox.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gawarkqpf.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gtfqvznrv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gpnnixvbd.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gvdieyddj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gypgdkevj.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gejstopvr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gqouhsbvf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gulxhkfiz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gaxgutsis.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gimcclpui.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gnwfuujmj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gkybdbscl.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gqolfftxj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gugxugwgx.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gtixeunwi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gxvzrrlmm.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gllghbltg.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gvjjeozio.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gmkntmjrm.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gpvytiigy.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/grxngbkgy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gcstegvaa.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gltuhmklp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gljxbfoyu.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/grhvxugsm.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gjxatwvtk.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gzjvqucph.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gvjrvnojb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gdwtzrfqp.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gbhpjmcod.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/glpxzjbqm.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gwwlcykem.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/geredcwzb.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gazxlmrdj.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gcvhuznhp.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gidqfkcjl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gfkwjzrwi.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/grsbbwdoo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gyvphpdbz.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/ggjuuzybr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gqkzrjtib.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gvyjghcrx.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gljbcqrio.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gzpmrvpgd.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gyrwtorvt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gxucjhucx.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gyqtvzulx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gjocbgziw.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gidtujqwy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gkqinesyh.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gueeilbkl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gacxnhhrl.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gvvklrfwf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggclgjnii.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gxmpqyzfr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gwvzrikzj.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gqhfgiggl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gukwssppq.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gbxmzpwmb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gejtslyml.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gmhgjyywv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gwztnjkgf.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gelmkzoyr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gwfahfihk.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/giyyeqxic.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gjeqiryot.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gthhwneof.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gyruonqyl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gbyzljvrr.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gxchxaaxb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gjxzkxcmr.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/ghwgwhkbk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gppwywrgb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guoultixl.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gmpccoeeh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsyahxhps.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gnfzppcfg.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/glpcscmfi.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/ghcakqtsl.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/grclwaqnp.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gpllijuvp.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/grginulue.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gmttyxqus.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gkftkyouw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gperjctxn.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gvdogetxy.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gzgjliajk.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gdsezeqae.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gbsyzsevz.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gmdfbdrwk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gquhvqciv.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/grpwpibrx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gpdhtopdu.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gcuqzaumr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gwaonwoye.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/goobzbkua.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gjgwvxzhf.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gdwofzwah.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gdeonnzxq.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gztwytrec.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gewyttcyj.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gikawjoqs.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gewzsrvvr.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gnnuqkjlo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gehtvkeuk.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gazthtphe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gfwzzgpel.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gdpnkfshb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gxrjfkkev.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gbbegstjd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gfgndfebz.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gdclbdrwj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gfkjgyezk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/glggnapho.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gtszocpct.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gwplrdknf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gbanoieim.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gbgbwhwmp.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gyetqefcu.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gtobvjmji.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gwmmlwilb.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gekndknxs.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gusjqskmw.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gltqtlvul.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gjkpbekrq.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gqavxqjxp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gtttdvkxf.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/grfszjgqk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gbhoiikdp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/glnnlhahh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/ggvczspgl.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gjtcndjjh.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gpfqhppjx.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gpvtlrkjc.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gtoxvdfnr.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/ghsygbagv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gyplyquio.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gxxqhaict.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gpzkqwwyl.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gldjzbwyc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gmwpxsrsu.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gflwukrbo.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/geihxfolm.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gmufcjrid.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gagezqspn.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gnbmmmzvv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gopnsiurb.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gqgmutlxq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/guaepcacv.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gnphalknu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gnskjtlfq.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gcxilhpmy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gjbxszdxs.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gajfkcgqf.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gcjlsddpa.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gcjtvztuz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gjqdznerg.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gguiypshe.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gwkxbkklj.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gvymrbbmn.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gptlxgbbg.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/geptjnjib.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gdgkaefsn.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gxvunrnlf.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gbpdxlxyk.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gbqvwuxjt.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gxgbqpyfk.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gknxcppdx.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gozokkzoq.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gwnkxdqby.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gphyilgjy.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gddmfkhtx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gltfttlax.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gjhzahtbu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gddikgyqi.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gjzvanasr.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gykqekomi.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gegpohsto.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gajjkevsy.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gsoxxzpeq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gitervejf.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gzfkxvjzt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gpsnsydok.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gmrjgqmwa.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/garsghcva.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gbqvxoken.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gkxjbcies.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gxylfqwuj.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/ghekhfnni.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gjwglwdir.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gccgjbtip.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gsezxdvnx.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/goukirtkm.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gsdywczgy.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gutegxcjf.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/glvmrtexs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gvuyduork.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gllmdjyko.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gkxezhgfb.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gcktrgvqv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gpmjhqqxk.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gbomcdxli.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gzlxbmjjb.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gmyyuxdfm.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gfwpttmcc.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gadbhmxiq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gprnxhcgm.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gwgacnbrt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gnnatisdd.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gkgyekwpy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gmwplgnbd.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gnasmnptc.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/glrrucoob.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gqvoupijr.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gvqgrkjzm.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gjeaqhmey.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gyjhppztv.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gkzuwwwbq.sHtML


<!-- 参考信息 -->