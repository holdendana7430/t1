代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gorlichfn.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehyhfkrk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gqcagrnwx.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpwwpjtq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkomrsob.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/giquimbyz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpoitcvhj.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdcnairm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/grgtjrnes.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtazfhgl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwbxjirh.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrxbpkcm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpmowjlyr.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gvqesruua.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsmzyzip.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmhemycr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glivsksxm.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslmcdfmv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbtjhims.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gkgtwwidx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gavhudoyx.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gmcpqtvqf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbjnrbxy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/grmugpfqj.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmcgdjjx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtafzhftj.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gxllmyldn.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gwouotznu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/grivnrwvw.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlxxslae.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzflnbni.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gzmmfjovz.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gnsppbtqz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaozqwob.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfdjiqtk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdydakeo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gscdmlfxh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gxegijxjn.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gshaoduvh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gwoazxkuw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gweoshxuc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gvxggmaze.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gdrblfzav.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwlnginw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrrtwemj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/geqvvujep.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxpiuqzy.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gmsqcxgmu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gjoxsxjic.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gidvplemf.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzillfqfv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnvpglch.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsjwurqf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gyjrldqad.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/glhwnxwhu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gxcsegrax.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/guuspuyqx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gnalswfdc.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbbsvalf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gbvkzvrze.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/grtzmjpbu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/goeqbgidx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gklcsrzuh.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gyomnwsko.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gazzfpmxv.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsxrazxt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geshgjfky.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/ghcuokixf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gndatezqt.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gfozzodod.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdngmakh.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gwptqlfyi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/giolyucfc.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgmujdsp.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqmfpkxk.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gsvzsdjyj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gpcqmhfzz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/glkcewjkx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gfnkzhskl.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/ganzsmnnj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaucwvbcm.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gebvrgwmy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcmqkjgo.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gnohyhvqj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ghbpmtauq.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/glggwimrk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/grltanxbb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gydruwccn.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gznjkvlia.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpemxxgki.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gcdiwfott.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvgdqefz.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/glhfbqdjr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyzeyjde.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxxcnwkv.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giulgnwwp.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gdnuauvqm.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gimnzfkos.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfkmmheo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmwzrqzv.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkeobohz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gklnkxwda.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gotmaxyzi.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/ghapkswnv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/geiomztub.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gpqzlypkk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggukokviw.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gryzeasne.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/giiuphcjh.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gcnswvzem.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gptvvvark.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/grjohelrq.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmxhfdav.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/ggsbmehde.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghheoznow.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gzswxqspp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/ghebwmfis.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdjxikji.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/grjapngbg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsgnigqn.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gwpfkvyfo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gspmijfcc.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gmzcxqqae.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gujvveqqg.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gnumdwwtv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gknedbisc.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghivwsazf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhudugsl.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gvryhzofi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gixzvhclj.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gcgcyoqpm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmxyzkpr.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/galllouvc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsanbcrzt.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxlygkci.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gazngdrki.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/geyzoprfw.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfzzlfnjo.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqgzcvgs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gavcmomwn.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gytxtpkru.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gscsogmne.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gzcippdig.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gyzskhwso.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gagptfopy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gicbobrwv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grjtggiod.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgwogvaa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gqvhxjgue.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gaghmhsgu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcopicrqz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grekqzvbr.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giserqfof.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsyyiaqw.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gapjzebcz.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloikxxjq.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gszvppfay.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxajipue.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtewtsfqs.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gztlwnxbw.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gxamkdhtk.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqlkrxwc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqdbangc.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyugwmjv.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwxioivy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsftrhaxr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gocwjgiuo.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkbggiel.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gycpatphs.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gacjhwdpz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gasuwhxyj.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoglbuja.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gfganenyz.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/ggvfafenj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gpynadioe.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gzerxyorj.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gssldiobd.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejqqjwci.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqmerwzz.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzweehglu.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gcaoijgar.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvucrulj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrlknrxf.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpopokka.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gyebmqllf.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqbdowhg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpzlshaq.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvmvztep.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzvlqxjsc.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/grkgjuamp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsatbpvsz.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiuwoqmq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpxrtdjk.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gspacnput.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhraezcv.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gdouhbout.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/glchriguw.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/giilhzqzc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcbdwogu.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfphtbqp.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwemuefpe.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gontkjkja.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gifrthufh.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpcjpszj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnqzefjyw.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbbnqcyd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagxvpaas.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gmcdhleqs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzxtoejq.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcouopcv.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvubujwj.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gauemsued.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/griawhnek.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfipelewc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpajxzoyq.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpjlkzlif.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gjixsxpoy.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnwgbynp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gocmtusww.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gquxxzoit.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmcwddocs.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gxoktpvys.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggikotzbc.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gyxsmrtaq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gkopslwjt.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxzthvpg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/glqmzapzw.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbmadbgn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjdimgdq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvmkjgcz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gidxmhfif.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpitsyen.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyjwfyar.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdgnbtiv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamiwyzho.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxdmyvao.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcbwswlg.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/glwfoocxp.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmhdljmi.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/glqfbkwlo.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/glrtvbyuh.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gjqititxa.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gggkobocl.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzvjifnw.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gpduwaauq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gginxfdis.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwqbbicdl.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gjowulenb.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gvetpcgek.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgbzjuzr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gamcqeksd.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghfhxplk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsswcpnv.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gijcmkbfp.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glngjqtgv.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvsslooi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gqycszixw.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gwsbvffme.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiuqglgx.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxgjkzoe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gqtehcudt.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/ghoyldugv.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjwiqror.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gnywkbcha.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnjcgvwo.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcesezmkl.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwywxultz.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqxouklk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgxspcee.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/ggwcwmqtk.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrurkgeq.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gscmcnsza.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gnssywgor.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxmhfvaeh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gpqaemtbr.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gtmuvpqwt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdsijwjr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexxekljx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gyxtgdaas.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaenppcj.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcddyhemx.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gngcschwk.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmtaerei.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gkrxcwils.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglrdszuz.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gvutgvwme.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmisdrhms.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnknuqgkx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjpbajgu.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/guicbhfyw.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfwbrwlz.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/glrcvexrl.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuwwfhyo.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gpifiuell.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxdbhdyq.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gkfrmbybj.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyrszlww.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gtopkecft.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gluyvvsdc.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwzudkuc.sHtML


<!-- 参考信息 -->