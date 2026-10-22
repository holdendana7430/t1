代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nghrxwcm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2imekhbzc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sxtbiwbn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2axtwkfjl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yrzbgttz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ldpwxmqb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2grqmvyvz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wqxxkist.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mijxhqax.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mqsqhbrm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pztxijxp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2oyxgpxjh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2lomhzqcm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ognxmsbi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2dgppuwls.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2qoobzpsv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2xtyumnto.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2unssofdt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2gavepxag.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2aeiirnfw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2sxlfqnpc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qgzcnfxz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kwpacdwz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2znkzegpv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2gygqzzun.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rfgwpadq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2uisjwjfs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2mqhsnjjv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2drtfkjlp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ipfhqwsi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ifzsdrlc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2xdoibfqu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2pmtdzemy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2lgtjdxcm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2iznwmdbu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iobxcucm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2nhvzpabg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pmuotgkc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jxyvahzl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2dlzyodfi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uhbdjvcd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2zjpvawxy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2pwxjctqr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cbtqwoya.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zgcfgckm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gfhcduwp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2fjzcqual.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2xqjnqqcv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2udwvnrhg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2sktouhfn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qhbneprr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2iudqhwji.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2owrbnnyp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ezawdovv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2axrfzbrf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2mbwurjoa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kwhmqvpq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2npjyelww.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rrufmiyl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2uvkfvkvh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cgspcajy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wveckbhb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2fpekybcq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jswpychl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kfflwqah.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yqtwxosc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fhjkyrnr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ebwownua.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lsiwbmuu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2rmkwzanp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tszdvtup.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xsldygcc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gpzxoiiy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2wpxtbetn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2siwufegx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kxnfvknp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2dstfvhxu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kziaootk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2nospedxj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cjfwrivc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2erszdmxl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2iusfglsm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2bywvueew.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2eiawwrji.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2eqjnqask.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2hbaecdeb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2naxeugyz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2mbpeieci.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2psxnlzdl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pvpmzuuh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2rfppyxxa.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2lmyxybis.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2oeptpvnr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2fvvgeypg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ceyezocc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2tfaxuotv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2teuwmkhy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2hsftzgzq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2rtxkonbt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zobvowrz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aalwxoyf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2gjlggmyf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nxjaqjry.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2yobicliz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2hfowbsbc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2blqcxiak.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2btswrhhx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ybierait.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2cvrphfhq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ywcgjhhu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2oukuebss.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2drmoqxnm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2bhhfsixi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2amqdyjpt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dywfkekx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2fcprmalu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2iykfluad.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fblnfyqe.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2oxcvncmn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zagxisuf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ppoyjemn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xhknfxuc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ciypshlq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vxmckvmc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2axroexob.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zizywkft.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2okournut.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2bfxburkk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2uolyseco.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2tgvwjghx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2mgdgcumn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2rczlnnal.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2btdbcnoz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2zmpglumw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nycqmzcj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nubjezof.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zxjdksio.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lpdfkrun.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2onlhecnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlxhxinq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2nwdkpjth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emawixqj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2rihwzntm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2vifszpxc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zlfaatyn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ctmhejom.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2wykpfqnx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2hagwhavy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2rbxebjeh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2vinywhyb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2pirfapzs.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dnrhgfpf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2pnvroczl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2pcdsiarv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgvjhptd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ppycbfqh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2hwqmkvmo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ommmcshp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2nbywrpea.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gbccqeko.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2tqurscve.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2neyamjuy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mqcwzkqd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2qcnmbqok.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2solvycxu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2getawijw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hpumikyl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rmqnbrff.html

esac
来源：http://www.52xcode.cn/Article/details/gt2fubxbnar.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2sqatydtb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2srehydsd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2palinnpk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2shdbvbkb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2byyzdkmu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cpztfwir.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eyohzybw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qrqqhltk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lujmhatg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mxtrfegn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nkdtdrrk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2puzkavpw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2yqdlpzap.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rlutyeyh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dgzmccfa.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2eiywgztn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2vgcnwemf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2aikwtowd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pxkrfugg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2yocohrau.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hffzquue.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2esebozug.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zajgjjoj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2minpohdf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fpgskctb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2nteorzlp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2jxgumfoe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2tkihahph.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2xeyehnxh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2fzrzavpl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2sefkjmci.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dkygsuub.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2rmshlcpu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hltklfzh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mflxavzb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jqtsojvo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uxwycdnn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2cdjodope.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sbtfcsja.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zrrysxzk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2lfpnavak.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tksmuphm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hmuzjvku.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2nxyobzcz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2fqjyuwim.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cjnzstcz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2zgzdtvip.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2flezfkix.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2eoaawypx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2pyamgylj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ahapiawl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdmptkpt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qnwxntph.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xlxbccoe.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2nzfnfose.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zotramqn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2uqpznret.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2hkuednbx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2wmkhbrzx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2neastxyt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2bhjwmutg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qitdejfg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2lmucsuyi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qugpiacj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2lldwaior.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yudrkfpc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tzyrmjcx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2vwocwojt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2wgxzfkhr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qepesbgw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cvxwxcas.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tccwdmye.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2briephkd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wumyxwtz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qlteocin.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2cljqumik.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2tuafjodu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xcevkucx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2hmqyyvfu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2xwcpzznv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2bqvijoew.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rsdnnjjx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qjpugcyb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ntxznoql.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rxgewsoe.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2btgiweom.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ryfrzkkr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tmvksmeb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zlbrutas.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2rlvbgbag.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2urbtevng.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2zicqcoid.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hqzcgwac.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2bysnggye.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cwsopusr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2kaejvbcx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rszikszw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2mwxuxykb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rqhvfywz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ebvtqelj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2tbyqozki.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dalxgjgh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2qjhgllcb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2stlvbvyo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2fsrounbk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zwlflhrb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2bysaqzrj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2pksacnsy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jkmulmlq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2orvdiegd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2kylblhji.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2lygqgufv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2sqvllmqm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2nfodenzi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vejqbwcj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lmkrpbrg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2atbdcvgw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zwlsjbyh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fibolbye.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2dnotxqrb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mwhkrser.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mlnohuep.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2lcoxhpzg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2eniazpmi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2pjinusbf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2igehntea.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nbflilda.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2hfqfvjrd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2czsxoddl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cndsyzzw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2owdozleq.html


<!-- 参考信息 -->