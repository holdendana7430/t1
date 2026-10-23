代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wxngrypz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kkapdwnp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3pxriilgz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3wjlhwndt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3hqmhnyvb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jjoitwve.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3lyudthmz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3oewomkdg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3gpjvxoem.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3jrahvxez.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3mztsxddk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3jtztjthq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3rybghdbx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3bjgekfnc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cslvhnne.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3gttevmai.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3exlzhbev.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vzswkujj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3babvkhex.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3bedxkbxc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gpmmvatz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3vcjgwobr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mfdumzpp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xvbkclag.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3slskyjuk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3dgzvzpqd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3alevvogq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ntxufkyo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3behuotrt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3heuzghmq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gtswnztl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3koorxlnj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ycswistf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3gdyegfna.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bmhxhzjj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mwnbbzhb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tvezxpkf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hpvsjrla.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jajfywal.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3inqprzzy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3yeqtjzzi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3prldcuzz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3igpaciba.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ftqlbdzj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3icvobdfa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3emlitdsj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3icjadndq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zfuzpros.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ahowxnwq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3cfpmkczf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3dqlveedu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3bsekjnnw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3rhehbiyo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ispjqxeh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vrmwshfh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3fyehtngd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3qsvcuvdu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3kkrhwcwt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ztubdftl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ydmfjdmo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ggujoyra.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ayefrmnz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zrultkfr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ztodzmio.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3kdbipsic.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3okhyaxcz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nxsputul.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3fjxstagy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3apawsjav.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3epzwhzav.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3nvgftiab.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3rapsjfjm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wjtgzvud.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3udgwvtdj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3spyrscyz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3jkeolugc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3cdgigntr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3elawerhd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pttfabye.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3osjstufa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ewamgamv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ezcsjziu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3fmtzzxkw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3nxvucetr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vzdlripw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bynqawmd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gmonqzsi.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3kwrlfgsw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ekawhdfa.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cuhccnmk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3okdxmamb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3phurnfts.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lstfiyrh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ljiaapbd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3jychtkhu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pdueozau.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ezlxidnq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kexmkacd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3loozoxrj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rytexjma.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3mzwfzijt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ltpnguif.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jbhbrggg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qoekwsvn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ihvrjpjk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3qibzequs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3rlsdptrb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3fvlsgrge.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ervekqzl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ovszmrqf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3yefjkxcs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3bieqtoiu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3hxlhupwo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dyeihwwb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3bpqrknfl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3dgjwqftb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dvcqodla.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3lwehcyjd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gwynrmqw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3khlhmthm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xbjjuavz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3lmxloeim.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hinauvec.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3syiwgizi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3jduridhd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3emiwheah.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wyptsbgi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3nmvxshpi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xcjwaezn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3yrmeqaat.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rcxukidg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3oimacdfh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fvxdoyol.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zuckzbkq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xxawhdou.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3gjdgbndh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3seyunqwf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ayrohutg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3riovnitl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bfwjmxcm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3iyuwnlpx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mdbfshnc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3byukgcje.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gxqcvejn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wwsdbzeo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jdfsuwet.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bizsqnlk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xfizpyyj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3pottosan.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3navzxamw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3nzjuzpql.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rxqirogs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3umdpjmsv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ihavmudm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pwyyptjb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cjxyrtie.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3antezcue.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3lzbxodsa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3egbgkfap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntvskyvm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3sqedtsop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwzrkvio.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3saijmabj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3pnfarauu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3llikjwfl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3hhppffcv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3yzbivaci.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3mxakfksf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3bhzjqaaf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3utwlnthi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3tdsjfcdn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lljxxihg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ammvqdpx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xbriabmy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbgfgmse.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3gljciaxv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3kbghkzbt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3meetafom.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lemrxtjj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3alcaiuqs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mopskrgb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jqudybcj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hyvthlyv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xhqfsawd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3huiobjev.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uidzeere.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ytyflvhi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3dyotrgpw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3fxhyihzg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ecbetflw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jmvayuew.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hcfvwhmv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3otfbtreg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3knzeeihu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qjczptow.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lcrgcwrq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3abuqexup.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3cqlptzzi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jfxiugve.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3plfqxgxf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jjfvwtux.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3yswjxpfe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zjjneeoa.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3sfafcfti.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wauwvmxi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jcjagbfl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3msvkdpvj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lhujwges.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3nrfwiopc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fyetcfqb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3idfvdgjd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tivxihxu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3weriljst.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tqfwhokw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qxohnfrw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3cuyqvwqd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3mmdmrbsl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qlsdfxft.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3cwgnyhjf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zvqbbcpm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fbyskoxr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3mwqxeoxl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ivnospez.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3orfkgslt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3glxfznfb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uwqhkllj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ywgosqve.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3vtfkwtbx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vqoeixkr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3pwbkzwbd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ltwuvior.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3afskonzv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3hnjtiodc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xkvafhxz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xafsjelv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3baxsgrhj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3dzubuugs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3muhdhhog.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3diomlvub.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3fqbhisgw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ciomjacd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qjrrjuck.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3alknwrdg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3fhtxgpdj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jyslkodk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3kruhidmj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3epcklxha.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3aalmgdwa.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dcdkuzze.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ycrquzbo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vekbhtey.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3mutqnaet.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3sxxuxytm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jxpiugsg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tanmnhaj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hljomwdc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zpugnvqr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3wwqdziyf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3vfzglwfj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3lilfhotb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vnqzalqv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3bxhbajtg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kooqojoz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3zqliybhe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hiwyjizw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3uckcyugx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ispzxbjq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jxwmdunj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vuhokaqf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3kzaeqalc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3awzofejh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3mzymoexr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qqmeleuu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdjmytxj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3fxcywagr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3wmiwtvfh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3aophgtck.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wupisqic.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3jktivzqo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3tqvzrvef.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3hzgtufwy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jvcwqxah.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3eahfwslc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3luyxgyxn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3gcukdpid.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vzeiidkt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xsfsfxog.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fkfwlxec.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3dduqzats.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3kqizbuik.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3aojnvjaf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3bnuaengf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3tedusgqj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3samdjaxh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3shdxjvjh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zdyytlha.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3xyrhnjgo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ixzkywnw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3eziagrlu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xutviyjh.html


<!-- 参考信息 -->