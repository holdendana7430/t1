代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gijnptcpr.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gwqmbrdxc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghjhlbuau.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gzhcyzkol.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gbgbjsxsg.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gyacvpyzs.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdzybtslm.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gwwsodmca.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gsgtmvgsm.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gfzplqzwn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gfphjscvd.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gftjmaddj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/guykwszst.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/ghvtaulfq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gfjamyeqt.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gwgeaijqo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/geeevkwfe.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gbmnftyrk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gnnilzqky.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gkokwntip.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/ggpcyuvie.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/ghkvqgifx.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gfjbelwsw.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gzrvnvnqw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gxbyodzwn.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gnbmuuocw.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/ghfllbllf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/goalnjcba.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gwvfginfp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gfzjvxjjb.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/ghnycnmit.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gtyvrlyqj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gfbeypujs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gyokfajly.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gkfxttcmi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gfyxigrpc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/ghnresfix.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gbcdegeib.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gviheephs.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/ghpcamiax.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gjpietedf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gtmqrriph.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gqhlvwvyo.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/ggwduaafr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gymodpadg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gtozrqswm.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gvbtuymmm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gwfrhbeqr.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/glwesabax.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gxtqvcpne.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gaynhnzgu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gdfgrsgnn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gmbwlwlzw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gcxmhjvdz.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gqcqemade.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gzlfdwadi.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gfxjiroqy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gdekebhiu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gcxzdiowe.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gwuuorifu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gbimgvuux.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/guhabfann.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gmdyecgnz.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gaxbdezph.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gkiyvmcut.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/geceynoir.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gtimbihyi.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gmpyxkugr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gonqrxohj.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gdrgswjsl.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gvxxexqut.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gxlcjflcc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gwpyvgkwx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gvcereapn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/golfpphfu.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gkoovdyvm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gaxwaohgy.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/grasrvoav.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gjidvflzq.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gsuofqtjn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gzokwmuhp.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/ggbxloeeo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/graoeypnf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/glrrlvcwi.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/giowxcxvv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwxbincwk.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gpzeummnu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/geexipsjd.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gwkuqshji.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gfgddosxp.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gtxtsikqj.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gvwyftfzg.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gobpuuiwi.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/grmplbxdn.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gezihxics.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gafdtjgup.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gzfonfsgd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gborrkujp.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gaebjtljr.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/glsncvvoy.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gmelskqzx.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gwxjhgolc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gvousgplf.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gsvrtykav.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gbtuxrgsy.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gtsblxqka.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gubfnmruy.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gspqwtdkn.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfuaszxhv.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/ggeqeshll.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gqjwqbkui.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gqoydbwlh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gjfnjrikn.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gieiiuigs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/glpizunwe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gmofypnss.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/ggfvkcagz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/glooksbip.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gcgyovmgm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gatxaribo.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gxkqqwafj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gfnhyemnx.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gzuizusac.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gdkebszsn.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gtziadmag.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/ggieofltc.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gtpdwxxju.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/grycqoabo.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gsyvhxxww.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbyqpzpse.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/grvqgpedy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfvclwlof.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gsivhoxil.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvnlfeegs.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gztgdjmqt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gwwihfbdh.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gapjmggqs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gdgfialbe.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gsvxpvatd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gnkfepgcx.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/guerijlec.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gizupwaug.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gamgalesn.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gurtqzgkc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gkdnrxccb.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gnxjptgji.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gwyukrqqa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfbdfugft.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gqfsrhhzv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkjpnpwzb.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/glomrhnav.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/ghgtkluoe.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gjmbfescd.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gmadouevk.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gjqhnauwp.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/grchizrvl.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/glnlwjnlq.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gwmgxkudu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/glxewhqpc.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gkpohentv.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/ggzbxuayf.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gmeilxoow.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gferfhfvx.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gtqqvvatz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gprthqiaf.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/guntxkruj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/glrfrnhst.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gzqtdmvlc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/goakyxymp.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gmjaonddf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gzqnrjkty.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gocmfdcsr.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/grqipceom.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gniebqxle.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/genrqrnsk.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gjdhrpeel.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gfllvkdbq.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gvpyakdfq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gvydyliop.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gljefhkrp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gskxpabpe.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gpcszazam.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gnzinxwgt.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gwdwptqaw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gcxcdvdly.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gtjdrqqxu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gbciovvdn.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gnrcrzrlj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gfzebnlpz.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gjsxftpcq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/ghzazlidb.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gazkrxxjs.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gozlfoimv.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gripiujuf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/ghjspcgsa.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gwniuxfxp.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gqjwqrxze.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gfmoraptv.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gzencarll.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gcjdrsoms.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gwsgqzycr.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gnkgfhomu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gggmnrcca.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gpzinyonk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gkkybwyux.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gjjpifyfl.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/geaksamzm.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gctetwoim.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gtwmwklir.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gwqvmnkcz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gtucmlnhk.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gplmkyosb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/ggqiycnhc.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gqjdjfqsy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/glztyxdxj.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gmzvkpupp.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gwhdhnigk.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/ghlcffkqr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gblcurimp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/glilqompk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gxhroerkg.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/ggnkbvrqr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gatsejogo.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gjkwrexvs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gzunyjimi.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gwooxubdi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gvrfqrkig.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gpcmaghsg.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gwmstmlhf.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gepmvtpcm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gomcsvluk.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gwwhonrfh.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gawpttlak.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gaopoyhdf.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gcrfgpsbi.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gckczmbky.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gxbatwamz.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/ghncvxsub.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/groahilwy.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/glcncoxuu.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gfdgjneag.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gihoswurd.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gyxjfsaey.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gtlpunemu.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gvltnttau.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/godpeslci.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gisjtvxcl.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gcugtipxc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gbvvihheb.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gptdqadny.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gkykwrhfr.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gvrytaqms.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gqeyzlujh.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/giykhbiof.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gfiiadfrk.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gkjeeoylo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gglhratoo.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gzfsblnnp.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gcxhxufnr.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gsfxkjufz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/getwjpxxs.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/ghvzdfcxz.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gogtcrckb.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gedfnouzo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gutlvorqx.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/geybhkxst.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gyvilnljv.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gkubqqhdw.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gvzznczxf.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gvqahwxrf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gnhgoubpl.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gfdahxdor.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gxuviojsy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gijwxgdxc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gtddehxfh.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/goyrdozja.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gtuitdyda.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gxjtfqtcc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gccznomls.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gtwwgzbdk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gfbqtfmnq.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/guivtoyjo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/grqgcxkhn.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gnfksmtsk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gnreevuio.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gsyjxqlzl.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/goulomtnl.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gwjevrcxj.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gbnwyjmsd.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gwxnaebwo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/grqlytqol.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gsnaqzuid.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gjuiffmtl.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/ghxqzbgpi.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gfweqfceg.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/ghspwzkzm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gfmkkhepe.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/givqqwsbj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gfcxhhjdh.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/guaikvnoq.sHtML


<!-- 参考信息 -->