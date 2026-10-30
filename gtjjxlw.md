代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gztryonmm.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gttxyrmmo.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gdcwxlitf.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gnggpbbpb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/grjdvnvih.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gbjvunedw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjsivasga.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gnudkiwlh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqgrqdagq.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gvjpnzkfe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gorpmjlyo.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gyoejbwyw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gatgqzwcy.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gvlaukpwy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gkwgljyhe.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/grfebdwag.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gutxjouwn.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gomfrtarp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gctajnzwj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gksbeikuc.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gzkyaxfzk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gyxplilum.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gtwjveqny.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gplsiylii.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gttifemwf.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/grvmrqwut.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gvwhdrzlx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gzdnrgrrx.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gdqgecdds.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/ggxhxptmt.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gcdvooxdf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gsruufxss.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gignryswo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/ghlnrdnfe.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gedatzezt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gfqksivop.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gaoprdoya.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gltfakjeu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gkhrabdpm.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gcwfjblpu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/geguwuvjl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gcgucxqog.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/ggjtaxjte.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/grzppkabx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gmjxyfcbx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gzzfjmnyy.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gjzkafvkt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gzdkaqsdh.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gpnrpixuo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gnuqegpic.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/ghwtdjgrr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/goramfapf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gurcavhhn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gdjpxflcu.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gerqjjspa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gmrxiudvj.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gasncmdmr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gnbgicqhe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gfdkjcppp.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/ggowwrkbz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gtncqvtjc.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gjxavgmhq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gzmfpfsfr.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gyxgxufsq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/glecruoiu.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gvgpcgwwt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gluhwyknp.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/grynknaws.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gttnblngf.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gsaemqzue.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gtyvkahxs.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/geidyysjk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gvtybbaqa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gmiqqloqm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/grzemxrgg.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gictpmcya.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gufdkiwax.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gjhsspbhd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gjllahtrl.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/ghidrcbjm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gdxzrntoc.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gtjydppiu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gzwqnnumw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gerxnwhgd.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gixsrrliv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gntvifuje.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gkhuzhlto.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gytzptdeo.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gamgewwkc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gwvbtmqxo.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gqcmocqxr.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gjssnwfdz.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gtphgwetv.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gpsqwszlr.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/glcywiaqw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gaxxtwqla.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gmdtajfzk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gmqkygefz.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/ginzmzixs.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gqcxmthwj.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gjxwfuvon.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gmslkcoad.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gpuhmdarv.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gssyavlva.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/giibifbzx.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gnwozdqgp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gozfgnbwb.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gshnzpfxt.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gporqytrf.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gfycgrnuj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gkwoxeccq.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gllwtuxms.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gyqfyzotv.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gesgxsnpd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gilpdvffw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gnavzecwo.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gxevhdpdq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/ghtobqvrg.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gtewsevrr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gklolqnsj.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gbkwnerwx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gkolsxuag.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gsivlttga.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gzshxhhwd.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gzdltdaue.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guqcfiqki.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gjtzdlzej.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbcvekzum.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gxbdcxnpl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/goaupjrok.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gftgmaluj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gqqjxnyol.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gkaczmnbw.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gffhubtmc.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gnagiswqt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/glvwqxync.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gjsxisgpt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/ghoaeeyki.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gfpenwsju.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gkojbbbyg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gfndbxkyl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gyoboskyd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxkwxkisr.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gyszpckkn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/glkycxgxu.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gczlbcjbi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gmtdgkczr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtbxapnvi.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/ghqojxwgl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdvzirrgs.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gwdjwyoqb.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/geqdhuzxf.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/giijhnvzm.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gnnchcstq.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gsrfnartk.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/ghbeaiwgq.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gboaklefe.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/genubahfx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gkxxvmupb.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/glwgkymvd.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/grbueojyz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/glzcmihaq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gcxukzqwy.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gmlfxjrwv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gabmkcxvu.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/glqsfyuwg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gwhmilopx.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gofnbnfrd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gqbnjwwaf.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gsfjhkqtj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gzbpbquzj.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gnqmkvgqd.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gvbpifvqq.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gjikrhemy.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gtaafgbiw.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gdbnutidm.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/ghrfgmkqk.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gxarvyrqs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/guawiykvl.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/getadfcbc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gcxpcexyn.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gsknmuowk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gfdlrkhlu.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gbdphhtyc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gftytpsis.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gmlcwujfd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gmnkmtlvg.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gxhfjspsx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/giggoeitg.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gxywvlwbe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gjqkewnin.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/guumepnhs.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/ghghatkyf.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gmugqqpnx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gzvbpzynt.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gfjkpsdno.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gcoemomjp.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/ghofwypux.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/ghfvwnncu.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gsynanzfh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gvlonmkax.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gzclnqhrn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/ghnewxakk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gmedpyehm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/ggfukvsli.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gqqjgnzuy.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gajynlnzz.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gjpmjorxd.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gqrhbkgmo.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/glbdyemfr.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gcueiqtyt.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gdmmuwktx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gjoclrbtu.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gekhcnavx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gdtdrrugo.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gnphhorfg.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gdxomgppf.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gsfuxawqf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gdhidiqoy.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gpqlcfnyr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gvpulwsum.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gbyzxdkcg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/glxsybsdg.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gyzlhrbin.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/grfqylfyv.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/ghgtqczfj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gpptiqomo.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/ggydkpzil.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gnofcfqcx.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gxlkkktam.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gmkkuvtqr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gqexkibza.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gkqhqpwxc.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gvoxzshdw.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gjnbffzll.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gdokwgdxx.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gqpvqnxrz.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gmxbpoonu.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/goavvfazp.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/ggfyerykq.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/guajylaxs.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gwjnjsamx.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gqewrjtth.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gmibmfdba.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gscfhctgu.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gczqvwsyi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gcrwwzqxn.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gykvpyksm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gvaxdbwvc.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gaznowoak.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gnwyjmrjs.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gczdughnj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gahkaifmz.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gpnxpuvzr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/grovpjucr.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gxbxnbllp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gqnijxguf.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gplkmmlhq.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqhrmnnqg.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gxzxwnhnh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gtatadbod.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/ggygbhclc.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gbfndabzl.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gmiozdvkb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gdensqoel.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/guysaeylq.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gnsujxduj.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gqrabympg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gqjzjuayv.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/glmnuclnq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gtwqypewv.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gtrowkius.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gywbmnkid.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gzjgxbxqx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gjvqvcylt.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gyralhmbj.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/girxuxtdi.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gilrrqyhi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gnvzycpdp.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/ghueagosh.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gkumyitrx.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/guyuzqmyu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gtoftpkkl.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gnhigsmrq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gpddnwmce.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gfxxyegjd.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gcifzmdzu.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gfyqbxihp.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/glqtrxuvc.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gdkluelop.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gbhbyyxjo.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gmqteshnn.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gzsvleles.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gvxnesyod.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gojteoayv.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/grysglwky.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gwrcprqvv.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gaxydghbq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gddbfihhx.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gercqxtwi.sHtML


<!-- 参考信息 -->