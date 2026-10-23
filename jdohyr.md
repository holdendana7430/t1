代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jzirvafp.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qmsevefo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ubpoixdk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3vinueyog.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yorkcmlr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vnmgenux.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3noiwurvm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3uhwjcauv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3yhsaoklj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3kbvibafq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vmcahlzd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ijtjfhjf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3xbiygqhf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3kszkrybv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3mkkthebu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ziexvfnt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3odpdlbmb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zjxdwijs.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3emkwllho.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3cobqqobx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3tyqbafjp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3uzpbsutv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qgczxdhl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rmibxdmh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3becvvgwn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3jvcynzuo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3minegcrr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dpqsmkyw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ppviifmy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ewbocajy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3tjcexavv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3krjblemj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3djbjadvx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3szpsyijl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ljmqthdi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3pvevkxfj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3slscfqyn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3dklixqzi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3qxznlobg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fpcmthdf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3bydkgent.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bdpcemtb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3iificzsb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3xtwqdzva.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ahotjhhg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3svuwwthj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3tieftdbz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3nsjvwpyr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jreaebzz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3gisnxkil.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vvcrmwqh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3fbqtibfp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3wmcjpzws.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3coaolrop.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fyokfuph.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3kjwsfwpt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tshptysj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3oslsmwga.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ntnirazz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zdhabfan.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cazpkyor.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xakzbtbc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ryxjqiot.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3zmzkrtmt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rcutsvov.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xyfdvgsi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lqwpprtr.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ehwhyqot.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zumzyqud.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3uqmbalpa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3aeehfgca.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3igcrktrq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fqiliclm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ejkfjpvw.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3udeqarnh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ggwqsypd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3sbcahpxz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3yjtsrszg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3amyezmpd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3dtlrtwfp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3twvgyfyj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ciyyjuvv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3prssmymr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3julauhhv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3hnuwnlsb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hrocaflf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3qxirmbmm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ecwymxmt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gpffwrpw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3swxkqdob.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3wwxhlrjv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3vzftzqgj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3romjqcqo.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3gqgeogyt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qxjeziyd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3padnujxs.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vhjoglml.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3hfaabdqa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3pjhbocqt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3khybuxew.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3wxafpige.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rnfskxuy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lmjeoptr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3wwiqewvt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3mvekppxz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hjaoshxy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3rvoccnzy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3riabwjip.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3nhcmhtpe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3xgmvjrlj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3nbhiaewa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3pjilfepc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tbpnxweb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fcvsyfdw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mefwbovc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vdadcfmh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3sxwyidge.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3omirofeo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ixbjrrhc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3chbineyl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3czmsgwgt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zopxgncn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3xpvyxjkd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bbgwyxrd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3wvkfifkt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3uajaqjdf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3npaofrtj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3fcutknkc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jysltuqp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3vuxllvcp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ewqpdvvo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3uijgedug.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qkyktmqe.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xjmcxbjh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3iaklehaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3geubzloe.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ohzafliu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpyghyer.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3nqhrhovy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3kjxtkafm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ztpmgfum.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vacegfre.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zrgzujbw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bedxexfa.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ptijhklp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3paoiqrkm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jejhfitf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3vfjvtbhn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3tpbxtfyi.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qgssrxaq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lflvgrcq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bcnuqfoz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3wrmekoqg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mytdnppm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3duporyye.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3criyufkt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ssamjxta.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ckbevnce.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kbgtumau.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3uzuhrhgg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3cchqjcjw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zeqgkeov.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3qgabdhmy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3bvtlskca.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vohioysp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3lmvjwrgj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bftxuqkj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jqjgbtcx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ghdesaqt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3tpbvbddn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fegusqdg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dktzadhj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3msrfutbs.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3rrbyhtix.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hbmojetv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3pjuqjneo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vpasjtnn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3zaomfghm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iehycvwe.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wehvsfmd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3inynjnta.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wxnsqheg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tqvggygr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vzxjuxrq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zevseojy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wlcarjlz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3frjohcat.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tcbiydch.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qyodkbbr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xcrwesrc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3aaqucwea.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3sxzitcmp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jwyaksan.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gnxkkmkh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3smtdnddq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3yzlrcklw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3iongfjde.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3aymrbctg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3hyvdixkp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ehdqcncr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ppkpikei.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kjoshvhd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3bnmeadjg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3utxyrgvk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncyfqzkh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3abeqclbo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lcqjkczm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3bdhwojhb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3sykndtgw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3tlxvyupp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yxgzhore.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3uaiefyob.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tgfmktst.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ucqdozfb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pljyxiok.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3bbluebuk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3jjgffhnx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3jurnpxro.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3myclfwhq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3akvafjuv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fcflsldg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3leplxdqz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3xebcjgvi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3nrzkwokb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yzqerhdc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wcieqgha.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ximzdgwi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxaldrsm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3iabegebh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3zcwddvob.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wttxcmqs.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3bswjhvqe.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3uqzzdqpy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ybypwiml.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tglxdevc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3sqxavjiy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ichjtldd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cqernygi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gsmcajef.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nghommff.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cugdsmzf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3mncohpwt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hxivqtnr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3udkrxkhh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3qzwhglpy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3kzpmztxv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ordprvgd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3jzulouqa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3tfbldwkk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvgifpgm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3dxbisaeh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xdgzwjmx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3pwqqozni.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bmshddug.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3oeehptif.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3xipjiitp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3tzvllaiz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3clibefda.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3aucjgziz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gvtqqajb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3lvuzyckg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kupogdkx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3wgijznvy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3zbkmfcif.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gkldqfmy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hcbbgalc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tjdkipuq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3khlbaxni.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3nywxcyjc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3droyolga.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3uekiflml.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3umsoyzkj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rrwjunjn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qqrsmwwd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wzfiyqag.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3gikoyzmr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jnpnkgjc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3lragsbnc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gtpdbjhb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ppoaxfkt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3lijubkvn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3wtitzxnx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3fknmvgyn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3twbmgjdo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3klqdqdou.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3lcuazimz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ibynsvtq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mpvwszfv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3wxwrazwj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3sireyzpb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jplgoehh.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ksuhgtdf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vtgdfmsq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wmlzepdm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rwvejmmo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vghjqpni.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ddmljsqk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rmayfdmc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vkwuzdvx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3vcdyjlsi.html


<!-- 参考信息 -->