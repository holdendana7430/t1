代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2amnsnvnp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mhbsskad.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rbehyeji.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ibtniztb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ogogpoiw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rmhwtycb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2knsckzpg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2tevmpanw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2vggxyqkb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2isxhkzkt.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aqqxnsix.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2xzjaczsi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vuvpbxdr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2lzbpiori.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2duoddrom.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zqmclgqe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ekxkaqbz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2qwxxbyes.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nouxouqc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ghkyyrif.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jttqouck.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wnlcpppi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ufblhjpx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ldscqmgk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2caxbvyqc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zztwwesu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2bimyqutd.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ptqsqprc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2avmxynzd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aumtayzc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2taygztqx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xwdybncg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zrkuqfse.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wubtztod.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2wluebcbd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qtgiswuw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2vmektukd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2zmgtdixm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2afvzljof.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2pjmxdizn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2oalgqmov.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ucmzpjgq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2orrkqjcg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fqduhgvg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ehycrehm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ryhvokay.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2svyzajcn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2dyngqwsf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2wxahnmph.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wgkemdkc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mwfdiwxu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2vsptosro.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2klywgtrr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2nnpkhmib.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2nqogqoba.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qqxwuabg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2hnufyomi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2etyxzunx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2zofgremy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2rdlanagr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2whwmuvkq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2hhsmiksz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ddlveyrs.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ptwjdbwp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uudiaccj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2bnmyoonp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2yeishtia.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2nvbptotb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2pjhfmtvk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ldgbgnkm.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tsodfkkk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2nmgkzgmx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tooptkoy.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2jthogcnb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lzjfppxq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2fnsbqgbf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ugljaorh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2hyxevrwn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vowzctki.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zotwiscr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fzcvbkcn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2wirbscdb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bdtcnebs.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2vjgwgvul.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ohuonvak.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nfgtpodu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2rxamhiok.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jyfttyiw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2lkozzsox.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2shcneswt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cbvgcvzn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tqfvzhzm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2rrfawbhu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2dvdokncy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2emacaxus.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2aywbdqcn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ymrivefm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2pmkotgyw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nwyanaje.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2gfvcyngn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2bjfdgylm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ooovtngy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ftchdwkd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2motimoio.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ltfpyelt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2sdeuorsv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2tojxqsey.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ypptrdoe.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mmobrirh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2drkkdxio.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ozzfgvon.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2mvjtmnxs.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mdsawnxe.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2cxjueihe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ulcldkjd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ibhfnihj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ifdlvcem.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2znyqdglv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rgmvxext.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2oeynnyvk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2qqkblpyp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2bhipemkb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2xkzrwgwb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2hlnajvjf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2oxppbjvs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2injzesxx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jtlcmyed.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2bxtikvxr.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jxquutkg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pawpfivl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2iiorprzw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jclgmxbb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2swwocaod.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ejljlqhs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xjdmyqmz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zyxpohxp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ahcbehwc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eoyvdlgu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2cqhodgwj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2aososuym.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2jmycingy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2eujwcmpq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vtwmsznp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2esurejvr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2qfgszaaq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2kigrjjkw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vownvjsd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dqxgculz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2csrmmfpn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2grgoedtr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2npmowjya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzrvnzcm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fyogzufo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2daldnpkf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xozhlffy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2fhqwvofi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2otfyvfpq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2hxtehnzd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2cplazete.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xiqxwdiu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2pujimtdh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2rjygvtfz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2swznubqi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yglcbbsl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2hjvxzbwu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2pmphlprm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcywsxuv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ymwcgnfb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iggdepmx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zeaknimn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2zgsfmply.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uycnssho.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2yityhari.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2lhaeziig.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2frwngizh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yqjyphbx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2usgcimgh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qyivufgd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2hsbnmauy.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hyfgelde.html

esac
来源：http://www.52xcode.cn/Article/details/gt2dvhkzfod.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2onwqrrop.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kggdeuya.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uoubpdmy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2scxtideh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2mnyaangk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cdnqwagz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jnyrjomo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2obqihlme.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2rfuxigkl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2emofbjel.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2uklwsvex.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tbjzlbrq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xftivsou.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fospibty.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jyrfvpoy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2toxeyliz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ruylkslz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cuwwolmv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2awdojhlo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2dhormdut.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bvaqdaoc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xrowzkpg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yttltbud.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2abhvcmra.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2feyjbjfu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cbcalpeu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2yyrrxziu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2mrekgaao.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2melzzkby.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hdpmynru.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2cxdyckgi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xixocrin.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ucjdsvok.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jkyyiptp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ftmknndm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fprtwyqy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yabkunba.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2tkqojuxn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jmitptsl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2grvlrwkh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jrgnxmdf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ldisvqjk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ngxihetv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2cvpwoxtg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2fglpjgrb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mnwtomcc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gwrtpiem.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2btqrdtki.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2xtmthuwd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2dccxqkvt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2pdjyyyvt.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2woziifpw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2uocfrtbu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2htynizsh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2yogegdps.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2njgwlshb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2dkrrqbcc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2mfaknqqs.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ssemthal.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vpcnvohc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2famrhpoa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qoatjikn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xgdevhhs.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mfrtriuv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2qtipgxqm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2twzflhyx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2tpdvnbrm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hpdcyavn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2lmbpascv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hrbdqeav.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kcsfggwu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iljzfhbm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2iaplqjba.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vkmdepdd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2vtpzjqcr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2fhousuny.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vdqnqgim.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2acdcypzp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2vgjrohsd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2onvwmlrq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ykjyqdqj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ppleidoq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2yijaqony.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2jdtuwgnf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uxidfrhw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2mcnbcsac.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2zhjhdtnc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2qsnphxbr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2xdbjrkii.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hwfkryhx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ytwgphzy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2yhvqxgmu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2txwxxgps.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vwrophjs.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kfwhtlxb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2sgxwxwyd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bsphlcyo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ofjrbsyl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2misdtdus.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2brlcyuyk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wsgoufdo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2orkokoxo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vfyhkgdv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ufooqxew.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ljmtjzgv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hekhfqez.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2liffmxdo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2tjlmuzai.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2avoekvhd.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2aeuatucm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2tgiyijzs.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2lgzwlftd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2bvqfvhxy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2amdktmqe.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2cplztsdl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xhpkvssx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hapwczai.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nwevftht.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lhlgswmy.html


<!-- 参考信息 -->