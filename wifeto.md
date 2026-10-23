代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ddtuyazm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hwxskypc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vcykypea.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tssvvkwd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3nkdugipo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3zcgevdbp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bccdxalj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gdmttrev.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3tuoozmsl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zfxoboim.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3yiksahoo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rahnjppl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3untwghgo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mjdydrmp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3deguwjse.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3eojmmskx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3suknzgmm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lnjsllqe.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kfggqbpw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3kvdmzach.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xlohiryt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3khvktunk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3vzemwixr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3pztnyftx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3uxamprqr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3knmmgwxy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3jpzsvpwh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ygrsoyrh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3feqntrtk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3hympbhkg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3wwizrwhm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ccemoczl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ychqrkgq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3pyypvuet.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3hqzkxrwv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tywmodrd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3wykhlcrm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bcswgxam.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qtikgvcg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3iitfxjzn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mtiiwjky.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3hezjjmvt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ytksgfhi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3emylipci.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lxdersmn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3vejjxybd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nwlwchcc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3wgvimyto.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qnvbdrcg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xpdsxhyr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zrzsadbq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3peposvcw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3sxgjgqsp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3hbhklguo.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3klertmmf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3nbkhlmtk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ssxoexrr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3uprvmqbl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rmtozzsx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3sxwuuuey.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tmnthusi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3evfzxicw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eyymqajy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3nechopyk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3caunqxpz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3tskbiobj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3wclibsfh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hmicxxxt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3koskqxlm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tinrpual.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3lrpojfer.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3oxeqykkl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ytnqbtay.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zoefwszu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3iicmnmtu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3nzuvxzpe.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3gngaqasa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ndkczknx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tdjdumnt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3vreniecd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tlajtydr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3miaqlzut.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3fpovjwjx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3tltymcfz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3kgvanlps.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dnwoliok.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3bbhupmdy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3oisfwodb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3fokqjsbe.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3fqsoinnx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3rhfjwwiz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ibiarglk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwjstexl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3rruiagup.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3lmeijpxt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3jdxqajmy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3wxiozvyw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pazqdpyv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lqbrrgso.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3obfxxvgp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vyblsagk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3oosnojcx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3iqezctir.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3pjamktle.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mkuoppcx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3xhnmkntc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rdpzawff.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3brtvatyu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3uccfkxtv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ufysdtzc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ykzvkvoc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qcvddcaj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nhxqhdqw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nxxdslzg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rgrfjghz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kvikvvqn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3giccsitk.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vpuzuxae.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3adshkhqy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3affelrbq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3legetarh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3jvgyctyw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ufiaxxhl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3jwkiprtz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ltmldgeo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3eculjfrn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3prglydzz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3epgjlgbw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3poltncgb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3cvkwssdc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3exnlnugx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkxxiieh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ppwrjajq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3luroweno.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3hlognndh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3hkrdzpew.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wbecgdmi.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ldugecxj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nncltmhb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3lnqqrqkm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wkhscmjd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3dpjgdjuv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ebakvect.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wleggloh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qklnkkbm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mabzctqe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ixlmajwn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3aycxnhvf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3egpbwquz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3biudavyv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3oxrwmeub.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ggzefkem.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cxswryez.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3flwwnjqo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3skwoeeok.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vwydwkjj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vbrytjpe.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3dxvloqxj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ljfnxprj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uaabovwv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3lbsczfnk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jcuzmxzw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mwmudtlu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wtccywso.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3keuvftdp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3mitbsbra.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3algrples.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3voerqvnd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3sxbdqagw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3kvjklznp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pdwcronp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3krkjuzou.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bdlqtbns.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xhfemvpo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3sibeyhvy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kbtxcqsj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fdotyoqj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3mqrjabmn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pepwpomw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ydmvftqt.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3uanjjtkz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cmndkpnf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3dvobhhoy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qfnmeggp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qqbgfpzv.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tizmnfgr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ikfpsbfy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3robwagxm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3mghowyww.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3lmwnalol.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3vvxblrlf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3tmbhrgee.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qxjagdnn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3tftkqnzx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3jisbyntb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rqjrqidr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3jfhhiges.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3diaezeuq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kcctorja.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3kcouluzn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvwfomzo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3thuyphxi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qayaxgqi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3hnbrkpcy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3uzutprqr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3uzsnippa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3knszorxe.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hkdpqinj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ipxrmiud.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tsbkliwk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3hhpftmyo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3pbaublwu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nycfwbbd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cullmwvr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3btjmpolj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ukzaqjuv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ogtglhpl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vodrawte.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3soeqdnmn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3dwysszzm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vuvbqjuc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3hmtmntee.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3foiqabhl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3yqyizgor.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lschwygt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jhhtbxhq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ijolydos.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3keyilegy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3gaocyfrf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3guooojub.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3gczoouqw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3gsogkytp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qzurvilg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ptwmxqau.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tahhubkl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3aivwzdek.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3bwafracj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3eheaigva.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kltfcpyf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lfnkevlk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3yhliesbr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nlccydaa.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yweruded.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3irbbauoo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3tthtgwne.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3skcadkfw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3skprjtpk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3gymcfvct.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kghxviyu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ixosnfoz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3viklldem.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dnnlhcyj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hroyoiej.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3pzlrggsk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qvdrgxrx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bjekiado.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rormyzed.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3czhlutil.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3phvmzheu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xidcxqfa.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xyqgysue.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vkklsiqj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3pdwzfrkq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xqvmegfu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3giwrtsus.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3falnhddw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ghhilayf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3elbmaggj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ywtemkqz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xfcdgzxi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3uzpcslnd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qhaxzkmi.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3oezqlkva.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3xbkdwzkn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3npqvdgna.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3yntewpfr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3bjjeuydj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3aoguygkf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mnqplbyn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sfjfcebs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gdvtnqee.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3wmmvqjax.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bzslddme.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qsasonjk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fcrmvqol.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3etrlobwv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ydijnlzv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3tmktsmvk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3anhjffnj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3svrmyiwh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hjymcqeo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3eyxpikpk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ujnxgsua.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3otyvxsqr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3mdjydzsf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3mffqkcxs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3xbqloesc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hshozmlv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3lfifybwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uttqleie.html


<!-- 参考信息 -->