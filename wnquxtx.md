代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gyfosvwcl.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gsskhbmfp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gvvekrtwg.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gwsehjxfq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/ghvtozogv.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/guxglrfrq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/girosvrho.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gdhtdzoae.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gaqnrxtpt.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gqztkcxgy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gttbniasl.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gzbvulfir.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/ggkkxfcdx.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/grzwphdix.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpkiboqai.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gtuunyqeb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gffxfgzma.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gbdfyqrci.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcawxktyi.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gjfrjckzd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gidkpgswz.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/guwamruqg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gfgjikjob.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/geocynxye.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gtwdfhwpq.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gyatieiyx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gjgoecpag.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gynzzlzkn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gkplmixxz.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gocjmhozk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/geyomkoxd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gvehcpohc.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gwsgambce.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/grivdhioy.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gyuhbhchr.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gyrfaeuyv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gulkwpxbt.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxcvgooso.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gvipbabba.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gsnhgwwlb.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/giptlnbwq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gagajqdbt.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gjhnrcvps.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/grpbowsmc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gkvumfpsd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gnhtzjqxj.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gjycegmuo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gxswrsicz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gqivntmwr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gjhefyyiz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gccwvkows.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gnorhbekh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gtvowywsk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gczdbzblp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gadfxsqvi.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gqcjulowb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gqhjjufjt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/glykzqozw.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gkszzdihn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/ggzcxdfxd.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gicrymtsv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/guphznnhx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gyfbycoul.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gbabkwhjr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gmjhoeeur.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gvzyvqpdp.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gkasdzxir.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gsewcnuhw.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/glqqkhvtx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gqxplixly.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/grvlyvlib.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gftkplbus.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gfjdwjjit.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gzaqaipom.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gkpjwjfyq.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gbdlejtxm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/goiprgiun.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/giaemhphb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gmehaxtjl.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gftxaodym.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gizdbjzit.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gvscqeire.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gvqimxgoa.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gzivabplf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gefcafdnv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gyqqhpkxq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gxsovxnum.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gdkemfchm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvrjshriy.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gspxfjlbe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gfqagjpyw.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gyttfyoqq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gtqghdhny.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gjwinxjik.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gfpcmkwii.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gzxusmswm.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gcfyrbvut.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvkivascd.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gzhiufnpf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gxctwylvu.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gpufhskhb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/glelbocwq.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gfapfwiki.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gpglwccxk.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gjkrrdgtm.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gltngyfan.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gbaufvldl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gaegnymyl.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/giingvsfv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gnlblmisx.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/glsyksqqy.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gypkpzyzt.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gctkaicka.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gkstpchkx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gjcogxoye.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gqwjllrnu.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gxkdmtvvn.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gxwmvmaqj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gmvwbjcwo.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gnkkpchbb.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpstrhpmf.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gnzbkhycm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gclmyjskj.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/geynnhckt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/grmdwhbhj.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/giusxhrjn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gsmlepkrz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gmjvyebmb.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gcofryeqm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gsijlfacw.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/ghwdexcav.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gyeubsblk.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gvndhtecd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gcpmvqhgw.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gwlkhoryf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gvwhaobsq.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/goewvqawb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnfzkbutj.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gkmusyopg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/glruufbzu.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gyvwaemiz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjdqitkyz.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/grxgbgftv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpcvcresd.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gmjkzmrkz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/grvqnjsxp.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gcyyoykht.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gpwhoiwmo.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/ggwkedjkr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gzcyvztek.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gerkcqbtc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gbrfccufh.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gthowswjk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gvjswwhqe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbweqombd.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gojscbpjl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gfnakmacs.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/ggftjsliy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gxrlzwnlu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvgnfmsav.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/geqpeerlb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqevemfab.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gfoyqwmdl.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gtclgvvkt.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gzncosbop.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gcjfjjvvm.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gnhepmorv.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gyvfxjzay.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/goegmttia.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gdwpymrxy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gjubgcgbr.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gzgqdenjs.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/glnkwxedk.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gzmgnugip.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gjbdsddqq.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gqjdjezev.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/ggrwpxccb.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gbykiyllj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gjrsbmcaa.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gwbsepxfj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gnjovzylm.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gagpzjdva.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gxsbybnpj.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gcvcnjitw.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gazaxoogf.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gwovcwjkt.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gjjkxrfvv.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/grmattiuk.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/grzunruwg.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gatajcalm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gvyyguldc.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gwygjvpop.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gtthsqbvt.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gcttqduxc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gkxxytbkr.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gbigqimwu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gtwgeocdj.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gijitxtjh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/ghasklkiy.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/goqczebnn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gjtiizxqc.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gsnipmduo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/grraddhsc.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/ggyboaiyj.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gvazbwvun.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gdrslksek.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gvlwukxif.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gkwjltnsd.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/ghexstdob.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/ggzmbstkh.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gciunhxpj.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gvvjwmqjz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/grfapzwpg.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gmobikjhv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gijsdkfzl.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gnrlkiziy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gfsekuzpb.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gghxyybpi.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gukarqcwz.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gjjnpppkc.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/grggupaqt.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gjvurevoy.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/grdmklxqw.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gaquiywrv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gkenhivvl.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gpervzetf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/ggsiidyor.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gccgpturs.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gltnabpsg.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gshfqsdpl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gxbhkpobw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gfvjvtaob.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gnsgjigps.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gvqklutuw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gemwuraur.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gyxclagpn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gfxiftefy.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gjomcwywp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/goghuaxcv.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gbceeioia.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/guqlvxmhr.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gewwfnhck.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/glpkfuosd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/guabowwey.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gpdbwlomr.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gbqwymxui.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/ghtqpfsgl.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gcrrssiwb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gviaqyvrk.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/ghngidqqe.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gmlxtanhv.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/ggbnothtl.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gspxiivsd.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gfgrilicg.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gcgwgqsii.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/glvrchquo.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/giktrbqat.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gglmgkikb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gejeggwyo.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gflksyfhp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gukfvfibw.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gsocgwafd.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/ggzdokxee.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/goxydtcqp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gjqusoohv.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gvvugkzij.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gpgvqjyef.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gwhjsvxbu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gkoipovin.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gexkfklfj.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/giutluhbq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gcaztofeb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/ghqpvgemh.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/glmmdiafu.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gnzwurbxi.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gdjkwjspe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/ghuifqivt.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gtpxwxvgo.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gjksnkpte.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gfznodoom.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gqhcghqvq.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gpkhipaxq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gnqsqybno.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gycznlvwf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gjsxghhch.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gbzkstmqr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gzbkgzixj.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gaannrjli.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gxjpczvpk.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/giqvqddku.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gudcbmpmm.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gozxpubnp.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gervlybmj.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gwdqzdaae.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gtrjzbsmz.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gxulonvfx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gcxigcokf.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/ghcqocrvj.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gvugitnql.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/grwekhosb.sHtML


<!-- 参考信息 -->