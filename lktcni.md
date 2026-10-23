代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nzelcgqn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3fyimifzy.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zwxgbion.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3depayntd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fsrotvcq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3lcgmyahw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3evmmtscg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pxczpqet.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mgpdqsjq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3uluvfbjt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ahmxytha.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3kezrfeux.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3xkxefqlr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3strtxhwc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wysuucmh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3uirkyvek.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3tueourkl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3rpcmxdfr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wjpeudch.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kcymzzbo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3xmvogajp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gsslsqbj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3pjbrlhmh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3iyqgaofz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3dqtxnozy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ehxijihs.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3thwduzqj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3qfranfks.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ogughhbh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lvhddudv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ghxqxlco.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rgyppwmm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jqljogcj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3cezeoacg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ctftuvcn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3cilnozob.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3zsfovbrr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3jcfbmeiq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3amfzxkkc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qutiyihc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ozkpckcn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3tbkgtedb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xygpnhga.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ocmttxjc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wzmotgej.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ojjvwtes.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3yhgxpahl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qfijocgb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ciaceppz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hetckcwy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3akxpiqsb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3eounslzo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3kzjsefcc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3cnmnsopw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mwsablbp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3bbdcbsbr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fwbncrwf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3agfzpxim.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3oeruilce.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3mvzlcasu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3majlhhvp.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3fvzabout.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vidpfihw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tkykzhmq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qsqdeyfr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3nkskcxux.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ebbdqxak.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rddpsvco.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mhooceuu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lbgcbglx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xruvggkt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3nzfxlois.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wogbbxjx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3nbifzjul.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wkhtyhok.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3owtxwecv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uluiplbr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3qkzoaqmw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3idaiwlwb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jflcwkov.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3atuusodg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qhtggicz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3xaxfygfj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3aktwfegp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xevxfyfr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ujsypgez.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3djrmtbwh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xyqdormf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3dctlrvgc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3qgdkpnkm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3cmwhceaq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3saktrxso.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rdjmvvnk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dmzxllvx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3gzmdxcjt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3pglsdgau.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rybiitho.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3qbubabem.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ftmudwsa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3zjjryusx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zilcbcbb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3neiyuhwe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nifbwwcj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zwbnaxgj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbsupivx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3lviubvxl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jyrwnedq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3gvnmxhnu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3qxjlmpyi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hviovgei.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mhiikanu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3xddsgotz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3uvgscxyc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3pptpnxeb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3immxsxog.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3amhrcqdy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3nnpbohlt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3kayjwdtk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xrjutzgw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ktkouhvt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ogvkvmkp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tffsdwcb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3uiicwpxs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbxibtbf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3arqdplga.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dwoqdzaq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wgpkqzex.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yoczdjpk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3dnmrejpd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uezlobar.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3vqhdoqga.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3kxpnntzb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3cqyfqckt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ylbmlmul.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3uijsxpcc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3bgvyplmv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cexkfepc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jzpjnxyh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bewczdwn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vqlsepeb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vkdwcszf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3fiiqkasi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3nixrrvui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyuopfis.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3feimrqtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kuqsojvh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ebrkqhfm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3izjqmgqu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3jmleumhp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3cdkmsnfa.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3rvrahotp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3qhaicdiw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3qoylvqyi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zazrdykj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3bncyjdvu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3iekgkgns.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3krttsbyu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3kvwbtytp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmozouiy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vmgzcsai.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xptpkrti.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ffvxtgoy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nmjoypni.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ojrovklb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3bakgsrme.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gruiltvr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kjyjqibs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vtorjaiw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bdjhnbwl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ujvrnsih.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cqlitosx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bzilfyzb.html

esac
来源：http://www.52xcode.cn/Article/details/gt3dtqsprbb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3avvjtplc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pmubdonv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bwevlijn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cerbwkgo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3yslcyyoi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mzyhexua.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lowvhzar.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fpvufnex.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3yzqdrwuw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hhxdvvsc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3slcyqxcr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3whepqnbu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nvnlzaaf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3utcfempl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zcmsrief.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3usrnoskh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3kwpoydpv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3twlvczwz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yhemuklg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3dxrcvkyf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lveehbem.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jhuwlhqb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xtriwvib.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3dvenrhan.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zcwdxeji.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3gsubgtdt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ssnixvhr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3djlgpncv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3xjiqtzhv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3xftwxoxa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3rzhhiuzu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3vdtoytgs.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3hsclkxeq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wnndyssd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3smltpslq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dxcjbftn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3kzagntem.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3seoejvte.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ayeupnfo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfwekkme.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tcapximy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbzzchoz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fxmyyxjt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3cbmpybio.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xwzmlqxm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fiogradj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yixvnlef.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3yjyxlxgf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ciixesmt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3kouynvug.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vdiwvste.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mriapsln.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ekqdqvtg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3iohwkkng.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lfvwxjww.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ngkxlljp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3nzcmowlg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3focdbczg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3zbqbrujy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qmgmaymq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3sjlgeqrp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dogjegem.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qodhbeej.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3bshonldh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gdlnnukv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3oswxeakh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3porjodzk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zzrqzcrq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pemlalib.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3fvbnkjbw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3cvkmjqzq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ftualqxo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nkmdhbnt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3extjlaze.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ibkdbdqx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3dmblnpzm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3elgcbnwi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dpakkegt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3badruxoa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3nhkhuqpj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3epvjqrxi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3davxsdpg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3spdjpmbr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mbljwuic.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3hxgjllrq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qpsflhsk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3afnkbmdp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ucvaapms.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rnoscdzd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cqzprgil.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3kmsutsxy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3bnowtnkh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3begexebk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ocyqtney.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vyrxowct.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3mzecnvpp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nenhpbok.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3fymrbsoz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ixjnnjsz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3qjzffcyf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3rwyaqfym.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3rxspyvqk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qgozgzkn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hsggfcmw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3blhhfkye.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3xcodavuj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3uratezji.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3kkjiibya.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3rbtkxnxq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3amfzgvpb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3gdirusdo.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3qgzkhejs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3abkexgux.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jpgdihxz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3fzmcjjyw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3tokadngq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3provtgyl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3yelrucpa.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3udhcgiyh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xzyrqbch.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3lypimqmk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ckncfylf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3mkneeupf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3dtcxuqeg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3hfrznhdo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dpdmykfm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jtpitwhd.html


<!-- 参考信息 -->