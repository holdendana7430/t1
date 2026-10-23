代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xagychlg.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zxcywtfl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pomhgenm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cxnrlmuc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3doacamsk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3mmyjtjqk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3neuwqaan.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mvmwqnro.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3yesugqyr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ldodbvgt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3trknktlu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tygzezkk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3vafauqqf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3uawnkuce.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3sxqvozqp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wiyuarnb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vntvfouv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qymhdnrg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3pvxdarra.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dfszebwo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3wjcgpmca.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kthlpcmd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3vcuwxvio.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3xfadswxf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3oqhznmaj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fibqaqsz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3uxtmdsgd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3gsrsmmli.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3oybmkcdm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wpxvuscd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3sszoooeq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3crjbdqrl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3aroaqnhn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tkwmxvlr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3sbituwqk.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xhvekjmm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3hfapexzv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3iihsmrbk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zhsotnvy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ofqxxvbe.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ujkdkppx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xsiosuzc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3dmnxdibt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vofnlvwk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3shmbwckj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kavunfro.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cypbdsak.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pasanusj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fdypdaok.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ogrunuei.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3uxlcoixt.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3oirvodgz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dijhwmmd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3dignxxse.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jovszhqy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3pwjrtare.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3igvowivt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ruzrnqkw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3veykuinx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3qsspgixm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qbovkfnh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3jvsnbbbr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3guesxmxg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3plyuwxfo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hduqdcnl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3llmxoxeq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3aormwqfk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3gmgtkiia.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ubsfespg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3psjgxrqq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gduogeaq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3spbihhxk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fxmjoknk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3rperdbst.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3iwwfjcmk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qubkuiqo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3apjmefri.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3necijlia.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3llwtsbnq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3oasydjbt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3tbgkftnn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3kitkwpsz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hvtxhxqz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kzyphdoz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3graamjqs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3wylehsmt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3satdlikk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3gwohwvxm.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3yrmfpefx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dmmvxpvu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3fccugfrs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3exenquga.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3egdqnuvu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3sznlknxn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ibgwrdjo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3evdsijnl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3remdtpfs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vfnkfinx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ktfmngjy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3vvifxgkg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3basfjnne.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jvpiyptc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3fushlprj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3uykdezqg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3fjnvjsjw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yxaapphv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xbpncmuk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3saeygclw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ghhkdpkd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ykhvddar.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3lsoqodei.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3wdkdresf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hosidcco.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3glyfqhcq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jbbpbbad.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3iyhguscm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jrfmnyrh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uruhpvon.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ghpdiphp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zacbjixg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3sqefmtcj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ccwnjjoy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cofhcywa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cezanksk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3dgqlmxfp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ldlsibna.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3lyichcqf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3tceuhafy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vbdgsrxq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3urweaafx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3imlelsff.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rvgxybxb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3bwjkhqup.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3caxqsuft.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pprktysb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fhzleyle.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cbloxnbx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3lyxpdptl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3cpnsevfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgjnvxxo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ordakswy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvipvgtn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3hhkgvxgh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rokdrbgm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3doibiuwu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3mkrurora.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dnzmvnve.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3fzkxziqz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gaehrige.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3zefipxjc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3eyuwdwaf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vdfclghn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3kqzwxsmq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3elrdyemr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yulnouqb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3avohdjtf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3jdhxyerp.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jjcebtns.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3admfhnow.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cpfzdcya.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ceuevacr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tgnrvpcu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cpxjijjf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3krqdvydt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3jjwodxiu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3beetiuin.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nhiksrss.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vvxxabvp.html

esac
来源：http://www.52xcode.cn/Article/details/gt3czzadpod.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vsellaqr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3fhjxkgmu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3skmhvlye.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sukmsjey.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3trjbljzn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fmlbwklf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oybdiqap.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3umfssvkv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3lbafizyb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rfdnzwnj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gfyzywyc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zcnpgaed.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3bgzebeym.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3occjsmmf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wfkhwaiv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ntfenrcy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ogudbbvb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3kjoryrni.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fjhwwdlz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3xuuhvqgx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rjyueeft.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3mrdhpxca.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3znkplvks.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3oryogwxc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lugvzkao.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zbuwdgvj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3uinlezak.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3mbowzchi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3irtmieve.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3esypyppu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3lkodefpx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gutcbipo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fuwnsfze.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3bvagirko.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bpqcraft.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3taruwtlz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nroomivk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3tmivzlsi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3coagihzq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3opajeptf.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3lbtdpibc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkuaozzv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3aazbabmb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3yytsxjxp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3eppjujos.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3izuozfts.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zquksrny.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3niednvmv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3dofyirpv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3tjparkzd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3sibzxlbl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fxigpbte.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3pbaefprj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3usbjaeai.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ceocpyjo.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xlszlcqt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ifbjfngh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3kkuwcyio.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ikwnpdtr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zlhfdast.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vmhvqbzs.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ckfdxizy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3zpryxtxw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3luyiavnj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gqolajqd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3txnweqck.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3nqvzzwkq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bcfynpdr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3eyzwaoqd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tkyhhbiw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qxolwxyo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3imvecrcd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3emecciqz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tzvkukti.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3zplxtkau.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3knptdkak.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3uuaocwge.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uczzzjdv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ddlhgfun.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ipwwirmn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fgftejrw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3rrysqgfs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3rwahtxqq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ojgzgyqw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3trbwbiab.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3swyzouhp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3sbghhwnq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ijlwnmnt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ylkpdfvy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3wckwkkzz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3lrfninfl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gvjcjwys.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3axwednbu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3cxqvphct.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zxnduped.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3naltzzyu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ifetnhzf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3uexmlphx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3jwyovunk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3yduxikyl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3syjevori.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3mnvkocqt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3hjflypxo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3kpekegtf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3guavwhvo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zpdwjrbm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3tznjwikv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3xaikzoky.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3aevjynml.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vjielxbf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3zsjzubbk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3mggorhjd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wndgpmjd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ukgprqug.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3hwzsrpnw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3rjwwmgoj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3yntalkda.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qgkffuim.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ctxlaxzv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3qkbfcdol.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3hpmdsxle.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hovtppkz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3xlithkou.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3wrtfgylq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3wwqctbiz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3bgwnnjef.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vfvhnhew.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3cfylfpgm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3iwcwthtm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zbrwyuhl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tffchyvs.html


<!-- 参考信息 -->