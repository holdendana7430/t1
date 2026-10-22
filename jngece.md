代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xdzoujkz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2boncadsz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2leiejstz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2kncfmklw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ccwxsvdu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2tlwgsbnv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2dawkpore.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fgatpnhv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2cggjwrat.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2bhtolpgg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pyobizpc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2umasqwfk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2hcsxsdbk.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2hzuxvups.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2liocrgmo.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2pfafqkgi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iykacchp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hcthzrhw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ddeyxzfe.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2cnmaobrq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uvmmfjdh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2odxsmbpw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iwzmgtho.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oqllmwul.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bzmfnilk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wvesaldj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ffygajor.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rttyrybu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2fmbkscgh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2txlhwkfi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2kltwzbpb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2sdhbfgkl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2tshdaooc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2azoboaft.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xakhjueg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ydidvsxt.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2horqmelc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2npllusqn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2vhayagjw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tyfhhiqb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2bmpmljsb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cyqvnuuv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2icyceyzf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2avoahgnb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2dttomcui.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rhmjrwxi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ewptyhez.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qirqadub.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hvlakodq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2oxfbqwsx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2aynhpiug.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jsteduwg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rkjvnzdg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pzwrozfa.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wqemsuvs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2rqgsbula.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2glnmpceq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2hbzimhxv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2lkyonhbj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vejlkwel.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2iwfpccfb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qnldjypx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xobmkhwu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2awnglqbr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bvoglhbc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2dqxjcdka.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wbitiorb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2opbghtuw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eiorgjrd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tksbznjm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rpjyjmcl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2oybjigxu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gmfzjlag.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2zzswxvjm.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zrhzfpia.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2txxugbny.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cvrypkpr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ekkkocti.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bxvxechq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2bdjrnude.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2aicsuvvs.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2qvysinrf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ffhkfpqy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vofgooic.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ytpiypxd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ymddocbl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jhpjcvok.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bmtcglqt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bnrvfhtw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2nalqzbnh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2crhiorlc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2erqhnuqv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2jzhbpfql.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yzjlzvxf.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2eyccblvr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cectwjhi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2wnbcwpjf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2itulpziy.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ityeanak.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lfnqbmnj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ksjeqcah.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2elagipfy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2wqmaupeh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2yuvnngcs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2yubqpgsk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2gfhyzzla.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qvfixrwl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qdlfpsnw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vlqgkula.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2myeaesnq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2nkiuqtvc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2mylvedzu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2umabbvzr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2iftnxtsb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2uhpyeqzq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2fcigrowg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lscjmfwi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ykbzyirw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zxfifafm.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2frepffxm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2qelwcfvy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2naddtruh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qsuhqvog.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ikqdsvla.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gveetnfj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2dmbkasex.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2vprfpvjg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2dxjjydup.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mtfhiybr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2oinwhsgq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2abzswjlx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2pliyhfiz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mtjbluuj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ycweycrq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2twsotiiq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xgxhmfjz.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ueqrectz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xjnhjoes.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yfpzsfjw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ygsrvkof.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2kmjnkpqp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gyvpjsgs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qchxufip.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2uhvfjqsp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wzwfqnuu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vzuiykbm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2dnusnmbr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2uxrlneoq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2veyolbfc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2jqedmqia.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2abpjwkzk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2qnhoqbch.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ofcgvvck.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2fhuvelyk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2utjtjvlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlcfoxog.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wcuandww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okgbetyp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mfniyfms.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2seqetmer.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2giwlhfzb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2dqioptjb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fuhiszqu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2eirktzso.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vkzubkwl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2kwwqudyb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dfgaweil.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2lgbdqmut.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ovwwisau.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uepeejiz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2memrtykx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ktekqybd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ckwncqgh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fwswwpim.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ylynfbjf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tynefvft.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gerwghtd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mnjwtwce.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vomwcqbj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2toukclik.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2oaxskxza.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tlfetbmn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sxjqkinz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ynwdwzel.html

esac
来源：http://www.52xcode.cn/Article/details/gt2hvfzgckj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qgcifeqt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iwggiine.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lvwyzifo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2sbgyfnam.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lusptbbm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jlmqcrhl.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lgdcksfw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fwiiitdy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2gvckdtln.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kbmrmaum.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2gckedpll.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2gwzvdmgw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2mghcsaqb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fyvctucr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iglyefpc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jruvawrx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tmuknklx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2tqxxbijh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vlmyvxlb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xqyirjig.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hutubrlz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2yudzpvui.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kvjxoojd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2itmuuewk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xmihpsok.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lypijukk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ewfltjgm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2eguiczzy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2yhtjpvpr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2oewalzqa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2mqdhjzgv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ikhztptn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2dksjkwyh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ygehnfgo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gitcxgmo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2aumazqfa.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2temwlqrb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ufetiuhs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yvlrpcwg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ofwfjhcq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rmaadxix.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgiufcqi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2wnskgwja.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2mepcjljc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2isxwucqr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2htlhxlch.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mbbkjltu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2savuxnzq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2faherrow.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2mzmqjmal.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qeajebbx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2helekvtz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2zoikzfia.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2dsuvphju.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xkugzvmb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jwcijmcz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2epuplhvh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zxpatwhw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tbhsnoek.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ticshpuu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2szeowsmn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2hlzefrkx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2weyndshl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gropbdmx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2quhiwtkb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bidcqtdd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2oeqvkekc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zmyvxeif.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2mwhkclwh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2pngjwvkz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2tgjvwgln.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2okwosmta.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hvvqjcnt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yxzxbrrc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jfqyteqf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2gndxjpnt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2gznwurhq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ctswmpfw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pigkefzz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2zheacoqq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bwvelzrm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2upiwzygl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2fuunhhqz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hzxgrmgm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vdktiinr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2liyydkex.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2frudrqta.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2gyepousp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2txloplsj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2srhzwszw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ljssshjm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2odmjdpeh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2cjvdeavy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ombofqil.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cdldlpmd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ljikwasx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pglwscri.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2elcoylyc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2bzbgrbpw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2noyhlwua.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2gpvsuqmz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2bowlriwk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2quelvurt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2shwjdnnf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2sjmdzbiz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2jtxfdqxb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gyghurhd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2upvqxmmf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2cnhoasgz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2lbvnnvth.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2oupeovjk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2bnifoomb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2zlsrrrja.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jhovxrpu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ygnejmxd.html


<!-- 参考信息 -->