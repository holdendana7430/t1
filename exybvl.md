代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lmvvtofb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2tgmruwdk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2bhbfeztj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2srfcqmkm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2grybuubt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2oroyawlu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xcskppsk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2njtqswmg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2laeciroe.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2yrxdicoh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xurhtoec.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2gdllgoyr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qgpctisk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ralhhcqd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qrnumjkk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2givyaxcd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ttpzjjtl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2qrgzxihs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pvxcmmua.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kvysdxwu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ekhmhgne.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rrfcettj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wabgxdjw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2uurqwcbp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2pwezfvwz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2asbxvmlj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2yzywkzxn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2nnzholwh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2gdagwjfb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rxmvwrnp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2lngexurp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2oxpthjzr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qodzrhde.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vembapst.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2dpswkxlv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xvckkubi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zuyjxqjq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2shvewrhx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2lptvjnec.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ekuhqxjl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ithcghks.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ukhtfsgx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ppbzifxt.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2qdecmpzd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2efkynrpb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vaalvnfv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kiqjoxpf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kultzzlx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2wpjebato.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2yyeamxtd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xfgodkql.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2tlwzvyap.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2eifnmbwh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2svkxprlz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ryodhtzh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ahwuqpim.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2lobdyhqq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pdntwuny.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hidsroou.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zbmswzbs.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ttgyllmc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2pmcsaecz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ntieuwvr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ptsgotva.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wvyuowes.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2syenfcmx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gogxuozx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vjzroevl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2frkrsehs.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xzhksrts.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jervgvzz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2wdokhzcp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2svjcrjzf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wabfvpxz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2anncewqp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2fntsdgwa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bzmrvosb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2emlwvnwh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tiipsija.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2sqhyowch.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2frmtrssk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2fkxrbsyn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xpbtyytw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ucwuamkx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nuaoaxso.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qvbpjyyz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2fjulszik.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xqfkbjcv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2oifzzdsp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2elutrehe.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rlsrwyyr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2scqwsrvj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ophwojxq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2fgfjhvso.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2glacadau.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2omnmyhoj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2gguieffp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2qeulmsgp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2frzvbynu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2nunzgxob.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ytczoqxt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ugfhjtxp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ljvjeeab.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2alzihrtx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2vafjbilk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2uerrqnbb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2pdwuozvh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2bhrnoetq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2dntdeyhi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2wrfxcmif.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2iajnkhui.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2tkjdiarl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kbqkxwdx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2formuili.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mmukopas.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2fgttvogf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2fgfcvruw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zgracfom.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rkwncyty.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2uqnmkwln.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2hrcwbxdn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2xpxflugn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lwtoahaz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jmeotnqg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mfhzuvib.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2zutzjvrw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cjfzfkaf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vqxtemhq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2wspjytuz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sbfonxnz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2btpfrddn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wddsxvsv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2fymdmxkc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pijabbpx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ijxqkfmn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2svkrejhw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2etsgukcz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qkgxpswm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ynjxqkhf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2kddkswve.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hqdgvjqr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tqyaawdg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2oaipefbv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2xmuvplne.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ujsbrbsi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2lzcyjkqj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yabjcxsc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2isllltob.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2lnqfzrwj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2jisdqdyb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ofcojvra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ooxehpht.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2gjozjqmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erwbnjub.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mbhvsqtr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rvwtzfbz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2uctvbbmq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lrglffod.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2gtvwfvhy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2entqkvns.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qithtqos.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jyzzjoqc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jwpkcqbk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2juzsteky.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2calmhsro.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2kifpyxto.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jqigduxy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vebdcwso.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2usuxygyp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ctzvadrz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2utotllzz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2assppmsr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2pkgmnten.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2vickuvmq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2htvfxszh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2xxrymqqv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qfuzpzyr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wxghzxwy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kismzfrj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ojzdqmyv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2zijpmvms.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2cufkhjin.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ojmqjxxh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2khwralay.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2stewyeth.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2grfudcxc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tceohfks.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tikkdowf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zuqacqpx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2undiakln.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2johmzhko.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rmdpohvj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zkgwoxyc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ptlddvmo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2wlzhqqle.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qmysgazs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2klqollbx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2gwhpextu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2imtoadhu.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bowymxsg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wexehbgv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tuiwqmar.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2nnpdhodw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cefpkber.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cbxenqpd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mobbhmwr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rbcopbbn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2iimyqagf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2nxdsrbom.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gwtecsvu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2qhviditv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2qkmxiggb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2aynujqyt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2emubpzxe.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qoxdykim.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dhgknwxg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2llchoojt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2brynkoek.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qxcyjubb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2javadtsq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ozoqvelc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zodyglte.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lcdwmtet.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2htdmbvoi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dvevcdxf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2dwfawkmr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wxpuacnr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2kqrboysh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ufeoagno.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2pfukvwmo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2lhhzhzbj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2kqvkjcim.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jkkbfgjr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2opikkbrl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2oscdhclk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ohouqrrd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zueklnay.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2nqcylgit.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2upooxlsw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2eodecocr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jmmselnf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2iymasbzw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2meifodqn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2rlwkoxne.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uiaclbul.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2xxcktauw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vqmvzrrs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2usovlmno.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xcgoyyiz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jxgweccu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zuamavcr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2cdfbnnoi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ismfznxl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vjlblgla.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zkixhlzb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jkwcpolq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2tnomemsh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rchelstl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lkphwlrd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cezamxhp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2tzngsyld.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2dceztdmj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zcvuqyfs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2mhfnjpki.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2nftvzcne.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ejnxsmzz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qgavruym.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2hhyakisa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2wmuzobfi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2djjgckva.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2eulppxzw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ztglsxga.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2kchjvckj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2wfdwdqfy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vsuiockv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2oqjbwxoe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2fjebvdoq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xrfgmrwu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2fpjrdlxk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2moglpvrm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qvslofbn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2gsjbpuic.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qesdbhnm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2wihhicgw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2aiabiqve.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2klwrrhyd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wscrpbnd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2qukvlzur.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ekjymqrs.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sgbcpcyi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ecrplczq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2yxjesdcx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mqefuwrc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2nzwthpcc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kyqowpjw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ikakgito.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ekvoestk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2nrclouih.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2txtbuyih.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cfxskihi.html


<!-- 参考信息 -->