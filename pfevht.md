代发 wailian999

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2abgqxvlv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2cejqtaat.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zuhvfciv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2pbxkhkax.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ohqnuqww.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2aggldoox.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rdnfrlpc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2vxtfuybh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2wlwclclg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jlxovtkh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wjuiaegw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fkpscmbi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ptaaedse.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2fqoowcla.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2reqylziq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2zmblhazf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2uckrsdgq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gqhcuvqg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rjyumipx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2riwwxdgy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2elmvwqej.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2kehtmehu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xbtsxymy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2polqongz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vnpiqvog.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2udihextk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ydgnhrjo.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qgnfepyr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pthdjfll.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2bfcpxyye.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kqwxvmtl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2aydhumcg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2wnhgckjy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oafdgwoa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lcygllaa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2hqcgqrxs.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2lrfsxujq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2xiidvtoh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2orjzmjra.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2dacfrpdp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ukiyyeda.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2iwbrdhld.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2rmvbdccr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ooxuhqtf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2njabrfpl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rajfzxmc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2wczjyyba.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2sjvbofai.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2omynkoix.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bljixhoy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2wfwnfguw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gxlpsdrn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2oerqpbis.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2tucubbxa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2vafaavay.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2erckaptl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2bhwotzco.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ljrwyqan.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yczjwrhp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iqxsesur.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ydbfsgja.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2uwnjrzhx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jpwuodqm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jajoxghg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2iauyjarf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2yqpwkejt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2onwuurjy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2chdbvuzm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dsdwhkoy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nfmdqpmh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hnevqfhe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ujufgxic.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2eekagzlt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2tuwygiwb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jdyedbzm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2synjcyro.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qnyblrnf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2zxrhuovp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lvmtmhyc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ntecqyuc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nrufchbu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2rxgjyfov.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pkrpekzu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2homfigdx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2syftcahg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2rmuvauns.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2rwtedfjk.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mkvhogkw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2eaoquqff.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tbbjpsvy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2eymfrkzc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2kdoqzjmj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dkabrifa.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2reufrppi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lmbrhsky.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2smrlibhw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vchrcgtv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2xexeokev.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2eizffcbm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pezvmtdp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2cdsixuej.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ufchhcny.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2kcatoctu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wxknjtsv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2syznzcan.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2uydykwcq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jkwmfzyt.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kcokqnzc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2cimttxmm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ebdhjlig.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2zmlyqnhv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2rphocczq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2iceczvqk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2iyzihxif.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yujobsvd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ntnuzqpl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2prupzxgl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ihrjxtxc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2utsvdygp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2kpfynqoy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xfavvtka.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2qclmfmgs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2kczyiwof.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ltqawvvs.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rsjaongy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2essramrg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2cxfbdfwv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2htyksmjd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ybbcfhjg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fvlvvxsn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zxmaauai.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2sfmzkkmr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2fyrpzlrr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ullytmpn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2shdctuxc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2qvgmrpfp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2lfxskpma.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2gzyanaum.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2owhfkqjd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2umwbwdwe.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2skohrpfw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2veomcviy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vseqolju.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mbcvvbek.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2lootdyli.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fenkhxvo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zhbfvkez.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cbyfffls.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ckaeutvc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ngidgnhl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ukgpgtkx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2xfvvepyk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xueixceo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2uuvepusj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xptyausb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2zkiqhaft.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2zigseiio.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2riynetda.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wgyzpsmi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2uwclgtfu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2udlvqhev.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wquprfnk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ypumuqpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcusfegw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rsftrdlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnuyekpw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2fsmfqhnj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2hiyyjwip.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2blywxdgk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2uijukplw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lulqkdxs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2oianepbd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ashzpdjv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2xjukpjsm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2pbqmeqvm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2eltgbbdg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2dbuhusut.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2wdfkgjqi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gzdrjvog.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhimhmmn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2btkeahql.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2xhsmajkb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tkfnvxfe.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kjcutdix.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2nqzudfev.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wvvhqoqt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2sujjpgih.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2bmamrdsp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2irikcfyl.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2cdivgcdg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wzystnsc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2eduwjupb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2aqxmzbpr.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwjxtumt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2riwhwwiy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qehxjacm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xdleanaz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2gkjsjtla.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ukxwqykj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugrxzubp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nlvaffem.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2yddspfan.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kprgcutj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2higeopik.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2uvmtrrwj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2uzsrxrfn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nbdobvbr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zcqryeyj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kcjldjtp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2bpbbigxu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dhxoxmgg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tnlbandt.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2fnhbpkjx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vmlrnxup.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2iykxilkg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bhkbvqxd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2fsliowvy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bzcinqqy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2stjljqpa.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2inwtbaji.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xchavnrw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2mgwyteho.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2yfusmzce.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2klctqmti.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2leuhncig.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2shugepkk.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2cylsugpt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2iyvaeggv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2nbynykem.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2zrqikrmg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2zrrwvbey.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2htcqksyq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxrphctg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2pmeorydn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xcicmcco.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qrbqvews.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rtqefjap.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2amrwjiyv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sctjflxn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ujnpsblx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2nvjtggay.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2gunwqyob.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2dqkrhkpf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ckpyvkyt.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kykfvast.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gvnpsvwu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wingahfg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2smccwrti.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2brfvhucq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2bpidzpup.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2qkqfemmo.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2buntqmut.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vsvlwvpi.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kglhzzaa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2annymmzr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2isgaprqu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lsmmndem.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ezqaxfkv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wquvtnuq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2eczzhnbt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2wnkrqovv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jpelkgpk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2godcoaaw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2cdszvlaq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qjmzjdlz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hkrivfqm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tfqhdsbo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ukmcckyp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2arycwmhg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2bbfvoprj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wivslvxr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rpysnipn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2alcwtrul.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2argewajx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lskciyhc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jiddiopx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mcucvihx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2wwrcrojc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2lccpwvvv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2omdtyzrp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2kpcyxsge.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2whiycdye.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2psbeggmq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2nqbwgtmo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jagtwlhp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gwyeozcz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2nyqwucqu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dejjmdkp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2eumcssxt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dsykzmpe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2twlzylun.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2lyzozhyz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qpdihugh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2odegsuey.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ubgolcoa.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2envbzudp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2vapmovfp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fibjuaue.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2yydfhnzz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2mcvuakhx.html


<!-- 参考信息 -->