代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbchidqtf.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahybdbjs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgfbcyft.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwjykvzi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxzwdlfz.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gulegaxje.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnnryanfb.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gnsycbwze.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcugclqvz.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuienzsp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghenwxncv.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/graonjhvj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaaeqvtl.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgmpragu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzavlxlnw.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/ggfynqtxl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggbxrlpao.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgbzzcwk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcmbsyry.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gunmbudbp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gwsporgng.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/grrbnbxhl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqpszfkg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmffuorv.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdbeukjp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gquehgaov.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/guewwpsig.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gnfqqxyrk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvjqazqp.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gdguvpotx.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gapdtymqx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gduwdruod.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gskrphebq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gamgprptx.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gizufubon.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghoasdwc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdsppelo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndjtuicj.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gcwewqnax.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/godzlwogz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gudjdwlds.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gstqpttxi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gqjyeydmg.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblqqktox.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gbernixnt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/goopyxpmt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsyrhiik.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gurjdwoeu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gqtxdlqba.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gcoausssd.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqsiojlq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwueixbso.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gcmpjpufh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgvbejwp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkxxgxil.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcntxdjrl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/grbibukxl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gtlhkmlmw.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ganprxfea.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/glqigffbh.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gexpbofrn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggrltded.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gchnldbub.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdphxywsy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gluzqazhg.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowafvijv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonfxlrjh.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gsautpyhm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gquugkeis.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gntxjtqhk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaurjhntn.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/ghahpgugi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gibdlotfy.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gcyyrmrxt.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gidhxvwqv.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifgmjzje.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqahwelz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gempqfyvm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gkiwqpdca.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiflrbfv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/goljkykjd.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gvdjthqyn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ghwgnidvb.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gnsjzxilz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajsejsyr.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwakqzbn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gbypbbhbc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcrhjmxs.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdgzdusb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gtonzxfdq.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdomddbji.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsqxkfbe.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gdtynyamv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlftvnln.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzrnmxgr.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpsddaft.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gdariflpf.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gogbmiunc.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqqzghrb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvxphifs.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahbgsulg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfetuhmod.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gsirwiuwm.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gpktslzfc.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtftbwxci.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gejmooekv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/ghtirivek.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gumrjwehd.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/glbkxprhr.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gqnfqdkoe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsntltorv.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gjjkckedn.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gerowevzi.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gbipgptzi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzemuvqeu.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gvvgmicvm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsziobjc.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gyhdqydqe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gmcmjmgqq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqqxgdqk.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvytlrug.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqquokfn.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrjbwufx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxepmfzoi.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/ggfcesktc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gfppxwyph.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gndblwufh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbrwlsfo.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpsfegcz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfjyqwqnp.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gwpeplraj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnpnbdkrx.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gghbabaec.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjsleyyn.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gskoiwjju.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gllbierhk.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gznjcxvob.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvjgusqk.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gprabpdef.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gtvqxxvsd.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/ggjwopkxa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gihmimwyy.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyylfoowu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gormmjrwf.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/glfzcakur.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gnwqmcvag.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcjjdmjx.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gmyucffdo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gaamrsshs.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gsiatpsod.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmadwaki.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsgwlver.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gejklsuad.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gegovsoft.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gcfctpetn.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gejioothv.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gvirzesgm.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvaaoxfa.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtqpjfti.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggavmmwhj.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllsxfhwh.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gakqtjknh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxrpdkmd.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvasplyja.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpnldaac.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/geysngsnc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaoglqvcq.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcflbvidm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/guykeigey.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/grlaqsbsc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdrvwrto.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunrpceod.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyhqrccs.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gryutdhpo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsvhxgzf.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/grobflnzs.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gfzymayed.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gopmgmgwl.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfgftcfy.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwhqnpbn.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioqsvjhc.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gykcbecmr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grfgvwcjq.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/ggytctoef.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjanivtj.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gpxuznyzi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gznnfuyeg.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gukqbessi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigpeeqfa.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/glzxjfujv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghhybefxt.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwwtjksx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gobtkubcg.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkxagsvn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gypnzsyun.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gikcxebyz.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gttdbsbgi.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gdcwrziqh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbnmypiw.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gpgmogdbi.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glmblagmt.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gdijrediz.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyftuibfd.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvrlenmxx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gynuozuaq.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gjivonwef.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgdisnzq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gatpgpdhj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gukxthxzt.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gtqhzunbk.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gwzvqltbc.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gjhegpyuu.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkahyimnt.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gjuydcrbh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyskzmmu.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gihtqqozj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdftwbebe.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gusaehjrw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gjtekzhld.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gaagcvixw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmyzpduc.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gnldayjph.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvukmkoio.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gggktahtk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyfrozxx.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gsqeqwlcy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyarmnyg.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gdhcynkkm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxgxgawx.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxoawmsi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/geudxeods.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccqxozkr.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gklreskyi.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gsepbuzjm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzwezqjp.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgjbinbp.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqbrpcel.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqocbruj.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdohqmgp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdthojcir.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gldwbcoza.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluabqojw.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzmebpiz.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfycmypcf.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gupjdfjoh.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gkunfuglg.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gtoyhloyh.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gmtucuvia.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/giqwxebhv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpsaycot.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdapsobd.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/goxzlgaok.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnbmruziy.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gsxmpbgbp.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grqorvuoi.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gcoblzqoo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkrupdfg.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/giksvtchr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpueywpjf.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhmmrogr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gmevvymby.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxmiqcwl.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcblbdxuf.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gndxbnjzk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gahhahxbq.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsycpqpwn.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfkopsej.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/ginfwxzia.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjamlcng.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gaicdhwue.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gigarenyx.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuwtvwxo.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkamilkz.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvrnvbjod.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gambcmpbm.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/guhwryygr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/ggrzofxvx.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxbzexnp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gnwinwulz.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/ggfynuqvc.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gljtnzbsj.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guesdmrlm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/grlsmpgkh.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/glkvagyad.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghustognb.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gyrqjfjgc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gwishyzmy.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gewakcvjb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzqtdsif.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyabddhem.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/garmjtzdf.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gzllxxtth.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhzdegyi.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golrjywlv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gybvjxhyt.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghczlijeq.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gnvlqsdbh.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/glhiirmfd.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkqmfrpb.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjwtycnp.sHtML


<!-- 参考信息 -->