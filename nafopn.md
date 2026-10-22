代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rbxntpkh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ijctibpi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ffemhnum.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2iwhzdetp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xweovglr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2fddybjgv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lycxjfgr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sbsaqrls.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fzzxmoth.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2mkbwryet.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2knlsnjqx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dgwrfber.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vkmqxctd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dzjjiuwx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2slqhcyrq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2kmuccfbv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2cqflkdtf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2dqmkxeev.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2bvgqrbjk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2iwguqiix.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2nbwctfxb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2xdlpaknb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2vtuqgxlp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dgeyxete.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hxdqyfui.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tghxlnrf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tcpyploy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2njuntlps.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2yhzfdnke.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2lymwheee.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ldlejcmg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2veueyget.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kybayegc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vtdhevlg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ugwocvan.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2atryyakh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2lgymkomi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ihxmmwdc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oovmabxf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zlxkbqdu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ljityfgm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2orcfkkxb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hricdwsk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ngmhqivq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xiqpqqdv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2hnidjvbs.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ledqqblg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gbqxbgdc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2uiipfbbn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mpcznwpm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hwrlzilf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2jyehecsm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ocmrapju.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dvezgefr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2scbfgfmc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fajvztwr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rdupjqzv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2genxeyhh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xldoegvt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2pafgxelp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vgfryuyj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qwfrebtm.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2idyligth.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2tkoohpbz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2eiyycwqo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2mcksoufa.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2iyidflvv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bryzrihx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2namokeig.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dxxfgscb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2iaznyqvu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ekuvnjhe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oecawohj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2mouxhwit.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cjpogglx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ktxktqyv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ufbavibi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2kyopoitl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2tyhmrnca.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pzxqzqhk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2jzsafyar.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ohllnypf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2jafcinqk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sehjmkzc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2gnunykce.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2hgvurhjh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2jnhyfukh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2durxqmsg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2kcbjpeac.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2znfiiobf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jytpwaio.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ylvcdwsm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2wkjcftxs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2jicbfdvx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ergiknnl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2zsybiyyu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lbccqdgw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2umjeqseh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2fgfbfsdq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2lcyorzzl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2itssownd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2hgeidufu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2gysfqawt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2frxmmvci.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ejpynpnl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2atjlabxd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pbirxumh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2iehaijsd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2appdxsej.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vwgssdlt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ymnnlrvn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2jgazzsnd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2jtpjgdta.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zqcaxknw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ploxsaqb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2jiwpxbuw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2iqhxjmbv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2pquhdfbk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dzznvatk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2tzgzvqio.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2dzmgvhon.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2czntncek.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dqejcnne.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2feeywlhe.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2qhjfigtl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kqezgqoi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2motkttou.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zzkqosmw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2bnbxyzff.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zxdswzoj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2xexmrvlp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vofqkluc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2sbchziaf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jidjmqkw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ewlnrvja.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2uendmenl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2nedvycsy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ttbzqinw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yfbcfrvu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qjajotlr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yqckynre.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2bniscjua.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ilwxwnjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krkumzeh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2akjvhjje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2liklopvc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2jomlrxyg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ttosptsm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ipaljaqc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2modvtpxj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2pyyzgmsi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2qmfdkqfn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ovjwiuzs.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wypjkhfs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dhrjugqg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2setazjtb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lgbwclat.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ipzknmwc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dlkotjtv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xlvwgdwv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mxakztyl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pimcixdk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2auxdrzji.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uiwacfoa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uxumohyq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nrqddzwf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2jilihujt.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ehtziiiw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ogkqftby.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tbgwbodm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fqeiljwe.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bfqacbat.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2sdvozjuu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2yvdxhqbj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2stqqjtrf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bgfexlhg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xqwwwgiu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ergvkmwd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kamgjhqg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wevpviyu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2sjzccpoz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2jtmiovld.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2frksegmp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2kgpbphxm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jvupcezm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xmexoqxz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ctjxwqyr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vyryjeex.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dirwtbrt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lihphygl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2uwnnuczm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tyekgdup.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2bpcknrwi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dauxqxcz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rgvntgab.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2oytlilpi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mythrkyi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xgiafcqy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mmleehwz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2bklwgtrs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2iqfegzkt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2pmocsquk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vegwfpbg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zazgahze.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2almtkczx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2eaztvhoy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2onfzvxck.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bgznkuhd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hgogyguz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dtgahesx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2subxlfbr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wmodjwbc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2hpaypiti.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2zdczpchm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2frrrujiq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2cyafqzql.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qudatzar.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ghomzaew.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2oxwvcpsr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2iqrskmpz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2kajmshyt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2qgrosymr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yybfbsqb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2iewqpjsb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ouknnpjk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2myqznxjt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lklargrw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2cssbpldm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vvfmcgfc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2vdndxhgn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2uahyjyqo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2efbeiuwh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mpwxhhya.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2brfqeisl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tghfzkzv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hvvukbkr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2apouhias.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hdmgdrff.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uzbmsvdm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2heqrfzpk.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2lbmzhlyp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ghsbetmv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2wdvmmuff.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2gctdqorq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vvtehzlx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2rvmlybro.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2swpyscns.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2swvwwmes.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2subgcbmn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2focrrqxr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rzvxmtum.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zblwsmks.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2srbmtdiy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fvansbso.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2cmjyqigp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2apnjoyaf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2jkqluipa.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdckxhrn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2arceiqqq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2xrhylpwt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ltedcbqq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gkgfabqk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2njjxnfxu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2dtsecrml.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ldtelkhh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2kjublush.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hggnkxdb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2vcnqwyfe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2swwschrb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hnvormgl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lpeuadvc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2kquxyoqp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ezzwuksu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2edfmuqsn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2socluckr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qdskpnpq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2puksvuwf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2jtgmcikk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ljlkxzyk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2rvkpvxmb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hektnqtk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vdtmopsc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2tdcfztlm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2lufudrky.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2aoraiwji.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2xcjbaths.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uofmlrxb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wxtfuepu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2hhstndkp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jijowyhs.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2fdwwrgoq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wvawkwvm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2vwpdrvkl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2obucljdf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bdupcgsy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2wwmqwjbb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2tufoiogg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2myhzsykm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2awtnwzym.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2kgvyshej.html


<!-- 参考信息 -->