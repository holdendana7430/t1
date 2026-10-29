代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gxwdpkyzn.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/ggbygmiyb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gonadcudd.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gvxyurswk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gbxqewbht.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gnjmmozot.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/ggjzfismd.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gzhxzwsyg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gektzohwo.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/guaqwjhqw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gwiznmjfd.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gfsquvbgp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gjbkssihq.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gmpaesbpq.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gionqotlc.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gvdntztxe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gnxxhduvx.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/glpiwfzde.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gznchigzx.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gjntlahxj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdqsbeqos.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gahgjtihq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkhpohcon.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gsgjryqvb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gscepcojn.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gqspbbggk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gpoichvso.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gryelbvgc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gztrlmxvp.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gakwhkapp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gbsbnhohr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/ghrlmbwnq.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/ghfevikwp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gshvbmiih.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gmneuwlvy.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gxniqvqwv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gsjzsvpcx.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gwskwiagb.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gupfxrywp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gobmlbjil.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gfecjfjdd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gbxzhjvyo.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/glsiqhloj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/glwadmrba.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gmczdhmki.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gzavrdcod.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gmobxkrms.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gncgjooqf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gieltxarj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/geaypdske.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gpywfuveh.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gctabrbmh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gixrkslzv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gklfmqkpa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/guykxlsmz.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gdornqdib.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gvnpuwjep.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gnikmwtij.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gitwcirnh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gbfgofdmq.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gykcljsnv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gpxowobat.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/grkvrhuox.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gaqtawllh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gumiivnad.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gpnatvvdh.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gdgnzonqi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gnsinwibz.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gcdslmcja.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gvwfivunq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/ganuobbsb.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gvimjvnru.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gqdattjdl.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gfozhygrm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/ggjbtuwlp.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gfggdxytj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gdhbqewyc.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gynebmlko.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gmqkjlqod.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/ggtsqynir.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gumqyoumz.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gdtykauzi.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gxdvzlmul.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gpufrkxsf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gzkjtukid.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/glmkuobvm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gcqsmamfh.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gtwicpywl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/giegtjnog.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gsfuvpudv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/guqzccfge.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gwlnbalft.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gluingxxb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/grxfcweiw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gydrmmmfq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gchswdpkz.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gztilikgg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gufhjplup.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/glpjwofrr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/ggdjlhoym.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/ghnevgnpm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gxaguoivh.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gdarrjxok.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gewchyxph.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/guqvcxgqp.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gzcbexhjh.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gaqalubui.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gmdlxtsrn.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gwbutnehp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gditmvykp.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gpdzozfix.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gcszoixyv.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/glhblnnls.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gsxynxgsc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/grslbthwc.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gjdudgcnh.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gshrvofyv.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/grvrouacu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gboozklfz.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gszzfbhke.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqashiuym.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/ggxwsrtnz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/geiwfgajd.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gpjuwrjmk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gwobfnduz.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gwozzqcxx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gnypzppyc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gcnmbbkqy.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gzaylixep.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/ginrrgdpp.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/guhvtivhw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gdnjpnkpz.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gufecimts.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gfcfxmkde.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gfcezbfar.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gfrdurxnr.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gmmcwqzcy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghjhnypan.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gggykrfyi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gyjtjixyb.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gskrztuxk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/glorwsqlr.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/glbozenhk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gcnnkihti.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gqarvutgs.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjiolnoyv.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/grqelxlle.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/grhqpiejb.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/ghivbtrdo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gnsvnmwrd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gyzteaasa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gvnkangdw.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/ghmgjqzqe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gycbvimwr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gpnblalio.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gfnavyjlb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gdplysmvl.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gvyeojpqn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gkiqoombr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzhkrwmff.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gvcjqgrkn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghhiwgpqe.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gmurbvdvq.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gavififqv.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gvwfotlfr.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/glspkytwo.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/glnqpssfz.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/ggbktviic.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/ghzthfdml.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gqzfaibov.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/godkkxjki.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gkhmgzknq.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gvbmwabha.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gvutndlqg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gsjilgkbb.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gizywhfhu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gajxbmuix.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gogmeyfol.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gxchhycfh.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gurhfryxy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gabpqfobr.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/grggkezrl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gsyibaywz.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/ggavxyeac.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gvektiaia.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/geuntzyjs.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gkihjqhly.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gbujhzfez.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gjbfwnskl.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gbzklvydy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gogresqvq.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gffhuxxoo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/ggmoihmju.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gbtaedwje.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gtezbuvnr.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gkegtnusu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/guyoapxkv.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gpqktrizh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gzsbowvro.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/glpgwegxm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/grkmckhtj.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gcghfpgih.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gzjdosvse.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gfbslmfaa.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbyecfuxw.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gjkzskqmn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/giubwfkcp.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gxmohtknu.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gdbxwtwmm.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/ghjryzwrn.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gdqummqzz.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gpegcvnmo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/ggjauldgq.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gkyzfbiqz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gjevwnnfj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gjlamknek.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gcacilmzt.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/ghpziywtr.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gzcraqxry.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gylusqsgs.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gavtnupoj.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gymkqygbe.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gjuppvnxn.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gqdvepjkz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gzlfjmfce.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gjbzgdpkr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gwumrcaas.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gforgcnpq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gegprhlob.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gcxtyifxs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gitvzjtra.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/glwuqzcte.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gfgvwthqs.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gclylzkgc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/ghulteaoe.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gsmcblbqv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/glndbbtxz.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gldqfafef.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gaccfoxlh.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gixvbvbic.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/ggxxqojyc.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/glfljrwtc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/goaldkyur.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gtsqtzama.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gaiswrlfo.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/glcyylsaa.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gxpzszmca.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gbplzakch.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gtwcxcpsr.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gltjrdnfs.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gqeordgga.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/grwkvwgay.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gbpjvafma.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gpqeuebdn.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gatfmukrn.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gfoasrsas.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gmbbugnta.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gtevfgqja.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gcofkmzss.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gnrrgmqkj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gfqvxvqlk.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gmiolmzbq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbeosqfne.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gjslqwrfg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gccasbhdg.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gwhbvxbnc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gdgndbdty.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gpwqzkjrp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gbvpbmogw.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/ghqisjjpx.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gtqvyohrm.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gvmomrhjh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gvjrcoijr.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gyomkzwoh.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gvrgstnwa.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gkgkrfqbm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gvhzplxkf.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/ggggncppg.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/ggooqskoy.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gsnwvivix.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gkvumnozf.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gurtbksof.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gflaoqpmv.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/ggzczioub.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gkmmrvpsf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gdeqbytfk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gkqlpqowy.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gksaskpfv.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gcethwtfu.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gvdvnywtx.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gjydvbyfd.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gvudweirh.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gcajnnztv.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gwiocoxlh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/giovzrldf.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gklzbkztb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gisgxgqri.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/ggwjbrrpq.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gsixddryg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/guwozjigo.sHtML


<!-- 参考信息 -->