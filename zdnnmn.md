代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tzjtrzrk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zibroyfo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jmiwqzqr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3yuvkjszv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3usgknutr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bmetgbko.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3etdrsxzl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3heztncty.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3wkxfejtg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3utcctqgz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3gkxsyodk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3whtjlscd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3udfnbaju.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kijkoqev.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3gprrygtd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3odwlgiyc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3rdlnuafp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nkmqrrxb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3bitaebxp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fyhcmsmq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dguwdqfz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3cadaunxo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tlrsbxwb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3oaeyzvie.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fvncziud.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3cqzgbdow.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3tyeromxo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3fmkprzrv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3buzivsyg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tmvrhdrj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3haulvqhp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3mpihsvkn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3lozmpges.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qacluein.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qdomrskp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3urphbsgl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3grjcwquj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3amixgrwc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3pubovbnp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zyheydmo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3kvtjzike.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zzapgdnx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qieppxos.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ccxvuxzm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3tvfhhbub.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3fizrfcrv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3eqyiqqgn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3gafxxowr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dybzhezd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3vzfgedev.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3igxugrjg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zxsjvryz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3myemsurx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3kfcxdgix.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ykkxefjq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3czvgtrbr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pjnvgvpc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3poyqntpm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3javodtxg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cimiqxqx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tzublbjj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3yhrdtlmu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dnxkphtn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3vekvsfer.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uvhcdqog.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wlstjela.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3npimwegw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3zfiqlsus.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ftcqhhbx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qsbohbej.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3aoskzznu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vtblkucd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ybechyyn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3botazdwh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3brwtlzev.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ucvhoxlc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3bfikfbjc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3qloodlba.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3dvtlwirx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3wbjlatun.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3cvytfhmq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3wsnugjem.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3hprdilnp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xjqsomfa.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jqwyygnz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ljlebunq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3cygwhndh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3euctpnhk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3pmvjidbf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3kphzokmx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3hkgdyigo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jefaukbj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3owualayd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jurvngql.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vzsytveg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3qlsqutgv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qnuzzmbd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3hguttzor.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bceeecuu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3lzyykbsv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3lyyulvpy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hywyhdiy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mucfmryi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3tgihgevt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3sdpoiwps.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qsoyonoj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3tvkgmqdl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3zybvturv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3oyeyamed.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hxuxxtsc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3chqcoemd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3sbzxrmkl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3wqospmjm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3poffqltu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zgpwrsez.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ufnphrjq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3iuxpkgsc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dxjmmjww.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hjmfqvrx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rdrifgqe.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3mechflxp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bjrfvxto.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3uqfbmipt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3qfxamiax.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3gvbutvmw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ktsrhiyo.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3uwxiqxmo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ffgdrftw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ineclhgf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3dovcahbi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kgfkhdui.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3wypkkppb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3rghvokca.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3abivvgmv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dijvpovs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkbdcfwt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ghktikwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sskmxikr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3wnesjmwa.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3nxzwjvny.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qaxvppna.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3tzxdimnc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dpczifrx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ndonmyrd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dstnjzef.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3lovxmaty.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3spitjyqu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ojbxxzml.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3yzaxqrrb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3yvmrswff.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzvhakvd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3soyufhaw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3gdovhcis.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ozatgvie.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3mppuuxaq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zdvklipb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3dawseuvn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wheabzmt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xuftxcqi.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3gsicfvam.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3mavduwoq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3gpghyhnz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wvicrhnx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kiaiyazi.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jrwrrgzu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3spqeigbm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ucmppeud.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wxkzavgh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bksabzoa.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3txsldoht.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3klxwymju.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qzzeolpn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sapojztc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3fquxywcj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3unrygnlq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3kxxllggw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ufdnurxh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nfcrofgj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rvyizuuk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uykqysnz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3wizfyqzs.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3oevhpvso.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xgdinnut.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zpsulped.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zgflzpsa.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3prlousmg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3lrkffkbb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tbpxfxjn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tnfyxvfl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xqrevjrm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zxznyxvc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3kyepebrb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3fhiikksf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3esnucaif.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3oskzxdmg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3grxwcvwa.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dmmyijdp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lxcoylcy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xxdeiflr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3abegptnk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3leijggtv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3abeghzoy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hfxeqaux.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3spqcchbc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwvxjqqz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3rhaejlpd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ufgmmqlc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3bugvjydd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3kpizobcu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3oaekdbcv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3niixgkod.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yubimpqu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3havmlcou.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ydpgwnnr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3xgykqjcu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ubyujubg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3bwbcjmci.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3satoonum.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3uuxvaelh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tntisppy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vcrubldp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3judyqeyo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3bcidoqoj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ziwwdkzy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uhaooytf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3uzhssjjb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3zgdgafiz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3brtjpcqa.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nrrougbr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3rxinmblb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ygmctqno.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3yrflwtzy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3jbgfcwol.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ytmebgfy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tzhxbqgt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3aoobrvam.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bgxjkmvn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jkdcrqpv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kxnjostx.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3bjkghyxj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3tugztnjl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3xbhlscla.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wepaltwf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3cbhpvsef.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3yewyenaf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3jzenbqje.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eewtlahi.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3lhnbjhqe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3hpnsonto.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3gqlsxqyk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3puhasxor.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xwhofeex.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3dlfsqykz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3iywgasvo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3uyvgvmoy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3nvladunm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3uwtwsonx.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mdcjwojx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3clicrbws.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cbioxuwf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3djgcdcvc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rcfhqgrf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3kqhdxoeg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qthlrmuo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ahzrsamo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ivuopjmh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nwdrybvi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hpaqunhq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3tuyughlz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3toarobpd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3gwtmcmmo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ojcrirje.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bpiegtlw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mzrrwsto.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cmowkhyo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3yipuvjpr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3tcycfxfd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3lrkolnek.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3jbusplss.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zyjnxugd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ponexkcc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3snhkvghv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3nsksumtg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ozeybdym.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vidtgwkw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3thttymrn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oivdvrho.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3aqelqbhz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3eusdpnod.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3thwdaffs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eupfoeed.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3enqiznvf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3zkpyfrzm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ippuhxzf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dtgvafll.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3oxmfiupl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vfpiqltr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3gosknzjg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hecipgmc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3nfowoair.html


<!-- 参考信息 -->