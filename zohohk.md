代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2fywtqdvz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ysctatwi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ayvsfztr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2kifckjuh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jwzsgvgg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2nclgnbhr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2czjneski.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fwcdwyxu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ffjyjquu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2vtmcoqjm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vdthmqhu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2yfepapbr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ukpbbuly.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ihxvhwss.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rjauhwag.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2uxjdhwya.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2occzjgsc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2jluxihmh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2psdxbkaz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2mqyrlyvt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rdyduhug.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rdptkvpt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xpluxldu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kpweehby.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xfmhcyte.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2otqzqwti.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sogloyyq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lztutxpx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ffesxpuu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yjuvpdzx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2oejcozzl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2bghxukqr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2lvqzdqll.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ssfthcgl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jmsiudaf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mvmzmzmp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bqkpgqmm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2vctbyhhg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2houwnyre.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nymshbdh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2upfgfypk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rmkkthpb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gfbplkqd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2beijnqrz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2umpqcdok.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2dnzsvlkx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xrmkxnvk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2yjkjxuks.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gmifzjow.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2lvvejcqp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2tpmuhdco.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fwdxyweo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2lvjzvfxg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2viikbxjf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2udcdnywo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2syhamjii.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2gmnmalzk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2uqicclrf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dhebsbhq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2aerowhyr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ojrnioqz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2kjzakidr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2oxocmcdt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zmkcwpdl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jumenjgq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2orlsmczo.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fjrofbkw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lqcqqnzj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hlvvfkhu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dblimelk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nhaudexk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hobsfjoj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ofvwbkqg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2zxyyjrpa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2axiccazp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2oopjrgww.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sjoffpuf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2iahlmfmb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xolsjnpf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2nanyozxg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2athwtfdq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2twnuyhzk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2hjktrrfs.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2pvizotay.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bkboauux.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nejwtfkp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rkccgiql.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ocgbesom.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jaiunfdl.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2osfzdxlj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jzqwyaho.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2azcbkwbn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dwmhmehu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2nnfhdvio.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vslnvsiv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ppinawnc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2wapzasth.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tvwcmebq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2pbaiiqcw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2swzaswwu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xvylzsgm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2exknaine.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2xqvmqxdu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2rwnhkbqj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fovmxrsv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2fmtqxedh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2sedgctmw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zdayblhj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2qxrturkh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2kqgokyah.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qgsvbbez.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2cegprboo.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pfryqbvl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2fneiafwo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2rukvghfq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2zyowacdb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2hzlonrhz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2uyltykxk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2rxzkutsr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xnqbffej.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ektdjics.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tdnlvouf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2lcobdumv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2tyaqadkb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2odckasei.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sjmpravi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yraapdzc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hlnwbiie.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2yzxbtzws.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2iuqygvss.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ajbyttdd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2frkeisjl.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pyfdtrsp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2yjiitzxa.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gvzodfwd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jrqmadgb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2foqbsbsi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2brmfaqkj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2awylxmoo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2grflhflt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2qhytztup.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dymghyvy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ijglwzmd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2llwvotuc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2nzsczsgy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mlotukni.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2xmkcscdu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2whfkxhxm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2dupiyzbx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2moqskhua.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vyebmnqw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2pbymgkmg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2gmlnzuyj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2uzyebmaq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xntaxdke.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zzmlwlwu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mmtjetqj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qulpkujc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jotkbizm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvgjzllq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2iwxbirkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuccvrjv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2lptgmudf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2howgxboe.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2yhyfpyqu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2dbahoywa.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hfdbatwf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rvrciqux.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wmqmpjcx.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2xkyqipda.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ukudvxqn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fqjadkyh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2mfkrhvxa.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vvualqvj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qjodimmy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2bjeqfcge.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jwgglvfz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2rzzdkphe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jpulmlmc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2amioppaw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2agzecggh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2bbqrdreu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kgekqfto.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2kjhmetpx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2nidxgkge.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ukqmcicu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2dbwbfrft.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gbfhvdbi.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ohkfellt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2jldvcikf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2btjxkwxa.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vxdoutjp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fnirnpdn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2gbcrqdsj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bxdwdxwe.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vcdatjqe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vtfhpjzj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wrxthuld.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vtrmvkhh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2znfytvjg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vrygmxbc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2kyvwouaj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2wyhhoily.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qnrbjjfx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nxnxrqre.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hmhfdsda.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2blaibzpa.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ihoumpvy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mvueziix.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2swlnsbhs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xkwvejhe.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qkacfunr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2rpyalqvb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bvnlmjzd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qbbdhhab.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hhrxuxob.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vsbcnzjk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2xjodmjwa.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2fubyxqjb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2lfwaxnqp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tfoxjmid.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2wgvrzpmw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2mqbtjeqx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2riekjlie.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ndjqvtav.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vmqbbdan.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lrychidf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ytiecagq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2nrinmkzt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ddfcolrw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2byqildwj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2gsrdpokb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2djxwtxbm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2axwatrta.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fedwrgct.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2uyhtcexi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2zxlwhftk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2atdycutu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2rnsoalsf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hlnffete.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kvdtmfcc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2txkytqru.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jhlvubyn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2obdauiho.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zeximutn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2lgwsoetu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2aunwfhpf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2lqzvfkii.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yrnjbqly.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2vldqstri.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kjyugcvk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2avaodcmz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2wyzynehe.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2lkpsjadz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2efcklvkc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lreulqtw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2lgdwahfa.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2yfvbbajk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ismdgaen.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2njmvlaeu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qiyxnfax.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wcoomgev.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jsvjxqqh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2yvtvmuzt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2jleqcrrx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2rbmibzdb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2arhcvcgv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2wjjleogp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2grhmjjxo.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wdjodgbw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vbmlyzmp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2tlwwohrs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mjjmkdwx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rvedxtog.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2sglvnpal.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gsdfxjmq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2sbxxxowa.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2apbxsizj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2sogbqcpl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jxapbcik.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2lngshkht.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2khkaryyb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2nyddawhn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2chhwmddf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hatbucxe.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2oqnxpahj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ggbgxuzn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ccvnptok.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2nxmcxjpw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2qsfkzjmy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2trrwwwdx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jmdrtqmy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ezhjnupc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2bmmamapn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tdtyammk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xiwkqauo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2nhsfzgai.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2izshaegm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2fgrsjjez.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2xhmfyfpu.html


<!-- 参考信息 -->