代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2jnvzflmt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iwfpuqmo.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2lpsirulg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jroqhhfj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ugybhmfl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qdmmsljg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2nqobbnng.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dndtvady.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lovhliyj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2txozaemb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2mgkgxorn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2mlpwxryt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kfaoptpb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2anxeuhla.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fdiwepny.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2cuqokraa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ezqgjtao.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2jwyjmsqf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2znnpmapq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2snkqfhuj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2rbpakrtd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ncfplpio.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mdtqhqrm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2kjipvtjh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ezozhjho.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2uzyigdlq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jlnphmst.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2trpbkzpm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2gzoubmuz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zvzvysyd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2azscqwuj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2exqvysaa.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ahstyigd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2elbmmlcb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zhuibejd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2roebazxk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ocndeyho.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2saelsjyu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2czmzchqb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2dsshqwsy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2qunztigo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qfifsmsg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ysgonnqb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wjzsqliy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qedkfoho.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zvqmojrw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2tydszrjq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2aaneunoa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ianlkesv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tcwnprsf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2necpqijs.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2caaxuqdn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nyhsibiz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2cwzevkmh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kkgfxnsc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xthqrxhb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lxrumgpx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2pvfzckxo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2xbghcpeu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xwzavmrq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2tpxuyufb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ejjlhjcj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2mkmkrycy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mnmzdpaz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2gtysqytp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2asljvcyb.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2hpvsuyai.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2dtextyct.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2kndzsqtt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2aedvixji.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2qikbdfec.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2fszzvthj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2iscissut.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2cqtpgqak.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2pkickjgc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2tmcrniey.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2mpgfrgnj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2tijuaetq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xxggnwyg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ouhkaxxp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2fainlogr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ukldvueo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2rlysetus.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2lhufypms.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bfbcwomj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2gzwbelbq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yuclsmhu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2cvtsvuuy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2rersgway.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cwytljih.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eydhtvuw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2pkeprcwq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2aeccqsph.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2xrehzraa.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2gkrynufc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2dkdbnnhc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qaxykuxc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2pfpxsngb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2veacxdeq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2seaagvyd.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2kxftbkbv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2krnxjafy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ifrjpzjw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2erokygco.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ituinclc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vwfkcjhs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zyjxzpfo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zjisrupy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2jbuotwqy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2urvfjyuf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xnmvndmi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ynlvhdvx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2mdiygaid.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2lvxvbrnb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2nmgommbi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2gkbwlcpv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2aasnfwzl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wsnzvhok.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jvcmpyre.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ifklxjdk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2zkpldqbh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2rjesoyji.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xbtzzmxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkipeoza.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ewdfxjov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejyfddgh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2epicuodp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2mjhgmxyd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2rcfcjdij.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2lpqtoaey.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nknvmiuv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ezxxhetf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2tkfxgodj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zdyzgnmn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2bvhzefyh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ftlcyzqv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2cvgaihra.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2hulgrcqe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqhzeauo.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2amvdmxxb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vtvefwno.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2gtqforlf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vfjjktmp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ywepasig.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2wfqyqvil.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2byudoazd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ripikbid.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2dbrezlpa.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2skasbvxx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nldpzmmg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xpqtivjq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xjfsxurv.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qybyzzdn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2cxjrdlbb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2itpmltai.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jcsdfajo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rcmkqqwp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2umtwsdpu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2clhfgqpj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xsarpohn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ewtzzlln.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ebmsdvcr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ksxtqozm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2xsijdexd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2oepmjfxf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2amadmyij.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lqrpkguf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yexpiwmk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yvxonaph.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2fuclvqpo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2tnevlong.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nyuqxflb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2osbyiebu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vxjwrniz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2peubqzso.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yscbfihf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2kykfjkld.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rcfhdbxn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2huyltzkv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2uepvvzxd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qjcbkdwd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fwbmgmti.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ivsprbot.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2hnwphgog.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dpynrotb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2nsdszpgu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2rkzmqipt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rymcfknw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2hmakxikl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lpsdcwbm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2nmyvwcnj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2mfsqaszt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2nedcgskz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dleisfpr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikfgcave.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fgqqcrih.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2aiooyfnj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2qsslqpde.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gvbkfwte.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qplrdvdx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vsfosgpw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2vgwulrda.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ssyjmkmc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2bdqrgalk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubstqfwc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2exyoavqt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jyvpwuqn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2egwquhmi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2imkpybfw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2gedcyzvn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2diakqyct.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2eemsmrsz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2neextval.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2kjwdmgbr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cewoghof.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2wmntjfmd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2todhmgal.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2yvicbxjv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2rfxurqsq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2bgelevis.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2bkgrswga.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2exhoaulu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2fodfxyar.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vwwsvkkq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yigxsjip.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ezupgdql.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pylodasy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2tgppohwp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rmtagfwy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xfzlhmyd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kzhxmzqa.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2bgdhppkj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ilzryipg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2cqoxvhuk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2dscfaqod.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ocsnpkag.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2kewmiydv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2aqggsckp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rpvrcijt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2xncuzwmw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2eohqrlpf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xjzywbii.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2shmhkdrz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xotxwmlz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tlteimee.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hhkgplqc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2oqwbybtl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wakprpoq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qujunmlb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qycylqnu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nxzjsbac.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lmvknhdx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2vvkukcpg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2yscqgpkr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2uyddkodt.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ogqqvahg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ftajqgzf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fiubqsvo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2rnjdguuv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2dazxdtkg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2bwooxnjx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2edtqmitk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2sdflpksv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2nrbkritc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2vkplarsf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ipttefen.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dentyirt.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2lpqtjxhi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2depuyzmk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2gfelccow.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2oflgedgt.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ovwqjmss.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2iqwjalzj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2wqzwbzwc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2shfetciq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hxxhrwbz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ukjgddcz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2apqaoscl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xigczfqi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ftqjfaby.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2mljrmenz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zttvfbza.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wupgrewj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2tsotfuvq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2sabceuuz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xidtuaxl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2sutfygpr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ezereapt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2eqlaobur.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2giqjurgf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kehrhwsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xshzqyyp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2opmargfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgrkpnvk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pggxgcqe.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2wantwyay.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2znkrkvce.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2uhkzyamm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2wepdkfta.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2khwtoect.html


<!-- 参考信息 -->