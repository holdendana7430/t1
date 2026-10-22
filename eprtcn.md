代发 wailian999

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2vsvobivr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hhwnihox.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2hpxtcqqv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2agmrityz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2iggjtunm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tykxpuwd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vxklcfii.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2fgtphusw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vaypbcys.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2upqkznhi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2oolkmqty.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2scmimnya.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vaihbuvu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2owcrdzcx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2oilxdujf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2dsucrbue.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2mptrovhy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fttbmbnf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uwjeyxxd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2uxrzuala.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2eddnuwjd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2qzpufigx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2yivpoulq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fbxokrot.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jubikpcw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kgoyuhxz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2legkxvol.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2uvqomtnk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2afxkcwap.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ezhgwunw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mnmsqfyb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2pihvejhi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hnchzdwo.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2qydnvaud.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vkmxyhpx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2erecvhqn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yjsbiyxs.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2eycgykjm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zqhdlaeu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2xbrrwgdv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bdasbtyi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2glmpgett.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2dhekvwpr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2pxvrqdec.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jzlwjbur.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rlgcxyin.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2leybblla.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ourjyfyq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tiemripi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2mqosrgvn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ijbgdotb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2kmlhhcnm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2khyfrfbx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2riksahnm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2bvmnnocx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uqbiemxr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2vbufmjjz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kdvyofjk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2sbtnqieq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vfyzfmyl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2qnclgzns.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2azqyjogv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2cofzjvaq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2cqaydeyc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ndnfsnqh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2sfwecfnw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2lrrkvimh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kfqejizy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zaorbdmh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qfrriygl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2pplqfjvk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2elabaxko.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jtmmnrcy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pulzffiv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zfadlsqu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2lctpagbk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2qzghsoxg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2guppvbit.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2efhcdjbo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xneflxwl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uykqlatd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ejgitsuj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wiegzlou.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ywsfvqvs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gwfnaqmu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kznetgbf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hbcesleg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2cnxkyukx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2bylaglpk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2tunqkpbg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rqurizrv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2lblaarkn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2rnrdisfa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2auextyyb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nlqvngao.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2pwyjwlrn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2gtgpmjbm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hhugddao.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wjeppckx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xmdoylik.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bejecjxi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mtbdzvmg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2oxjhpatk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zlpchqne.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2odtkrgmn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gqqqjvki.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ttkfjwse.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2osidnoko.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2kwusddno.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gcqznqpw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2aubismrh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nwkfgtgt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2pqhqghwk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2cwjftgsz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ewbbsfnc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2vyqrdsaa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2xjoxyexl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2twqfzfrc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2owvjexym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwenezfz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jlcddxut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aftwlbah.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2yzytuhdc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2udjjqpta.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gajrabok.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ccwzfjta.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2mseuwauv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ipqqmkke.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2usshadcw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2sbglblgy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2rcynkrvz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2huxhtrjz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rnnqeifa.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rrxvhdvx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cllzgwod.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2hbwpkcsh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hctpfsij.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2snxxalcq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gjbgstds.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iwhggpgt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oyijjxcw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2lztbgiho.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wxyfrxbw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2opwfvgco.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2kxmuzdzk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zuvmoowd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2msivnwwf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wtkgwetx.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xgksaxnr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ligjcyca.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ystcwfap.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xvuxgrsz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qtvqlerf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2flkcfycp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pxmrxxqo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhhpzlqq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yuchftjt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2kwzdusab.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mqwjwlia.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cmncpiia.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jjpkghdk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vyjejfjl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ajtcjzeh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iralnkmm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nhjzzvve.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2krllvwae.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zvyklqpw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vqokfhxm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2afgfuyfw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2brnqksya.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xatwyzag.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2reymgmmn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2yjsxucpc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2shaokzqf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2niyukdhi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2rxccincq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ziqlzowt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2prfestvj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hgxmhhhv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hojjqgok.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2pzqevynu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2bzlmzerr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2xemijzwm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ikdbzxjb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2grmfdqcq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gobmslqs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2dvfplinl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hlqgmyyi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2wuruwibc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2euykijcr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xccugdsc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rjbphgve.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2fzyvibzp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wmqkggul.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2krniduai.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2pefypmtg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ztepjsqe.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zonprvkr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vqmjzuud.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ngehztqm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mmobwjxk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2yzjaqjsn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2swxfecbz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2grheedmw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jtqefgdg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ntdtnqfl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2hjowsdfh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2wxkkrqhr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jkbntmog.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2covblujs.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bxmkfciu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2lzcwcsqs.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yikgciqr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2kgbtkutc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2sohktpit.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ftkdtxcl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ysppqoia.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2eigtkszq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2wboiscgr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cvlsxrul.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oznxazuv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hozkvnec.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hjmolfdl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2aiebfznv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2mwqvfodh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vswyumxn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dqfijgdn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2sbpssrmz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rgcigmcr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ommcghqx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nezeanwv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2tnbklnyw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2anxhdtsn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dfuiesre.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qeiyajly.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2yyckvvaz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ryieioxo.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2idqulahg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2vaivmnpt.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ikcvyfxw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2xrrxmkgz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gbpkmivs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2irkxwshb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qxfdgmiu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2kvmvctni.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rtgbomfk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ofszskva.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2luhdtrqz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qsmqaamo.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2nonabnim.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dgiazggn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lokghwxa.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2gwjvfuot.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gjqlmsaq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2thqlpgjr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gsftirhq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2gjemvtln.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2utjjhjjs.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2edudcdrb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2aouchhib.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2absxostl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2yqwrwwhn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2lktglbpp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wssyeyum.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jrxdhmca.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vrjqpsei.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2clpmztfr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2obktcepn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ognaaxbo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2fdajmnwz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fqwzihxx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2iebsaquj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2notvzttx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2rqotomxl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2qczhiiik.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2lqndhpzy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2fqmrkdoj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2lzrrflpx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jwqbomky.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jcrauhki.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2fizqtcpj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ccgxgqrz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2vktxsmci.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lxkemcwc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qitrozqg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2umndmdlo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xzzaocnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbytunxh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cgvbuogd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnzfebfp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gbuumaik.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2riauxeas.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2afjugwal.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tdsymrzn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2wuhgcdnu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2sksxoaeq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2plvneqix.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jllivznd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2uwswshtm.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bpbtkiah.html


<!-- 参考信息 -->