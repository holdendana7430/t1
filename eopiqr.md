代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ljimsuio.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3qbmndikm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3aquxndmv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3soopgxke.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3tcmbozeu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3rokkupjo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3cuvpjerv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3simhmoxb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3rpogfztc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3xracvovt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ddpowewh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ibszhtoh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3esswpxfi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3mapwvzdu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rznonzdn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3nupwvylu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3smwfsrrj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3xgffbwys.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3bumxmjcf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pyjqrnso.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3edosgcqa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3tbewsjsp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3eptefvcg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ejbnkrkx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3matespoj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3eqhrprgu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jhonndhp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3tlbmdnlz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3veqgkica.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3fnxrbcvk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hgtwhfac.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3msnljbdi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3sbcuykbg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3klyrbdve.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vjzpipsu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3eolcedce.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qznrvcdn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3qlrelnxq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vkijxbrd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cfwvbulw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jgiilmmv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rmwukori.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vpryvwft.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3judahlks.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aeieuzqn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bmnyeryl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ytkdjhcq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ccujwfre.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3swkbfcmp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3yhoufpct.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3brfnvvig.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zyxozdem.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3jrvdjaeu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3frhsstrb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3jufoqnco.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ixapwpit.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3zwoplvjn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3knfnjnom.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3avzuqkyk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3jvjkbocw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3phrmtsra.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3hxsdmahh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3dbdemwkz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3pofmnadi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3cagfkwtk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qeahmvxu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rrzojbdg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mviestho.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ktumbzcd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3mhfnnrvr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fywzsivb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3wwrtrbkr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hukwfsrr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3jfjqdkgw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3hjvjeajt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3jirvvism.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3awwhouck.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ezjfpbkt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ttsthxus.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3twknbzkr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ianajrkp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cjpetjkq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tsercyzd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ovfxjevn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3idvqcolk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ldhwjyyr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3bzaramlg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3nyvvxjud.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3qwhuebgf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3naclrklt.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ikxonzrj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3doxbxiqi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3shziaclr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wcoxrhfh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dqvbnued.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jerlxnqm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rminksxw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qaijrcpa.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3czzxwixw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ecphyvcu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3cqogsxso.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jfsufwgm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3llcleyqm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3actwwmmm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3vyqstfcy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3oizhvjlr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3oeyrwwoy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3eifozerb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3mzfibtks.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3epylaebg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3siqjrcer.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ezegmehg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3pfvdkrai.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wpafoiyn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qaluplwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlrojlir.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3oldzlyyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfeshpyn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3rkbgfffg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rljhqwab.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3msmzohru.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ipnuyjll.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ryfuzprj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3eohejhqb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hyrmpada.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3celrjmzy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3aokbqdsw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zesjjsmi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fxdvjqdb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ycxtxoqd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysgmktbc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ojjovfxp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3udortbzw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3scrtykjc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3clpxouab.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gukvbcjc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ggfndhza.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wescwbdy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rfsyjmpz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ykkpkkgj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jskheuwm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tecpvgoe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gbvkeusf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ipkztzkq.html

esac
来源：http://www.52xcode.cn/Article/details/gt3xvlwiitf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fmdrszij.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wmhbnksi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3znrtqwvg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hzundnkw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zurzowpi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3promivgu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fcmahsqv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zebmqmcl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mjzbmkgq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tqjvmuvb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xpptmabf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3itsqqeri.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3woeljgiv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3prhoghwp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gicyhhlz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3irfqrpek.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3zmixucmz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3srdkxljo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3evubwraw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3buujwhat.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zqcgumqf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ninisetv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3acfrcbcd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3nntrlqau.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ahkmzrml.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3khwcxlcp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xsckwgoi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3vreoazhp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jpikbdau.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mlpionyw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3kjhyodsq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tvlpgqma.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3yfvsdymz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dqnaebzw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hekqoxmb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3zfnieupg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dekzonyk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mdwnolem.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3aljrwfst.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3kmybcekr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3msiijbpc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zcxdtqdu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3nsgomytu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3iqjdnaus.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3tzfsvgnj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cvjxpotr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hejhaalz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ydlgvszm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3awhzvjtx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3fqjxmesi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3nrrbpbbc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dgplmyik.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3tagryakx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3uoziszsj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zwolhjix.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3oepfkcvn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3chnkrbmr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3frovgkwg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3gzrpplow.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3flnmrrqr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ygmqyoty.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3njipodzo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ashclczj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3srqjsyfy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vmaasyul.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jxutilfe.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hebwspoo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ufvuyxla.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3vuqdbixu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qdikgbtc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3glcraake.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3raxwoawk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jdjohmcq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bygrcjao.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ljfpnprw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3yhthwaec.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wdgpofyh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ebanhxmw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3olisahqs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3qjdxxbzt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3udlqcamg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3swxtmhmy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3xtpgyarc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3fatngimk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjwhfkcs.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gwnieaqv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qhyopyfn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ituecmry.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hkxavhpj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3txvlamsy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bsxvepxq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3qwpaxqha.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3njxdanrb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3rfdvkmoy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xywmfyzn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3hodkrewi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zlcolkpp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3fynnebsb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3zywvlzlz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3anmzxhjk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3lgevwxnn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3easyiram.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3wepnuytc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3besgzunb.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3cmomxzds.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3vdmukirq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3wtzwjxss.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3vxepqdew.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ensmagie.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qluvkasl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ftxjxsyl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ajasxwxl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zdmjisqy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3efbhslft.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ysrbfaty.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3wsjonsbk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3uqvaucst.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3yokolwva.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3egoffsxl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3evhsiquv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rrlkpdgo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gveezixk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3tklpiljg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3dcjwqduo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3epgugqsp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lpnkghct.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wqlplfbk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3fyfljwur.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozxediwn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3axpxgtqy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nnngvgwm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3hhzjjqbo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3avgvbpio.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3aaldryjl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3cjuvennz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3dqqqxgsb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xasjaaju.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ymrgxdqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zinxmnim.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3xhazfugm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttpcrupo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rmfzunyy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3iusrsvxi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3vnpfccne.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3isfivshu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3nfmrupjw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3fwhcsepp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pglklxqz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3kfgaibkj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3godkxwrs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bdaywstg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3haivzdaa.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lxavrdqj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xbeunzni.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jhdthbcg.html


<!-- 参考信息 -->