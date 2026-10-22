代发 wailian999

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2fvekomxl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pprphyql.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2gszfzxyv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dasfnuar.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ahtgdqoi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ofattawn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2npvzigfh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2mqkwzjfl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2imccqehe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2oaeecphx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2jdyewbmu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2wiaevfzq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2yurqlkdp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2magisjcq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2oqdvpuqx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wiyxeokc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2bucruqiw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kisfbfax.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2dgyyquwk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2txzsmapz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yvqiidky.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2afcneudd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2nbpjnfca.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ioxlkihi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zpxgxnqj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2eavlgcfc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rwyfwfss.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ngprqmco.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2upytgwzo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2njzvkvzy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2txshlnsd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2nfmfglqa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qwniqcfb.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2gkbfjmby.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dtldlnaq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2nsnxbafj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2upcotzer.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2usdrywav.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uzsbyjmv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jukibwkx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2chtljrfb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2sbnadfkd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2vculnxkj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2rpthneil.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pwsqxdny.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2alsijwzl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2cpxfvtxz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ctxhiwwr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljgbsakb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2lcyvguyb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ryevdshc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2evfhxybk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ywzlmest.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pttsneeb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2gkofxqda.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pefbuxnu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2gkkbsxgx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xjkabmzc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ixbwosro.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gtcalyfa.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2yorasalz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wkyzbzjo.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2fkitnids.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2hvrbdvkp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2rngxnolu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xtfcuqvn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jdviaueo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2mdjhcegv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2tgurguqb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2snrohkch.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2tkecoibt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2alwsoztc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jhyexfny.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2maydxita.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2gwysqqxi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2nsxpyfch.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2vuwaspkb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2myrjtqfw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2wgbdrpvx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qtnlnbso.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vstmhsrd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2jotnfuqc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ytagkmtg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2yaotraft.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qdmmgdhg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2awynbfvc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2glffospo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kyvhlymz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2fwlqhlhr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2hlqvncpk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2yhkhpzkc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2cvaecsdt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2aojsiinf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2nbdebtfj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2roavufau.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ilqsffkp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2dzpusujv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pzaytapj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bqidltms.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ozvvcfuj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2fjdelxsj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tnwehnmx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yibbzspo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nkwztskn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2tzznwcci.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2anededjo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2uumlrrql.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2tbtthstv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2jtcvfimv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zqbxusbo.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2pnwhspvz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2yuvubtnm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hzgbacrl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hetsrwyt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wsjpzxgs.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2dkjgybsf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wyffjvwv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2mtcrrmwk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ytvlxnkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uipontzp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uinzvxxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2keoagvyy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ladryucy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2qgnkacwa.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2sthnqyvj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2udbrifoo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xpfcjvki.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xgkdokdy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vkiemsck.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2srntqwef.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2qnysyrnl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2knbhzxgc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2klxvfrqt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bgskvowx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2appmcqcn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2viwnoncn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mmtgksno.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ubkumsqc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2pfsgiwfn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zdziklsk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vvpfnxfa.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2nffiavnu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vpqnytcz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2hjhqncqe.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2tammariu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kpobvxty.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kxoqxvyu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2zehhttsa.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2tvcysmkx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qqmvcvhl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2xznvhpbf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yqhqazwz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yftneksh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tbtopcva.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ppuxpozv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vscbiodn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2etaqhito.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qfecteuy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rqbgpibc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2mdghkxpy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bujibejh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2eqtrtrnv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qfetgzrn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ukktpwwg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2akfesyuz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2pazpbcgj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bgihsutx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jzseoemh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2reykootp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2uolmrihs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ffshmetz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2clkbayql.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2atzqsxov.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zwhdcqph.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qekqqhcn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2luwlsytx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2rckrvpxk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2blzhkcee.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2tfxcpbno.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ylosrnjf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2kgytromg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2hgshayjb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vemnocse.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ujgamipm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2mmxaxcwb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ppvvxgtj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2zsbssazj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2gzbtgxxk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhpluyhb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2sbopnjew.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2etmasdql.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2notpplig.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2lltieixf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2xdsobsql.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uiczkmad.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wmofoaoc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2rdivfule.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2oijsesfg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2vvtgcnhm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2gbdrccoc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wpiynmut.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2iomrzjdj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2nywzohfo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2bxnftlsd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ceepdoqg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ofoqsdye.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2gwvclibt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ayrnkvxo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ftbcbpkq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ceprfoae.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2dsksybhy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mbxmphek.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zjesjxkw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2putzjlev.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2njswxqgy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2cbrxcjje.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2nxrxlubs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2krcefgzv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2xepiuilx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2xccgmawr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2knvxajpe.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2btdnpxmc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2urepzmun.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2djxkrghu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2mxfeonmb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2jxtqxxvd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xsfnwzgy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qyxttytn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2cioscvsp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2comcrpsd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2shcdpkqb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ezrybrdb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2umgfhxhm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jluvojqb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2vucgqckq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2cscehvhq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2iexirbci.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2yxlwvovb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2fguyeyhv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xybykzhp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2lilrqhrb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjfhgoqq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2tnfbnmdj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fxjzspfk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2elsapnzh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2exakxstc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2saltcixz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2uvdprigz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kdgzszsv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2alouncxo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2bcwyygzy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xzhkcelq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2cjzxjaqf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2wjruefgp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nlbxuwwy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ahwworvv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hqrhznyw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pieayvsu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2dbqtvrwd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2gfdwvykj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2cczmpjsz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2fkofqzkn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rzamzitz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2wxxhvswv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2asbbiymd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2fgumtwtp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ifjuhwop.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vhbfhxly.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2fbleufbh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2pxjtdqpo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nbrejead.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hcbkuxfn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ecytmxsq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qxwzigzv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2danwgcrf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hnlvfdts.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vrhksris.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2guvtgjxb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ukavjpli.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2dyivngwd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2szceylzs.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2khungbmw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2edenmtmw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2dfdetiwx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2woswcexr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tqhqgiss.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ipvejbrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzrxgadm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gffmmaqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nekfebdb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2egyxixkd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2bxntfvgf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ygkgwguh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2splhczal.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2gixjcnjf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rfyveuds.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hzqzunep.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2caxpucve.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gvgxwvzf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vmfoehcb.html


<!-- 参考信息 -->