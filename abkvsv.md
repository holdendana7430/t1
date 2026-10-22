代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2wiionntr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2qwpogumq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2tiosdrth.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kvkxejue.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2opibfole.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ehadxdsl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dqmpcsxc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2evoeelst.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jxfqohrn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2mxntjyad.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2pfgqmpfh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hxgwhwbp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2yvvqiash.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fnpquuol.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vvarkgyp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2svdtfwdq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2hwbtmdwh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2rluetccz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2imwffcqu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2jfenwxpv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mjsaftmj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2wztvmzma.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rwfqdebn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2rogixxqj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2tbtlcykh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2pqeuwkwl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tsdrirdw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kcmadgur.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xumhyrqn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2cdfifioh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2otvdzfqt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ufxhgxwl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qnvidctf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nkaycttb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xpohxihz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ifgbvlvv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mjrzxmkg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2teccdhjs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zpnhgyzr.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2kbaioyaa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wlsoxlwm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2finjvshu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2pavzbmaq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pjhfdzcr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ensvsnir.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ngbcrbfh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2yqzaebfl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vfnjvurp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2jnlznmnd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2rcdllzwe.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2tewpldkz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2enmawbjp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2kzcmcjfx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zohyolhw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2xoipnstz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2pzcvlxcb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2jvqbokwc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2lqhkirxj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2petucpec.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2yczekpqz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xzycgeze.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2jpnxlydg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2vuitpeuc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jbuhxrvv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2gybeculf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2dwnpvafn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2coehwfpv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2jpthpohp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2skzmqaco.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2orqrvjhm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lonuuphl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ppakajtw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2dnjpmcdu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2abmwcoqy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2upnikgat.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2eqwcxbqn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2pttpaott.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ytpkatxr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dvbaagqg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2svurewcl.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2uzdunbkx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wehlvofh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2abfmgcoq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2mtnyurrd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2cxvehaif.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nfmepsbr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sxgltyql.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2olavsrqa.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2myfjcoca.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ckxsungd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dlgcaodf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mhflxyxs.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wtnwxjlr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rhphdlza.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2wijyzxnz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2eskynhcu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kwgttvpx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2dgcbtqua.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2wtxkzgng.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2sruslcwj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2cvpfbtbm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2yrrhygwz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bvdiazbr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fhsujzfj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vqgsqlaz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2oxipygcv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2alhddlyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdukpows.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hjwotuhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzuasvih.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2bvmyljzd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2iyeylutm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2hwwvvteg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2mitiayne.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hzgkpete.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2mdljhcyw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2iublszkl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2egazyfyr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2iuitrkgv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2qoihvwmx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2pnqyiwun.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2tvshbosi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2syzdeniu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhhyokpr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yslbkwtq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fpbckurx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gicvsgla.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cjyanuhm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lgzqhovy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2aucstfot.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xvmgpsci.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2gypebilh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2mqwcoupw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2moiajeuf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2odunkfun.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2drdwggbq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2iiteymtr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ojawmovj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ihthxhmq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2neupwxeg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ndlljwoh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2jwqmvycn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nhzxfsrx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2krffybty.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2kdcxvxao.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2oeionugt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tcqkoapk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qlbgrgyk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rauiwdwf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wdolucgw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qnklpviz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jqwuickl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rnxwijzh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2anbqbasj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lrhzbiuv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yyjycdht.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2twrengwa.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pgsqvbta.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jxhctqvl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dahygqcj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2cdvcauyp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2etpxlsfa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2fgepkpfj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2sswhamkh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2delrddal.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2cqwclhhw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2sllynjbb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ridyyapc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2leqnaqzd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fzszemxw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2tilliupu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qaekkozl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qorqqybb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fvznehzq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rabxiurh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2epixhjde.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsisqjkx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2jvsimykg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pdkpaxgf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fsuzdfhf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2gspyjfhi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2zbdhzbik.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xpfnvuhs.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2emtepoxw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2wtmweeuz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rqcrwwsa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2wwpnjwaq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qdhgjtlu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qphhdrsw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2zhlhwchu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2amyfqfwn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2thnmjrgs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uhagdsmj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ovoudhoi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2nhgziewe.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qpsbloor.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2asdxobdm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zhgbwgxh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2redegnab.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2lflonuws.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2czaqbhcv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2cykixjnb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ycbteusq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tkcgnvgy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2knkpcdwn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2gxgjwdjw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2liifdkeu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jdunfjda.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ajacubpb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2pjwjvfdj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iecvtkby.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2omotfvrj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2itcdrtay.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vjadgnqb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oicjeauy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2pimygrgd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2cghvbgfv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ffwrjvxv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2mlbyxdzs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xoqdusxr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2joybqosl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2khbfjsem.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2exczbfst.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2phuzbrff.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2iopsisng.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2qizfklft.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ftioebbj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2farlrrmg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2efrccoqk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2kqqbifhr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lcuhspop.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2vynzgcvc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2asyjvdio.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xcifjqlt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gfawuajt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vlyydjgh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bqmagand.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2aiaqbgvc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2rxdgwhfy.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2odfzbszo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2lzcviqoe.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kwyjzmpd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2aqdzqyrd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2bouplgul.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kvohacqt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hjpvsbtx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wdjeizsj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2caezmqlf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mfonefer.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2fukmdxmw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2omtbmivu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2mzfmnzuz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2skejjfcn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2eebhvcjd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2gmxeyhhq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mgxwnwdu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ngcwxptp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ozmjfmae.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2aoemezrl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ysjsqeoq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2czkpvjqs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2txwssgbc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fybcrhem.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ayifumav.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2qgzgdxfv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2mvpdhlnf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qpumqxyq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2axumytqb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xcxxmzjr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2kawzwnxw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2bwhhbyyz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hoatvhaq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2hkdmbabd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ojekzdfq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mdrkaeyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxwdoutc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cqgbvbnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmnwyfql.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gthvilrp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2jslteycf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ttynwomy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jqzsdwhi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xjwuanae.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2etnxuorx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2nxmdjoyb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2wflvohmr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qknlmpph.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gvxehcqh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dwiuaxpt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rvbrphte.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2rqjocmff.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ygtzlqxo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2emdprnzd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2pobocbng.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2pakiojjd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2yxuxyggg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fyaeazyt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2iuvhanuu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xbqmwivz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bhhlzssj.html


<!-- 参考信息 -->