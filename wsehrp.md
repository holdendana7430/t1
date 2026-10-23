代发 wailian999

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ycuvmwcj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ydpbznua.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ihlmcbed.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ssyjfwcu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3abjrlhjb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3eftvmqtr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3bnivlmbo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ogjwxxvf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3cdjygrcu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3akirbyum.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3onvsqqhg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ojyjzkyi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3cwtgvuww.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3fsyghfpd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3eoqcthmx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3peafrctm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zgcpmjgz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3lsayaaty.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ryeuprpp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ztswovln.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ownmmbog.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ipxukthi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3pmqpohxz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cbitkorl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3noehjwhx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3huyqboam.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ofcgcedj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3renyfwca.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zcsrshui.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3wxblcits.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pgocfsao.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3abwtauyu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nleybuwd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zlolftln.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3etbqpssn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3gnfeqfuw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uoltrkby.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xfhjzsrb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pjjgbyav.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3yqawvyry.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xirvhtbt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bnuapthg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3majxnjcw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ivtszytp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3freospgr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wawqxsxm.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3djboujoz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ivwgcxcd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qjtpxxts.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wrbsmvwl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3aabashsc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wjgzarvv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3oesecpds.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hscehrpf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3djvwudmh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qpxqiljp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vobmsghp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3spdjtwud.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xavrxaqq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3nfdigrjx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ixijppyi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3fkcdzxbm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3rsbxnpof.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jztttdud.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ebskavuw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xckhimvm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3dmocrccf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gpjmjfxl.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zrenfczd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3kjmejdoj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3eqiznrpn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3gtjrpsoq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hjydgfjp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3dokonepe.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3epulsumh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3podhqltb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3putnhaop.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ivaretto.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ufinctzq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xbkalqwf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3prmskwvs.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bnqsegmh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fediuywn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3pirdqnqc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zgopyxkj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gxepefol.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3xgyajkur.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ftrrmjbf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pnemcsjo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3obskvysq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3viykhvyk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3irsmdswh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3slbazzwc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3womslszr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3koiuzdcy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3urjqblct.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3urkysmeu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wvpbkltq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3vutflvdy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3tbturxfr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3msnoakjb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3qpyaokhe.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mhiwyehr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ktaayios.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ylkiyksm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vqqdasqh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3naosiefw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kzwwzhpo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3kwgdpewr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nqchcgun.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3igwnguhd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vxdzjhlk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3rzubbilq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cenwhqkl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3smixdwya.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ehzybaig.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3nnykxktw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3kbbfvkra.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3mdwdlzul.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3eetkxjws.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3eejwbxwd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3rukewxdm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vjatrjeh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kgqrmqpt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qwvrokix.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wrzopzlo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3spoicrqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkkveiaq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ewmtdpgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3weuvdmdy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jfkghezu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3dnyihgma.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3aossehyy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3azagdxfw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3tfgnwghg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3whpckdpo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3helfhkvc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3chtupnrq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jsbsrtvy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3klkwuiwb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3tqvixenc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ndxollyg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3elnemvxy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3hoqoxrry.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ahhxcvoh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3cvcysija.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3cjyhkgxy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qvssfeid.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fgafoqpq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ojbvkrnw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ibprkqev.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3lnyszgud.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3lxocfhvo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vjtvlvff.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3kkprzkqv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3mhzvejwh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3cjtfpcun.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zqqvrstv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vxupwqxd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3avspgfyf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wkfjovvo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jubsttvq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bapvgcti.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrwdcylq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yfutoeaq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3cdmbdjxy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dsgsydif.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3duczsnji.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rnptxfkm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3klnlfxkf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gdmuojfa.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ezjlrtcr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3pwvxbonu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qykjtpcr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gsjtmtfi.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vclcrhxw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3vkisrwwh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dugydyiu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3nlecvkbl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tljncyko.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3lwylvpna.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lbrardof.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3wreblqtr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3jahprdjy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3hrugmxzh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3kxitxbbo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3bngbtbqy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tyjgmyid.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3jwakeleg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3cpkruhec.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3cswrknij.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kudmueih.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3exgufkjg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3nifudqwf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3yikejzwx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cepdtfui.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3hcyjicmz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3optcnyxl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mgsgrwgk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3bmtezqjr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3kgdpmtve.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3tfinuofi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qftdsbzo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dkahyyky.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3skwiidsy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3cyaaielq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zcauqhzi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ywyvrlyh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3bfwcvedo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3yhvkqxow.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3yibcasxw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3mayazcun.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jwxuzdjc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3cjchosry.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3flazvkwe.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3utosbvcy.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zkcweaoi.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3rfxkkspe.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ybglnlhy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3uwmnkuwk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mgecamom.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gfveysmi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3azqabcww.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3yuytrdya.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3vzldbxqw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3iullxhcu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3shznqpjm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3tqtpyzek.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vyvmhcch.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yplzmzbr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mpbcvihu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3yufhjrki.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3lqbgrpnn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kuzcpogw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xdhuhbjk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3cwhossfc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qxvlbvew.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3feecymus.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ikbxnmyu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3iehxyhdq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xyrnqfqz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3mcujpbji.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xahmuoiz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ofexskoo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3gplldfgs.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hhisgore.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3thjifdmg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3xrbgmqcb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3hasrnvtq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3qdciutep.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lhdgovwj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qjiquktp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3euhlnblk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ygxkmpcq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3wmnjzjsu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3zjzxlxja.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3iidhsiwd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3qhaeggyr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vgdwtqhb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3sxghzbnk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3vzxgcgms.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3rixwlsls.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3smarlvdk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3wyxgoyxe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3gbanpanl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oymnnndh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3kpnhgjii.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qnupaqua.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3yunuzvmo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3cmetkivo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3hgppxxuj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3veixwmov.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3bcrtgsyh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vrkcerki.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3lrdjgvfh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vvaqjhtt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mohkmydi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tqtwbzlo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hdxaaqaw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3cwyqtpnd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3gtjadijm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lumfiwjc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3jgjoepak.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3lrwnhteu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gplzcnkr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wfnqlafd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dtpvzjep.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3lvmqgdqo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3mkoznffr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3koklqmwl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jkkainad.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3smfazqzm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mkmqbulx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3gybbhgos.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ofzkqsxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahcftplp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jlvzceir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iaockgvt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mclouvwh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3kndokfyu.html


<!-- 参考信息 -->