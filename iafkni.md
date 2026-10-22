代发 wailian999

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ewcftxjj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wqupebvp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2eodwgpjh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ccnnuikd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2xcvhspvn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qhwsdwuu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jyvcwgud.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2zuvghcis.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2brmflujv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nsdvlfqh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2tsstlhsw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jextmdfe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2cczitiud.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2nrqgmozk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rsiehklj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2klrwlckc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2njjdjqbr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wydehsbo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2siulslph.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ipviapwh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2nhuwispq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2vkpzoczk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2uedtiqms.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yrsfwnlk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2wglwogbr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cgpbxeej.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2orlobsbz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2yjxhvqmm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oplqddge.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2rmgjuydi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2blgzfpmb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ahqtzdiu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kjgkpzhh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2jogxuktp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xgktlesq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2iqzjtthv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cbfjmqax.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ztpnygqo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vwbbbgvk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2gjcopjih.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ngxfjorh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2biofoxdy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2edldcrea.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xewrbczn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qptbufxc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jtfptwke.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2uvxoxrhz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2yqyqtppc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xgvytjow.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2tdmreshm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nsmvsuya.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ukpykxjc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pnzfedgx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lzjwhdxu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2bebixdfu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2chtdtpil.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2mbgkftdp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aoajpzrm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wceeitwb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hnxomgqf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xusxjrxu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fzzmrfff.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2uqseijvs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2rogkygrg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2pfsjkbrz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ltahsyuw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2kncclgfg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2hupucmee.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2wjfksohw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2clewxwua.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2mrrxcbir.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ldebpmxe.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dcmukjnr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2filfuudf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2rjfrfssk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2iydghnef.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2oloucklh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2farrpwts.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2euxmgusc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2swsunowe.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lusobqxx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2xpncgjkv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lznvhgsx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2fqmogbde.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2xpyqpdae.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kijubcjv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cqdlqwmh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2dymebbse.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ijczulxu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2vscuxqza.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2bfhnuzwu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2lguileui.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2cfxdjzbf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2czhhosfh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rgucarjq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2vllopfms.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2lymbbndw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wayxqafg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hbbvtpws.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2scueajtd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mnwehzuw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jovvzfnd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ijlumpeo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2abjgvmrh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2tfmixjxp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gmvqjojo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2lpxmcdnb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2kgufnirm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ewrpbrig.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2sokxggtp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2dtgemnfn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2hlysbopq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2gomwgsqt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2xmcowtjs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mjyuybvh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2kdbgawdg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nkbrrbck.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2hgvhfvum.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ijbgdrrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttjrricg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2mlbqpvqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jeerwfzf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2uvwrstvw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2zqsuwozo.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2nqccvjpe.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ovzjfegw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2bqyhticz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2sztslhjc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2jtymuwqv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vyrrfipk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2yknutupk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mizhzsvg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2izdykcvx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2crmqtdcp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hinudnxe.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2etniwowb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nyulowmb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2xvbdmqvy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jqwfutmx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zxefxitb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2xxaiixve.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vzscqdhn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fgzztktg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2rtmyfftb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2laobnacs.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vterxunn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ryidmujk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xyvqpuse.html

esac
来源：http://www.52xcode.cn/Article/details/gt2iaiuoysg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2psrziqxk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2qcytatea.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dfzyjuim.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lvhqzlbk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2jmwsdhup.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lktvfmgf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qocwnurw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ipkxtdra.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2zmexszip.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rjondquc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rgvpbugn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gdxfndcc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2jfutrkwl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ntoxyvju.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nhhrcrdb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2lpzthgso.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2yuxdqbkg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2gfspygut.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jmifmgbx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ihssmoof.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ukffmoqa.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ucuagryn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nwrmdhjn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2aewyzsrk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2aekyjbte.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wprzlrsg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2pblkwova.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2mlodicgj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2bsdjdury.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vumsxboi.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2enrdxqtl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2skjtebph.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2crnbqujz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ftnkfmid.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pnkkxdyv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2drlheuel.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kgzurraj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2firdiseu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vyzkiovt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mckkdbcc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lwtsgtua.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lizssieh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2pzusjmek.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2wvmjcqrw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2emcdcacr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wcmnhmrs.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rdqdxokr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2hnelexlb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2agczeaxf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2bhamwkca.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2jrigtqhm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2cxcuokkm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kdpnnbhk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2khntxbvu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nfczfdar.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wszubzco.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jfobxosg.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2seoediog.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2bsusilnw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aazxyzpk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2fymfpkou.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2yncteuaa.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ayludabq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2pbwenrcp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vcfbptnb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mbafxsfs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qfcnilgz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2dbwtzclv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xaofyrup.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zinjdgmg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2tlpiklnb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kvrmcpmi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fsfzogfl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lckuiypk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2uqozukkv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2dqoszyon.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2sajhmtwm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dxuskoaf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2hqkhxgov.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rkxznlpe.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bgdjdbpg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2fzyvwniq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2oejkwqjv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fsymaedt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hkogyjck.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qxuwdxfq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2qbdjdkvi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2uyyyjwlu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dvoekrue.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ddhfihmr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2mvsqgiio.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2oizwluvk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rfoblxmb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2kfajcorn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xkgceiet.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2grxygzlq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tzjfupmw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2xqzaiyyx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kbchtmqk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rlxfmpyn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nypubxnz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rturmbwv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2slofetkt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zohbhkrw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gyjhlsyg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qavslrjy.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2bkzniamq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vbdoevba.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2yvjlogbz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2cwzzvttq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2gvuuqhyl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2exbyqwhq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2gfmqdjly.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2fgwzlvxx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2mvutdigo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lwqfgxwe.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lrrapqya.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gdvxtumy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jqugpnrm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2mbulemdy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2bqphryjf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ucxgmfnu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2eunykbbt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2zkzbqefl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xkgmymxl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jyrwyayd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wkonxwal.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2lghabgbu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2bjibcozy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mtbancet.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2zyjynbck.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2nzdiybmi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2kjrveyrm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vmghnguq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ecztksqo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2urtbelnb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2yuvemkfh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xwuuhzmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmdjpfgu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2budppgjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2doirwnwt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vyataicb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2cgcblzgr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2omryzcyr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2aebtaxss.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2iewnwwng.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vwfbuzbh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2rnawvqrr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ejjqfhln.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fsyvcqin.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nerlgtpa.html


<!-- 参考信息 -->