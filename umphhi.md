代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ucumpegw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3vpfwndkm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3hqcwrtwj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xgstywip.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3alpacmal.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vbbybpvl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3uyxzaxxk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3skuqlkrh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nobxeazx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ncfonwjn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3kwkotoka.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hyvrufah.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3tpuuipeo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zmmooojm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gpacpezy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3zryeetvg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iobibmzn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3phyeooso.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3pxqxzynq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3balaghry.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dovwzmgl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hcridbsu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3expiyfmv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hpmeprww.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3tahvawvg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3eqdypexk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3obbhakwo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3gmltzhkm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3upzldphr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3petlibls.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3sehszhkb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cjxfgpnc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nrfdyftl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zsfermlp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rkzonwjx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3hsxrqshs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iynjgbxq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3faqixhub.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3acbplgqt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3lghlaeop.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xmaqyqpo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xqecfssp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ktlxtoiw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jyulkvxw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3kuplqnud.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wwvdmqxn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3lfkscxoy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ofivqztk.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3okfoulxi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zvqfjcin.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3vhefadro.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3hcrislem.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3jvhozuxh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xwlwdeop.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3pvduvtoh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3sqfwmrix.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3gmzcofdv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3cuqpcqud.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qgltaodx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3uhmfqlco.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3amtiiodd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3kbetkket.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3hmjvwkrd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3kpklcvpl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3siubpjzr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ijoibcko.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3uihwjcpt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3tugzupsz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3goxpiexj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3pqmurlbc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jiveuuar.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3bouipsja.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3yyhmidik.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rmecfwme.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zohzgugj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3cdnrxswd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3mhsyjzvp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3pfcxmtbb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3xohlaivt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3djiioedx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wdlholsh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qvprfsri.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3iqcgioie.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3mmtwdhpi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vpwdoqts.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ladebmqr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3oacxitij.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3swftekst.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ilhfzlgb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3musnxrlb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nrrphlfc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dcykgnsx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3khqypnca.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hxgunlfc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3jbaoyetf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3aodzfhyt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hlbdbfna.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3dbrrbzny.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3hvkgkkoe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qsrygdqu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3epbloizw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3lzaqjwpl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wbrajgxz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mlbbfake.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3xiwprwex.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3stgshnkw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3mnbsshyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iukighrq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ppbadjmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojmhpkky.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3rvylysfc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ybhpbqxx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3sahewwrd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3xpdcjnqb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3caiyfwla.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kgdylatu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3qpnkvxhf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3oloarqcy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ihqezrwf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tjjkayqg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3hxqehadt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fjmuvufx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lyqbowxf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3hymibthv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3epayozga.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zuhicara.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eiwsyinw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hdhkskzd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3temjivhd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3cljjgprp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rrkxiihl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3zcesnint.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3qegsdbze.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3liofxbix.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3qinacang.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3tzofbzey.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3basuzutq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3tcqimwfm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gcbhxzvg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3duopvjwr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ddqupywl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3giwvokkp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dvijtdqv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tdiojqzd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3hdzpbzck.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3dzjcdtpz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kehlqngl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3pywzqyoo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bvppeazv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wnfcxded.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3hedbilku.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gyhoirnr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3zbcwipjw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3eehghhkc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3baclfdpn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kiezkupa.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3boqmnskt.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3plalknoz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wysagwhv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dnwteuop.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3geauzxgo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tgsxfzxq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3kzsdfxrj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3nuyqdkqz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jrwoahrq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ultothxf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3kafqxhoj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3fhhnmsef.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ngtjnrso.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3yewlunmx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gnkfqfra.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fouoztuw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vsihetrj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3uavkrfcg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ozbzavat.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3njcjknbm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3thnnxlcd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3vfxgykok.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mkakxyfa.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3lqvafubc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3zjmprkab.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xypdesbg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zyafslwn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3uwpmxrvg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3vcghleqp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3eovtrvqx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3oxhbfdfd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nivkebsw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3waaqxadc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cgebzzvu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3woadhsos.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3nslvcmrv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ufhztjvq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3lzodigub.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3yxfneuqq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3klworxxx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wpcpdqvw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3gobolqkq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hoveqzzd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wygpjbdy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3fjmbtlsz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3yehvsyjo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3dsimnpex.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hfmbytdk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bgjbfyhh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3vopinobq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3flluzxkx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ujfrszfp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vuqqteey.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ylxdnnsd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rzoxmbkc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3agdaxrua.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3jrlbfcvn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3qxilwhhq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qwukhftx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3mrujsmct.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3broarmyi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3bpghdftv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3tkbwccmu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3gjhgzosd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3rmbivebl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3oxxuidhr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bxdbxzbg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3puwbaxhb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3loelkxzc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qpusquml.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3jnigolyc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3hotmosfv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3wacwnkeh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3fjiivhru.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3cnagyuyt.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xofshuoy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3jnzgafww.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ukiktmxl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3hzlasxob.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ikmcywng.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3sgztmxpa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3pmrcyymj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3veetterj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wlqrzscg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3usnrjzfr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3hesywdbx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3fzavexln.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ivhiokth.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3whdngjfl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zpexagpv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3rktpwojo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3zzsrxfwt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wibjhvcf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3okaecxzb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3idamapto.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3kxxqfjsv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3fvmsyegr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3pbwleadb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pfsnwjuk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3idqgokpj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3oegwnhil.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ayjqlxvt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3duolvjeq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vkovnojy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3kppadylo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3mpiwadot.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uhtubxvs.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3plhgwhex.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3jfbckwim.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3tgkptjjo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kscyizxe.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3angzjnsb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3eikvlswt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qbqmkgod.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jbjyoyye.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3itsqyxel.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3eatjepsx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3rhxfaxlq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ykkwnlrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ioggfbzj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nmdatdep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dyzkefwe.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aragvxop.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qtgomzri.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3byypexey.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fsomgqrf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3njkpaxhf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3dvvqvhbh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3vvgplnxg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3iuqmrzve.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bzitvlnd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mvmyzcdf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3xysqrtzh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bppuesze.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3isqzpzcj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3bfoyapjk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3bvdekyrk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3psdbgioy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3gjjrvsvy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3hwbfibax.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wawxkbnx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gaecugos.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xxgqxjje.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mxuwgptu.html


<!-- 参考信息 -->