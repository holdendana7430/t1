代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jxxicjnu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3mbjzbpcv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3aeqsodkh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ixqusgqd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3cezdosjc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3pdhktqxz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3zkubbmmb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mtrnjwry.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3uuhesjzi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ivxomtsu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zlvycssg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3clbcvrky.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ihwjbgxd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3oebzaina.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3izuxtnnw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3yetwrjts.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3bkkcvwzb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3eavivotw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3wtflppyw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fvabhkmi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3adgovrai.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3agfldnde.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3akvpgmxi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dwapxzwi.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3usigogor.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3dntrgjfq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3amirrefz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3gxaxxwqt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wmuhjibr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rciperqw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3evkolsuj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3eixuipog.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zszlhcyj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tukemhki.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ydonyike.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3lprinujn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pqqzrcdw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3mvnbbgzz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3rgvnfsln.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3uierisda.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3smerhcyr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fwpcddep.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qsklmwse.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zsukspqc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rqurfugl.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dulazhaq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jbmrhils.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3kqxmvnyb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sukfloel.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3eeshpwqi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3onhcvckq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tazkfbcj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3mellssaz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3luirbjgw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3huzdoory.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nbnkuqfv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ahwcggpq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mzfmqvev.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3mzoptgqe.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3arvpntcf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3jbsstmuh.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3mngbdpfv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3wotjcqeb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3imijnvhw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3mlhcoaoy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3orprmcgl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vcppohke.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ffmslyjw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3eygwbmpm.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3xlwdfgmw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3blcltrra.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3hvyiedwt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3zljqkedw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3mbkkmixf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gpbnpvxa.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3vvqszwzz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hjaufuaw.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rieowfcq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lcutsgiv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3jfilbulp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3cpuhevjn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rdejnquk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fmqhiook.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3prqbfxgq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vvjdlghy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3kbjgsudj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3lbhlvrpi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3zdpzrmzp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zjolcqaw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ovckcvhx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qussviqk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3qvolhksm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jgasdibk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ziqphbwg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3efpnfcgb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sxhbekwl.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3btakylne.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vmdjqbpi.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nbbldcbx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3inegrvbc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ubuxzqnz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xhjzfrmt.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3exadpaaq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3sbppmumy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jypvmpsb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3kpobcsys.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3mtgnmzqi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3aelasplg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3cqcrcrqp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jlffwxlq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3watrfuxt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3phpxypuj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3feambsuw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3locpdgth.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3mgzoayco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgdguldn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3yietwhug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3filvtlya.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3tpiodqbe.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3itvkdwmh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3enojntww.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3acgkdjxr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vrikjiph.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3uwivbiux.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3asengzyf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3vywsijjs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vkpzscbu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3udofnmir.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3mnadpmub.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vzpazmbe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dkcawkvg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3weomgkgf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3horuhwxh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3setrnddu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3bwbxlikr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bfxuctkw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hzbekqln.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3runanacm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ztwetqch.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3lmhekntn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nmcvozdw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yewyfexn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tgjafqnf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3fwenbbhy.html

esac
来源：http://www.52xcode.cn/Article/details/gt3gwrwlvdc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3vgfntccw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dgglpklq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3btcbcdaa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qnpweulh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3phkmvmxw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3whyfzpil.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ovsvjsbu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gfusbjgg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bkucfphi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cyfqanuf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3zfuekfjd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qgysgtex.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kmdaxpsu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zalwhbbm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3heddfzjh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3aclvrdjb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zrjvawrx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rscnpklh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3woulfrmn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3evyuacvk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kxjvnmdy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3tkdgfgiu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3omdkhdjv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mhuqrkja.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mupnqrai.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yntwetar.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3pjbzkdue.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3xisqmygr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3dgydagpb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3eieobpqb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3eqakuvvl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wyszkabb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3mxodurli.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3xueovuki.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rtfcviie.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3oszdipex.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xrdlcnkc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3patlxnlm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3yuejazdl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3upgrojld.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3mjrfrijz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fudlexul.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3hmpazine.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3bopqmqti.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mjovijso.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pitcioar.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3kkqvzxep.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tcsdlqom.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3yyitftzy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3bllsheoi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3otltyuhv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tfeejokv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3eiarfpit.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3sntmdkmk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wscuwzmo.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jyrjgctd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3qywpijlw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3kxqewlyo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3twsftsxr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gcxtmadw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wtsaqgau.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3stvrmhxf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ceobfwzx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3yuyjhmkz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3nhtqqvyg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3obrrolhm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zijytqzf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3mnwlowrh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3yiycoqng.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3xmgmuebx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xfmcymlu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hslppdzq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gdduwoaz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gknofvti.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ubpxkypy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jtwgcqep.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3swnhnjtl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xwhtmsgg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3mxvlicqd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ohkminct.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3lfkrvmmc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lryfxdsq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3pkmrioov.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3wsqjetmv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3tpgpqdjh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ysoccwuu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ccmwfgyz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dsvhrckv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3mnfgjmlo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cpmjuort.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mtloztii.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nprfaogz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3gvgohcjr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fltjtbtt.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lizvtyko.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3xlgrkcyi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hrqkmnac.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3cismskub.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3dfbnyyft.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3vdrusdam.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3twhiaedc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3mxxzqieh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ecytzqra.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3oadodkia.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3eezakkus.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3nsaqfjio.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3dkegpcue.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3jpamfiat.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ngtwswkl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3symcqrhd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qnetmwvp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3vkipbyht.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tuvfayrm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gqruexdo.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nhxirivn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3qesbkzkm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3sdslntga.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3jblgnkyl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3juessesk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3eoqnsuwb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3lfuifjtk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3olgxwmvo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3adulhzlt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3fopyopnj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3fhmykjfm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3swjwgrae.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3whcbejcu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ksmoeotj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3dydampen.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vmuxcivs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3osbroaar.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3akniihrx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3scijougm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3hqfeguow.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ozlipkiv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ldixgifb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3igqewkzo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ayblgaiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyrtydfb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3wrtlwrbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhwswyzv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3atsjtqir.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3mkwkxojd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3pdjvmepi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3psovndgy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3gqfujhat.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bvfrfwhc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hipdtord.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3svmanujt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3bypuesyp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3marsjzvd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jjbyqhik.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cwsynkzh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3dxzykzfm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vutsktlb.html


<!-- 参考信息 -->