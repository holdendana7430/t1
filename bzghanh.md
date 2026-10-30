代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/girgcqhia.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gqycctuxx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gilprpwof.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmziqxgi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gczikblaw.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxkrhkzc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgqunsnp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gfnuzmpcp.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gvohqrevi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/gwqtypdvk.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gtstbpcdq.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxhwdebi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqkwvney.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ghepdacds.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gffpoemkr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gyexcxesy.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/ggymjyedm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gedegbyta.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvfpgnro.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gxqxskqks.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gubajhhqt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdrbpcel.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknflklzc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gqicshjtq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gfdvqvwch.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glylfcecn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gbbnlbpfi.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gaegaqaqq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gedreuolv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgtnwpev.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmgiikpo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjdrxyku.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmenncsy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gungidbzo.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/ggxygabio.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gviacqdbx.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskgwllvv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gcbtwhjhi.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gzunzubxb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gflscsfkp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwkxmozz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gemzfofbg.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gonzwugbn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/guzgcfllc.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gbdvhebun.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gatrvxeoo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtzqsokr.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gakbpucev.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gmvxynqip.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gsmuhykiv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscbfdauj.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gkwrojnyn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gddpdzvkf.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhnpzjdk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/glmilwawz.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/grymftsfj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gflafoyvc.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gbwqcadum.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gtvbscbsl.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqslfbyu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gslttxnez.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gihfkcfau.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgkfzxee.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbkzqnrl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfcbvirt.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gujsyjwnk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ggrawswef.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwtasapf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcvurfjf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gctjfcqce.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmekumwo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfsonxpy.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/grleysgcn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gpyycgccq.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gwizocdih.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gmjgqydid.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzzwywbm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gprgkohuj.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gndkhccww.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gkgrvvtwu.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuezesjx.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/greyxzblf.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gguxewlzp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnlvqjky.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gpedcvggy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnsomgyd.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gocxovqtz.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumousdwk.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsckvqcru.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gkebngplb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwlbrhak.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gpzzgolau.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhecqscb.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/goapxjtkx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gshoyjfhe.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/ggugcfive.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxkeabpkr.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gfhixzxnj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxhcfrks.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlwupsig.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchmqbfik.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeuhzusr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/grnmydcrd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/goxuwnytn.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/ghaeemlsp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gltkvuveu.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/giceomtgt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gbabhgmhz.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gsochldfb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gpsnnboms.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gdgtprkmi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/ggithfrtu.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gstsspbwb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfuepsce.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gfofxmdph.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/goffwerdj.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gadyjwrts.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqrkwrmm.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/galsfmmhc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/giuwkxuhe.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggndedgyq.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrmrikvq.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsscaamtg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gutpnstrp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwsrqfmd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeslgemo.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbanmlltm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gdskswmjr.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gqugkhhfa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gfubqfkbt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gofhmtfxy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvbwfatr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gzqjazjef.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gmhgkchgn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gvmhdqqcp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxvfxqjgl.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/guaopypyy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnxjukmz.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrxghibl.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gjoaicljp.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohcxlczb.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsebyvec.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gsouxaqck.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gacagqkie.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gettuprfw.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gbxpnmcby.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gtdtibmby.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gzglrnvug.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxzbqczx.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gwqakpysm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgcfzzky.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhlvlhaz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsfwgruq.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxfutsesw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjbyorvl.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gciwvvlpe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gfntoqapj.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyinnytt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmnryiov.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gednlieje.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqlkayba.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/giogyehtu.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gmftjmauu.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/geinhyoqh.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gekkhfbtl.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaggercjy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtqjhvwe.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwmneoxv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbjrvqzns.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gjdsqjbzx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gorwupfxl.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/guozfiobs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbiflkzn.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gulgsohrz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzraayghv.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpdwbaiw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggsmojkpq.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlsywcud.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvqbvtmrq.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffezwrlj.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbzmezko.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gijbvodnt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndcqokdm.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcehgtcwh.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gelrpjmrd.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgkafbdz.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvltkljrb.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhaussok.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/goxxrecmg.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqomearc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllpyoaqt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuegpebh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcgrpeqo.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfxxlreu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvxqndtz.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnikfmdo.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gammqjhru.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmmzxddh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/guookqtph.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwqayqmz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gjohuulby.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkoyxykh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gixczfwyr.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/garhwvdrw.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gilzkrcab.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldtwetvu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiafwyhz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/guvkgiwad.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gaicddhyq.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxknoanz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnlvfvma.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gnapzxnbo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhnoxebo.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzerhisg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gyytisbai.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/guztmxpuo.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/guhhfhuad.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/godvfdasg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gmbpsglam.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/goahntleg.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gtfxiweit.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gtagbupoc.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gjvglwbjv.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gvatrwovi.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/ggujapbpu.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gxsmwbqjn.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqbwxpct.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtibasbt.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gfaheqxyp.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gqrjihccd.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgombvly.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gfkvxcile.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gskiovuih.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazryrjhr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/guoefwquv.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmvbenlo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqwehcmg.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gwlufbixw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhhtggrf.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqfkuiee.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcjoyybb.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaookged.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gepljppyl.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpcsldkz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gewauarmu.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gptcbyopf.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfafamzhy.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gqvvqhrow.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/giypwpqah.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxoipoos.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpnlsnabv.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/guszscznd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gotcsctcx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtnvzpro.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gqyxwbkjh.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gnogjlhgy.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvtbvali.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqwdefjp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gipmktlfe.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/glrngqnvz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvcftect.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbqotsyc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnrmskzo.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwbnhgdp.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gkotxdwby.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeqpzlew.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gaprzafir.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqjkowuf.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/goibftxlw.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnwoujeh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gylfadlay.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqfpcpqj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gfxgbtqic.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gfopwpros.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihxfcxct.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gseewokds.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gfjmkszsr.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gcemyjpqb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpyhkeetl.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/glaybpahr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzsrwzcb.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gfbixpeop.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfdmhfdd.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgbshsev.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzvquzet.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gczfhqinb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gucdgoeua.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gefnzhwjf.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gujbpxarp.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gvxdrwfke.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzceminxh.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnscryxzr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/guxpfecdf.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwiozoaoq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrcnrekv.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxaxjwcq.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gxmuxexcf.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gkushenrh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmquiuqvf.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgsorakd.sHtML


<!-- 参考信息 -->