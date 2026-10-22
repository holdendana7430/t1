代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2gzuqrdkf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vppnsuaq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ighnwanl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ygwdirbp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mjtmullp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2jpxcfwzx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2rpgztrka.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2lgbxzwyq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ssjayslh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2fnovpktp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xmgkzmtn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iyqohvgg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2lhxirjxr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jfjfphrv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2kolyiboi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2enigacif.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2mkukwahc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2gymquthc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2uavongwx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ceswzkte.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2yblsevml.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2pablovyx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fbizeyki.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2aizqkjdi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rpsrpvyu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bohvnnkc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wwdqtrjn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2sxojvbpd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uzbjkaap.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2jorhamyz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2abrnhcwv.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2rbvgeark.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2jxrkzqqd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2pbvhqkiq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kxkftyuk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2hcowyxis.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gmkvquyt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fwvjfipw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2stfyhpcc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jcclpbek.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2otwmuiwg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2zvkegfpx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lgixonfu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2vjxizcym.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kqdsdvuk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vfpqmtps.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xpgceboc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2imunmmzv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hxzkufkz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2engrnrtw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2dzywxzxa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hndqywkd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2nafdaybo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wakltkll.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ksjpxwbp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pbtqtqmh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vgzskjqc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2sqsyssmw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2yoycisfv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2zvewneny.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xjvdutem.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2bkrmiwhk.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nzrodnwv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2qlvtdncq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2yjkthvqo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2sctgllyh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2auqngypz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2urqqposd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fnrmhqhp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2upiqopji.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wolttpny.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ejsdmpja.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2quftbnnf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2yzapjqeb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vwgpgczn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qwpdnjqf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ylgxxgzy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fsakefvy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jbyqirkh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2kgntdkre.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ysymkveu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tkuzmeqg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yjrkfodt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kwjpalqk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2fszrxbge.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2qgcgtgvy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2auoxwyqu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xbevwnpw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2vtgxjdzx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2lgujxajb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ilbvgowr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2hffibrol.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2oyzdavvy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hozhznfk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zexjbbvp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eysokblr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2tzepwtpm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rzlduywx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jmmuqojl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2asylfukp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2uwfblnnk.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wxfbzcsj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2coknkjrz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2zqqjkmfy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ateeqydv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2klhrmyib.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2pswhhbla.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2mqlitfvf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2xjnvdwjf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fugnexkn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jbzyytxa.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2rmjwkvfj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2hdmiccya.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2fgdmlyvb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kpqvyksu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpcumdkq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2yjldqstp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewxzhhhu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2wnplsmtt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2thpcclaa.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2afkmekvv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2nhsljdae.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ouqkcpfs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2mmlzozee.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ppkhotdm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2royozlrt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2hzlszcan.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2togeyhmc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2xecftsjz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2nhgvxrsc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2afozwnri.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2sfooixre.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iwxdlpga.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hiuzarwu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gljcomcf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2aazqotng.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2agrktpmy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2yxpgffag.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bmdaxblq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2bkzaxdhg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2xszennqp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2mjpasqvo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cpyreull.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2asbfirur.html

esac
来源：http://www.52xcode.cn/Article/details/gt2thkegmpi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2hemvtkjv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ozsoowxb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fmzuysnh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2acludizp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kwnsfvym.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nevxjnau.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lqvimkvk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xgcromym.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2gzzlolte.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xqarpuum.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2jfznazxe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mxrhlmrc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zclmvwie.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2icbwkjmp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ramlhdcr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hdcecbsv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2hbbvarhb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2aeretzpj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kcpcutyn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2puxlxtvt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pmlyhryb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2tkwynmiw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wdtzxdfo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2arudvjee.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xospstlr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tyomswwd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ustwmqtd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yctthcnw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2epbdghiv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ilojfoxw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2rbylazmu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wbeijrgk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vnmzblud.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xswyxgwb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tsarfsec.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xhzjriqs.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mwoadmen.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2rlscqoql.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2uxhidcro.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2jnbcfytw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ivmoyqpd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qpamleis.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2tsgmelhs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ycbmymug.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mtajydnj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gzheerhn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gtmdfdhc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2jelzlgra.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zjhnluwe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2nrlgqjgp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wrrocppi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2jqmbroxg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2inznoawt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2kpnlefal.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2uvxnwuch.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hcknwqly.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2owgeezle.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2msovzunc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2inppxzwg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sfukemeu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2egrejifh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2etepojlg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ueybsygj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hapmwwox.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nkfbbxym.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jdjjfyut.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2gzvdtelx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2sbtzxjlq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qlhhzbyl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zjyticgb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kqbrzdit.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2niictnjg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bslmfprx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dxmyrmbw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2cnfvlvcl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2cnzkrvcm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vgplnigv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qdmxpgey.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fogmrxca.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2grbatpla.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mmroblpo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lstfsajs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2lchfgyvl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ywntcdwa.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2eceqefio.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2tkpiexbw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rhanznlp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2flnwnwht.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mzoxvvfh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2sdjgltrj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vwqnjihm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2accpkwjo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2scitvfuc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2mgqgfeqm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2iecmrwub.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qjzhqkdm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xyffylgx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ctwggeoy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2dqxdlrhi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2cduhqjug.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nliilpjn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ivbwichp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ffgsfqrn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2dopchqiz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ecmeoumi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2swavnqbz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2kplszcwz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hyegvpss.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ucbcwwiv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2mrkuclbd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2iddskegk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2utszueug.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2xwtdyutd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ptpgardb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2lddefikq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2sgofjxmn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2qtrbfgoi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qsabrttf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2urpnjbdd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lvoifbba.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2bbvhhqgs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ykaxjypb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2waskopcd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wmoghzcf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2dndifkat.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2grzcaqba.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2tkivsvep.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2isyjkkyv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jzdkkjtc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2isgdtmta.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2vfrsasbn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2jdpmpaow.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2vmphuixf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vcyngzny.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2vwawemoo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2yhwjzdcw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ynneymjh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xnblskro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ontfjmao.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2lqcpwrir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvqvkmqj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nkmprtyg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wdvapgcq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2cehuranu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bndlbmjg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vfuqfyaz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xraeizpr.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2rucltued.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jiwlxyjt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ayqqixws.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oeyniqpb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2eciifqfh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hxbqhvlv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2aeimyshy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2kaiwlawy.html


<!-- 参考信息 -->