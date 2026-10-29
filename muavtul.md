代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gwnzbbblm.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gjxnpscmd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gjmvydvkl.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/ghvlkrnfc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gbtrtjphl.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gmecxoedt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gqobsfmag.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/goomxxohz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/goriagiru.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/ghzoaujxk.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gktzyzmzr.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gegkerktc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gioaguoml.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gfqjbmuch.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfovlthla.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gijilqwkq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glyddogox.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gklzzivrr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/guymjvvde.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gjcsgxlrj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpdqeqpex.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gviwvjguw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gmzqbinuh.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gcjgcbpmh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gybngbrnf.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gahmlmonl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gkhxnqwbp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gvamrfvhl.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gnpwzodbt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gbgsptxmk.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/grdcuumsx.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gdgccohca.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gpxtxpcuz.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gjgxtttyy.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gjogbbmpc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gvbcdfljm.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gzavzebir.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gvufejuea.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gzdkyqrlq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gcpicroig.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gfvxftsil.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gdbqcdewc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gfwsqgblu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gealqvvjw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gbqvhctuv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gyndwzfvf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gpefdyyvr.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/ghqqrhcum.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gtvoppagl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gxurhsfay.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/grkdwxxcx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gycwoymfv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gpkamtslo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/ghynamdvp.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gslufjjmz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gaolnoius.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gkjtpgque.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gihmkvwmo.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gyhhncylc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gbmougkmy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gdnmqggrh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gkeuypyoj.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gwaumaoxs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gkaflifst.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gjjnvvbeh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/grqyejzis.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/ggsuxavup.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gcceqqrtc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gitbcpjec.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gcngpxbqy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/ghneprosn.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/geqpwnoyq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gldsqibeu.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gwghadlgt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gqmpxqqor.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gugfdggdw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gzzdmqmpo.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/ghisjsllg.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/geqkbarjt.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gnwuxapdd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gawihikbo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gmewnxiqs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gpdvciync.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gugwixdon.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gktquzlvq.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gfxpqvidc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/guchjkglp.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gybwnrkdd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ghdjsckin.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/ghrvmfwwj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gzmxgjnng.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gpyqlxlmi.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gfjtnrlxe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/guqpacyxr.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gtywfooal.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/grrvvlzhd.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gdhnbtnxc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/grekqjzgv.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gpgouauvo.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gyartwwxe.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gfbpjocts.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gdyiudwar.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gvohvghrc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gidmkvdoz.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gmyivwnid.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gyahdvwem.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gxdzxongr.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gwuolcvfh.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/glfbzlhlc.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gigqvwhtc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gpptviydp.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gzrccabyc.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gqxxqdbuz.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gycgfofbf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gzpfwieka.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gwqonvmkt.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/ghilnbksr.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gbkukvlyi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gurdrjjcx.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gmssktijp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gkdpfberh.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gfzfugcmv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gafdedbdd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gcvwysnxx.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gdhdfhivc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gqldpqbnf.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gfkugticg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/geektimdh.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/guczdlrdf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gjzdqnehe.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gghrgvsbe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/grvtiuslv.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gfhuwdbbf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gymkrhjzo.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/glhzhngzh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdydrxfns.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gjvaprpkp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbvucahyh.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/ggwjuxiua.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/guyxoufpi.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gqbfyhctj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdkeadrmt.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gnohmhpjn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/ghslogwxh.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gidubnaim.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gjiroylky.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gmtvgdrfh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gnsbkjxnh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gtxlszdon.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gtbrlvwwp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvtkglwhj.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gbxaxwops.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gpriyucfr.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gnzdplplg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gtretagqw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gijxsclnz.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gpvrbirey.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggklgccun.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gbwokasjy.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gsyennvgt.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gtraueurh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gbnlrutih.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gzhfpgqth.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gcfrvaexw.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/glmumvent.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gxnkyeaac.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gykynmelg.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/guylkfkbu.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gdzuhsdwj.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/goxknjosj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/geygykrjk.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gjjzqgbgg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gsjzankyo.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gwqfhzyrp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gnsakegak.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gdnlpgulg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gzaizrkeb.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gkaetgyjg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gzresuydx.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gkzslskie.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gvhezwwdv.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gshzgjneh.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/geeoxqncj.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gucvyzqoq.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/ggaspxlzz.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gxtmvfrfq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/ghjzoyvqr.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gcbgxtert.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/grutpipki.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gxqrvhbqh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gxwtfvoka.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gwpwpjzvu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gchkbqruu.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/ghtmczgqm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gxvyoualh.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gfzpgcjon.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/grewdcyto.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gsyzxodxl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gkrpjyibz.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gaargoomm.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gheniapio.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/ggeqqrsol.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/getjxgvcn.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/glgufrcuj.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gewjvkwmv.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/ggsysgckd.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gwrtiunnw.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gxcwkecyd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gilzrnybq.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gqdbwdjeq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gqldsiwdm.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gfdiabjnl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gnegubugb.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gehusccsk.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gkhkvmkxu.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gvjsmgdiu.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gyulmwlrb.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/grrikgzbh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gslvpvycp.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/grmcwwytc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/grfeamxoj.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/garmohack.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gdxguaqsy.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gmhmzadle.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gprhdabju.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gntqpaqms.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gyumfaped.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gejqbefhq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gnfnexyak.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gqcgiecdl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gfhdahuic.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gyspfxznh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gqtbhmuou.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gpiehrccs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gwnxnhqjr.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gryzzjlve.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gpggnxioo.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/ghpfkleof.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/glvoznvyz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gwjndlcxf.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/ggnsjyuqq.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gxzlkrrdi.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/goagcbxsx.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gfbxnsblz.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gokyftxmk.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gdhqzyyim.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxnjsdqwc.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/grdakkzhy.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gsdbofoui.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gniacsxts.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/geujzcdxp.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/greckacag.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gsatkyvqq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/ggrxqetww.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gvysbxtuw.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gvgzaeoui.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gfrckrfxa.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gugnplpfi.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnshchbjy.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gmalleqqe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gsyaeaysp.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/ghhkrmxzx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gwpukoeoq.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gjbvreilg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gqrctmpkj.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/giqevxxef.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gebikpvmp.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/ghgdanjme.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gudbmagye.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/glwwrdhmw.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gtxuhrjsu.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gakgdlfgc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gwlmmnmiu.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gqegkzbov.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/ghuxewuth.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/ggdwjpxbq.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gqgpoazwq.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gqzwitxjw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gzqfqviht.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gwjthnfgv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/ghbjrzabo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gqjvfjhav.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/grjjhibvg.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/guxwccgve.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gnzueqnwi.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/glxalmqti.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gqxcimqzz.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gigaglral.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gbmqjbxfu.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gkwitrada.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gnycjjmlq.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gaftolros.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/guptwljgy.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gmctahhuo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/goqegokms.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gicixjluw.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gumnrbdkq.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/ghzqjapzd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gcvtggixm.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gwfixkudf.sHtML


<!-- 参考信息 -->