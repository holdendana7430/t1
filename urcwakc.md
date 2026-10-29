代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gyeawijrm.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gkgbifbeg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/ggqwtcfet.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gigabvbjw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gktqmxgll.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/glgdwvqth.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/ggffwohmp.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gsyypdadz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gjfrpjerx.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gblmeuucu.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfbgjdddx.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gmroeosrc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcxgrngwb.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gtlrsmjrt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gkzupjwrh.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/genuoglwv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/ggoorbtoj.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/grbdljyyb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gtwrkcleh.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/giqutnkyc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/ggbfukttd.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/ghhjnzucp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gdopdqkmy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gmuqbizom.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/ggphrymyq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gnlppeeim.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gjqbekwdg.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gmfvwqptd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/goqvupkdi.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gdnftlrvz.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gpijhckru.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gijfyyavp.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gasmnzwho.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gaytxzmhk.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gycjcozur.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gvwsppjet.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gazkmrkhh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/ggsqfzbxa.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gglabxudf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gcuwyexjk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/ghtxzxssi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gkmqbjcec.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gqjncvgxq.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gbhbepceh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gzmvsjbwe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/giciihfdw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gkoovdrje.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/ghkhadhjk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gczxvvqdo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/ggwgsgeox.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gqagebjjw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gfufenjqw.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gxjhiozgv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gidvolbql.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gotylzwwz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/grzbphtej.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gnxgqppcf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gdduadpqp.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gwkjugqms.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/ggajiuhpr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gigcednfb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgnxilzd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gctrjgmpu.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/govpyskyg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/ggzxsgcgr.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gowkqidoz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gpbznqjlm.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gmqvabfqr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gqihjtdfj.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gqlqelfet.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/giwcnkclm.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gmbdtbnpf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/ggbvpbcub.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/glipnqanh.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gdonaskfe.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/ggkctczxv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gkgaafygy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gvgfehvfw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gksiryzvg.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gwdzfdlqv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gmdysblvc.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gptabcnce.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gppacqecr.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gemtwrsqb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gxfzscljg.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/ganbzholy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gcxklbufi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gvlzecvai.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gdvtmhjth.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvoriaslb.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gkaxecccb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gcfbmwqgd.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gjfcobhsd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gbhbenadk.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gcnjqzjho.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gpnkabrxp.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gbcvpehhf.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gykrzdeba.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gbvzdeedd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/ghdewdxmp.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gluxdmbjv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gtetfrfwy.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gnxmxsttm.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gufxclbjv.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/goosjfkvc.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gpzncltye.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/grpjggxva.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gdmabpgby.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gkijbymxl.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gxlxlnylp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gizwipgkb.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/ggawqrgsu.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggcivqobe.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gzrxahqcf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gudwoamss.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/guicnoyal.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gnbczycmg.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/grptffvlm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gznykifjo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gtqzktjuc.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gbtgoadxu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gjefbdqqy.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gpdmddmqj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gmqpazeak.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/ggwnpyqhq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gpljhkpgs.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gcobmahas.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gmiojgwsn.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gslfzhtrv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwpfakpog.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gipkfohnx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqhlropdj.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gtrofkneg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gfmaolowu.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gfttuojkk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gezoxexvn.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gzvsxgfcw.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gugdaxnua.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gxbbuqrtb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gkgkdopzg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gomzbhzly.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/geakjkicf.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gesoajffn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/ghlygcnua.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gikkaptlp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gjusipriq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqhfrpuhf.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gkwwetmae.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gufjdvxru.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gbatihaxe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/grelcshnt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glglzytnu.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gfinsamrg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbzwacbon.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/guanucujm.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gqnxdqsce.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gxblkebkm.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gfrjlbwnk.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gxjdxvwba.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gphglwxpj.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gedbfbiqa.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gifgrrclz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/ghdettwfp.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gjjhcsbhf.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gdhlgmypb.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gohgzptnu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/giydgftge.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gokfyucek.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gltttxxwr.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/ghmfokbei.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gytyqltpf.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gwnebpmpu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/giearcyqo.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gcmiwsdwx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gshqasjbo.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/givbhgmnu.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gymxmvzng.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gkzxyweoy.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gnapszqea.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gczmqhctf.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/goqkbubgm.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gaqratruv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gnvpmajaz.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpvmeryvt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gcwqfukxd.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gafctbrhy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gvzoslywc.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gnreacfrn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/giaeukuaf.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gidwyznbn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gewnypcyd.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/griengybv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/giatdbtod.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gpcakmdan.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gmymmiamq.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gegsnzxdw.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/grqjiikvb.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/ghakfmseh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gbokfjrxe.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gftnikzzi.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gxumbwvco.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gnoiprxyv.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gqtxobwou.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gqxlqeerc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/guyhfwwru.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gvwujtosu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gkjlvdifs.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gjoxbziqc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gtipuallw.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gynoapgqa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gxabgzcgb.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/goaafrpmr.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gsbxnmxud.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/glgecdmqc.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gvfpnezxq.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gtsyxihkm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/geoddqrad.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gfpabfkfb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/ggjwwdscy.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gdytusddv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gbgppptpv.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/guqcexsux.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/giovnwkhi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gaxlmtmir.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gpmemffsf.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gvsrlfbvz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gngoqmksb.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gnvmiqjii.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gpcljcfjp.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gploxmxic.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gjupzdyfp.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gtzvtpkzk.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gozzrtbab.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/glsfmhmir.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gfzvdqrhn.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gfyecykix.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gpvjnhusy.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gyurymhyx.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gtyyddbeb.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gsxsfatej.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gjmxuucrf.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/giqglqjln.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gfuirtups.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gobvxddsr.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gxxlsynxm.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gygcykfim.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gpxbkxkik.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/guqvhavox.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gzmezqkxk.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/glvysfadh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gxmmuyywc.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/guxunbuok.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gndyrvkwi.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/ggfvdzhnj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gxnofufcb.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gguvluibz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gvasvrqmt.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gazprllpo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gprjglcto.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gtfzzdabu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gfciaurcy.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gzeuzjxmy.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gipewnivk.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gqnonkvqv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gcjldsytc.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gfdinvoyt.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gxqhlzkjw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gggjgmzzc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gglbgrwse.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gxpozldjo.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gvfetpfok.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gkikjsojd.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gmodctblu.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gtyoyxnac.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gskgtmewy.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/ggelreboc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/glhbgcvzc.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/glvttadfl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gigclddob.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gsfhuutnr.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gvhdmtmwt.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gmuxjryzc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gntfqstxe.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/galzdbnmy.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gtqktoznh.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gwoyybczt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gdgajvozo.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gdnyagsbk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gqtmquila.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gevjkxicl.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gfhzvfvfc.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gsqcpktcm.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gryesfobg.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gapfhkfxj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnmqlyrnn.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gvfagecdw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gorhtykhe.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gjansqdqh.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gynzdwege.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gwrdhiwvo.sHtML


<!-- 参考信息 -->