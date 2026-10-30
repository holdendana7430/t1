代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghffummtm.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gnhkdqspy.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbidofgqu.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjubapcg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhhzpwek.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuhjrfno.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galwtrbqd.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqganfqwh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/guxmakmwy.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshorjzto.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gjdtljwcl.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gooxvehiz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbrhpsbf.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbwvfwjo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/grojroxlo.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gwkyuplne.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/guagctbgp.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gllaksgdh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gydyaztcy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhmuecel.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gbugkqbil.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsulidnt.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpiiecrj.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gpqrbpnbw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjivdooz.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gydfftdpd.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gqjkrrhju.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjyuwvhw.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gckmvwlmm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/guxaunyoj.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevexdydn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwbtjmdn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokbqxrrq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbnvppiq.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhphufuv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gwkrpblvk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuwqprmu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gsauaehif.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gjmqptqjs.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkqlcxhy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhtgtaol.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvvdktmg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkpoqkmg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljodkulk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gmopfokbk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/ggahgukgr.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gmusuysaq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjmjpcav.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gxpttnegp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/ghoqdrgel.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpcxzwpm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxvlamow.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptrvgmdd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdjwvnti.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpulniyfd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/giuxhlojp.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gtodqrueg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gyluuxrsf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gytqozwuk.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkckctgh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gfyekehia.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvacgorg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gevtbtgiv.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/glhfcnmjb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkjjiqijx.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gikgosweq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmayekdzm.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gijdkxwhb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifcciejs.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyebrgzod.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhzdxika.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkdualud.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/goccsjucy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcegbruz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlzzkgwe.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gitzojihp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvoiczlqx.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitehzdpd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gubvithla.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gareardgi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlpukyya.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gxfczfvtj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/giurlvakt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gsumnyzcy.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/geynrkilz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkihkppqg.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gemjzvgtt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqotoqntw.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkptvlnbz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/glzbywxkx.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gacnitmhw.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gizalkhie.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gznlxsbzm.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvxtvdnq.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkepiawzo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfunenvri.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/glrhuxhex.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrbwyoag.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/grwhbziht.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gizcvcboq.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/ganjuxbce.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gebhnwulu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/galpetfhu.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gkexyajeq.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxjjuhtnh.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaibkfdc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghutkeyky.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gipbbcqss.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqevdccw.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gttrgaybx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbhcoprz.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gslftqywg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvdclajs.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/giypvwcsh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghfyzpmju.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gfnsljobm.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gzimpxvab.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/geafyowbw.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/giyjtlccb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gvkjzdqbb.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhdmclta.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gptyxippz.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gaigblqxe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpehpigpd.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gyviazead.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbinzfqaa.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grkzaovsi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtxrhusk.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gpghbxtvw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqgruajia.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gzehrqtga.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtewrvdjo.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gkikonwmx.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnocagryo.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvmuwinj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfempgllm.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gecsleuiy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnimnuxiw.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkauqswmr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gnkwawdqh.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/ghykwxkco.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gxajavpaf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnarukbmz.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycpioqmk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gdywfqtfx.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gfzpqmzvq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvibruro.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glykyafuu.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gefffzwrx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gocngrhfu.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdbfkbcy.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gfjwhlzef.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/ggncrsqru.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwnagftu.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gakhuapwo.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylosrrqd.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gjnotbwue.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/ggvzdgowb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gyyibtuki.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzmsqzhp.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlccyitp.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvjzvezf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/grvqhrcay.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfcheqbzk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gcptymwqe.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gaeywnykv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gbdnmgccz.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gltpgypgg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytnuxmaz.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgnbzifo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/giholzdzk.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgfbhmcf.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/grpqrunvq.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuleqcjn.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzbxnexx.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ghcsneqii.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpiffoqb.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdzallffn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gwexmmily.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/grkysxrmv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjmsmjqh.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevabrtzs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrgcezgc.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfztpgda.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggrgmwgem.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnpfmyxp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfsgahkhe.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwexcqjaf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwhwkkggu.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gtgpuavfp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbdozhui.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gqspqmfzm.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkgtbthql.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzecufrez.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grvmvrjsx.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxxsfcij.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glwuxhkzn.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gfapsaekz.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxkogzoi.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gwicfnbog.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvuhgnay.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gddccbtmn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtkfhkvuv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geacjaxiu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfezxroxj.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnhmidix.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwebkgyu.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gxikzxgqs.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gsubchboo.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gwavtqyca.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnkcftno.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvrnasyhc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtzxoqwx.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwbdgykk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/ggzoxabdf.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/grzwcbdgm.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gomzodhgm.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtcwjeid.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getojdrsy.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gubrzksfa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gjrgfgqeq.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjwsvybl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhssjgim.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvilgsvko.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gczboltaj.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlyiksya.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzbrskqs.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqgxcfkou.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gicndomie.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gkomjqwqw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/grykzxcrx.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gdopoyubc.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ghajoofyf.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnujyhau.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupudnsvf.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gkyuwwmss.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqobsxsse.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtemfojmr.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzspdftep.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqakbanum.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyuyjifk.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgazrlen.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gyczqocfg.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gaanuuzla.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gqmwaoglg.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxlnqlft.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrxhafvu.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gebquhuqr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grfsamlsd.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gvhfnuixc.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcdbtyqp.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gyqybysze.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/geffmkaot.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gwattjokf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/godokwvbo.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpyxxmpm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvgrxocx.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwmoksdp.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnqpgtrm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlpcdlhi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gcevdovri.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxvuljoai.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwhdlluls.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gakxshdcn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvhmkyqq.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/ghdcqjpgf.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gvadbncyl.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gedayqvxw.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/ghamffijw.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnroasuq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfpxyzkk.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtaglgut.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gpfezvxyf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbplwtodr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmxreerq.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdoluiye.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gkcervhez.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnhbsnqw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/ggkvhrvwr.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gssnsgwfk.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gpkpzewwx.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gxdaymuju.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gsmwrbqmm.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbpraltd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grldwzqma.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gemhybszb.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnrkeymw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfhwzhjp.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gglsocqdt.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gajrjvryh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgxqrwbl.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnqzazdu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdmndwld.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/ggecpyyap.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpktvntjk.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gsgptkutn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gmhdpilep.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gazijhhoq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/getkpoasc.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gpukrowih.sHtML


<!-- 参考信息 -->