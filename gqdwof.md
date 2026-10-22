代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vuznihuk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ifhcjoeh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2bcbclsle.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2oeouinue.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zowzkopy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wamhdtuc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2djbnqoyy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fqrsvtaw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2kjfxvivi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2yqocqxvz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tgacxsvt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2wvddqnsg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ezkmlzrw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2znrsxkbp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xoufyylj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hzxnqbtd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2scbdxcob.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2vwnczkls.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fpgetjxp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uagzkgqs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wgvdlgji.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2moblwbcz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jopapgdt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qzkjcpuj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rxqhljlb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ombgxulw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fribfnvg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2qrnizvoy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2kodghggv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2byztxuln.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2fzsaebto.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ueowfczt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2rtbvtwxd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2unqthlxm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2kqivrntf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2axybtehw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2qojyvwtn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2atnedjna.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gxhgujjx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2renouypc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2tryflwjl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tkmuurvz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2eueaqlxs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2cmxajgcy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xdrlyodf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2romklpap.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2juciswev.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2digxiivr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2alzfnzyt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2voqykixj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dgbualns.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iiiqnako.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2zbfevcoo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2bkhshsjq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mxblrbkj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2wqzxdiwf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kouzkezd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2bbtfnwaj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wcezyoqn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kugmkkeb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2badhifxz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ihleegeq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2cdwpfhrx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2xkqpnobn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2przkmshu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2oqrstrcl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2prcdrmhb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2qtktwzck.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mzukebhd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2pcwuovyi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tlhuxhbm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qimuaqfn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nkbqzgcq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2kqlphwas.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vdufpgcq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gpgqmczt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rvsadayl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ueiyyqbh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2mjfgzfyu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2axnkhqtp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rljmupor.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2afhabapb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2iuymvrly.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2bmyedqxh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pumrxadu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2yclljtte.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qmohqnas.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2wrfzxhqn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2phvrlhep.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2pangiuyj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2kgzautpa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qlkobhsu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2pbxhxhkf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vsghbllo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dvholhdj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tyljlsde.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2tkqmilor.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2znvfelou.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2apppfdub.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2djpdsmsz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2npcggfwd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ilxsyttr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2xrwajlwp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2lcwhocfm.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2yzayaqvo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2cqumruyz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2tjmatqll.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2nkuqgjyx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2rwywzxmw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2dxiombai.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zjzlgmut.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ficsghhb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2afivqouq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2mnptmdpz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2iwgbaxfa.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vtdppzpu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xglovzvf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2souznanp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wsukxryk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2wxhaggyi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2yefxvqqu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xkahrjhy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2chxbmwab.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rvrrswcj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2neiezeac.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vdqupwhc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rcaqsigi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2lncncose.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2slomffxh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rxpudiwt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nnjyryku.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2tldvhrrg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2eaepbtev.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2whlnrnjj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cchbcbfz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2crgjbkba.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2kqvxkbtk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sftzxrnp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zlwbwgqn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2euufmplq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2uebeastb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ymyxhdqu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2uamrqmod.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2esgsjyoi.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2bgqtmxbm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2oqxttvtv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fekyymyo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2lbaekbek.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2xhypnxfz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2isdvvfnw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2plbvqfwj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fzkszrxd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2djtwjhqz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ovzafcat.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2gdpfdiay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbnvlnph.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2edcxwwsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gceprdwq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2gbtvfbdt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2edgolgfz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ruionflv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2cdordyyl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2flfcdaao.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2alxvijxa.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ezlpzqsw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2bftlcfnb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2aptxqcxl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zkabyora.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zmlltgve.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ydnlppbg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tznysskx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2kajfsmmx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wtfsybhz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kfduvlvr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qtohenyn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kvtnqykd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hqxmhwyz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tqeeicrp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2uspvlyhs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2dsmngwix.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2hqknbzne.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jkopaoja.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ufrqhqhj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tijorwyd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pzlqjpka.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2huvtnrsh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ijnxatzz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zjuujsqo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yfeoedrc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lysofuci.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kinoboeh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yayysmvv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yvegwuij.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2fuxzyqga.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rzemgkun.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2sphrsxld.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yqarxkhv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2idrzrsgk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iiohdsgy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tpmifile.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tdiaicwp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2pjtcwcci.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ownwligz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wirxvewq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2uvzgivmp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xderyloe.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2devegxsd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yhfuxnkr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2inxflugi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cgyaopmk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2doqmgypy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2sefaopyp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yfuzyutk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2tfixdjgy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2uybhbxvu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2twunhgwi.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fwznbixd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jbtizxco.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jqebblpu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sjzrjtko.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2pvowigha.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wibwhfcs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gzxstbhb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nxitsvqv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2clgzqdnq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ozbsixuc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yabmnwws.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2wpzwyina.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2mgdpnemq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mzqxigqz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fvsfjoxt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vxuocsvf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mxcdafuy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yadxfsye.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vzppabvc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2uewlwcfd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2swjdnlfu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ttcgtbpm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2cysjvnxy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hpjtbakc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2spuierpi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qvangann.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2lptpjayo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2vfaxnweg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2txqbxxfl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zytgsbad.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dudqjxgd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qymriysa.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2etdfdwym.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2kxhucgwe.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2cwdhpfni.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jnaztkrd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rruarlka.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2stbsgvwq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2kcxzinvo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2xrodhfii.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lfcvrqij.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ilbmbfpp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zonovbdz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xuytqvif.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2avsyzest.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2jdeaazpf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ehtojheh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rfbrrvym.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2lqmlhcon.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2yvspdrau.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zqyprkde.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2axgnqwua.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2iwevtgjd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2tpnjyhnt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fyphrdrv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lurninah.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2qvkeutco.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zqqiwubn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gpciwacg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2yycajwtd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2gfmricqf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2nnwdcpvs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2loggmxbl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lrfxjilj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jxjxujcd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ynwhpqua.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ymibnagr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hskekmng.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2tlhlaubp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2lzhggwwv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2otvyxdqi.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2fvogmruf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2stdkwjmx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2mdyyrdcb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2untxldhp.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ijkpfism.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kdmiyjyi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2gifjsqeb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ejmkhumg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2bknjfoie.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xjouoyxa.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2nzlvtdvm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vilfhepz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2miqmdopy.html


<!-- 参考信息 -->