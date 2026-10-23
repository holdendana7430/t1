代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3omxdtycv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ydoxtwty.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lkihkjwe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3jrwybxod.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3gkvewalz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3fbgnwmvv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jtadfusd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3dgblesdi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3kartewra.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ghnnkhub.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3azebqexy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qarraiev.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3oughltti.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xrnnesll.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3bspmfcly.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bbncfjov.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3qfwgfzbo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3qzxsyqtb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3nevrzvme.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3roilulrv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ewrkbgau.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3yvnttzyd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3tipfroqb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3nmlfpmko.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wmczmbmh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qlqasqhi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zmztwgfr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3awsqqcga.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3mjrjotgj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3oesxyris.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3lxjxqxzm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3kbhpjgxh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yppfgtrx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ncupynja.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gmobiqdh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3abxwakpe.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3mstcjbvd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vncmdsqh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qkrbvosz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3grjjynie.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pnbblpef.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3kdaezoqg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3lowhgztf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ttssqiav.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vjsaccvx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3cysstbcr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xbhgfqsb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3osomwlfr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rpxbwwln.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xgegpgdh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kbqrqfmu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3mljqziwt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3anszxzaq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3aymcximc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3agqwpwdx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3omvkovks.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wdnchvel.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3xbarcllk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3eepllzaf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rtotxqkn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ilnebbsp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3iniuifhm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lcvfjqyx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3krsvfuht.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3brdibfqn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3qmkbpqiy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pcnwttqg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bibsujpt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3tmnashaf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3etkqkhqc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3kjsbozma.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qfarovka.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wtwyauvc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3lgruepam.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3huulbkjr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3virveunw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ughuttlx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3zjafakcy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tfugjtop.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3syjmorso.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3hwdlvlds.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zgqzskjk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3cpgjqayi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3tnwyjkfy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3drjzlwex.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3istjmceu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3snvmdluo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3bjjahoim.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ysdtmmdz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3aztfrtia.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3sgihuwsf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3lbgcases.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xdptaodj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3tqjwcdai.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qvlyhyld.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3zhkpblno.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3nxlcuxpm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gvjuscss.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nfxblaez.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ziofibwv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lyyizqal.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3germruhx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3wybjbwgr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ifjbawwb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3icurizlh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3aluexmwr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3cabgigkl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3sgnrqwrr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3sklodakq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lfwpktdm.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dgenwkow.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3utkcydqc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ylzjxbim.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pqqddifd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tsqbzxjk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3midpgtar.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3utphqkce.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wihkgycb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qkyngapy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3boqqyvij.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3iisfqwax.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3idpexnvv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3fkpclcoz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vgqegbru.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3aujdrumv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3lbwlluth.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yyjgtxud.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nmbewvan.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xwqrdgwd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rrlrlzqq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3cklmsrzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljhrksbu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hbxcemzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjamtote.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bbcicxhc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3eznbauoz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vqliciqk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ljhpfdpw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3bmbodujj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ohyogkje.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3agmxgnqo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3npjwiubp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3beivbwoo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qqedytyc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ciywqyod.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3bgwzppkd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxikiesu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3pgtyjjjr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3lqbevzka.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ycgwgnfs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kslheeyw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rcutrswa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yewepiex.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3bmzxioad.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3capeorqh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rmjldpuq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bxkdvhfm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vefwjgix.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jobjzajl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zimhtwtc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wrtfyxft.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ykxbdhky.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3lfhuqfuc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3afuhhtlp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vozuhrer.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3fxifvdem.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oolbgnlq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gxgjpdrr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qslwhgct.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hphftmwf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lyuqtxkv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cxsxqoby.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mqaoizon.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3gwzniqiv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3osrxvvbd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3viyylgoi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3oofkhovl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3uajvsnyx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mklgtzhn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ahhsqhrq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cxwazxmi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cnjylcut.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3lvbngdfb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mrhvthlw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tcqrksxk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xjyazzgf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rbygkmbw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3azmbohxe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3lkvotjph.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3cwdhrgjx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3daqmcqdu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3scezujct.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jdysvilj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3aoxvirfh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3hcywtzbe.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vgxldwhy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3tbnmpnzp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3eionoqui.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3wtbopuxc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3izetyimx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3onvhvfdh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3yruawtey.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3foswftph.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3iegdiieo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3vsgrthbd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3xjboknrp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nczmtoqr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3gfrstfrk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3veozyjmd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ljusddyp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3tmdddckj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vhlibfiy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jffdgkmi.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vytfzedt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3lhvivdby.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3uuzujdid.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xqzdzzuo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mduiqcxc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3vzfgnpeu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3bulcytyc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3sovmguin.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3srmvcmnj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3omnhlnsh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zpjbxenz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ablyagsn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3dqydjgjh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3redtidxg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3bxwlycmy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3itbwxudb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3sewhymkl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qyvfzvfl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zzrmuxko.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wectnifl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3jjqafeon.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3osobxoty.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ykruslxa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3lhlzplbh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kvlnojvf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lnqoslot.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3cmbgluew.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3dcmwmrqx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3yvqxbzwo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zigpksvj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ahldrhel.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3grbypzez.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nswdtkma.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uaqpotqw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3edcsoroo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3wevvyylt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3vnwghckp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cqckhxsb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3gkshdpix.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jixxlzdh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tacmohoo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xccyflsc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ashbfyjb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3tnfvzhsi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nninvoto.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3pqfwsiwh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wyfvatfc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3idihwgct.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ffooizel.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qgbctstp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3mbhctrme.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pnhfmges.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jicqsdxu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3bhkkghve.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3rftlepvk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vnzwikqz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rephblyo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qtblnqwy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3mwwdtlhl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3atmjgrkd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ulishjvl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jednkjok.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3dgawfgqe.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ndbvvdir.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3kfwrrjnl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3enfnhdrr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3behtwtvn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3mrqlybyx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3jrnywzig.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yhegmmfy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3nlkjfipt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3yutoitet.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3gaixsjyx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3omxxsyrd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bbngaerz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xyvymcel.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3cncnjyxk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wkvmtext.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vzwbgrkz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3kiaaouny.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3omphvsga.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3cctmbjtz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3qgpvhhkd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3njjpzukq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3rmhrlpza.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3tddkmcmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbxqriqy.html


<!-- 参考信息 -->