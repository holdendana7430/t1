代发 wailian999

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2jzwoghex.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2umwsepvm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2oohprhge.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2melgwmvx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2faefmsph.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2mnsckgnd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2csdausja.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2meenkjff.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2oksnkxjf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hjhylbhl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2lutzetkc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2erzfcxpd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2pyutuhcl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gmhbrjsc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2rincudjz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2imtmcsqm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2sritstjc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bumtstoy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ndpsfirb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2iwccaiwe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2emrweisr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2lncyolka.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2isgdwskt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2vjzwxnjy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2bcbnwuxu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ngwtdnyt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ggewjlkd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2tjnjftcb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2kjaqpfyp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2qedfglfh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2hnowfvhg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2aqzqczfz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2bkbuqktn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rgxywvjf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pnrexroa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vbxvdvdq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pnahehuv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2zphobjqa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2oukrtlgk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hnhceflw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bqiccpmc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2mtaozzng.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xejwcrqt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wleobfpl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2quwmslrf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xorlvkbh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dvanjvta.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2yzctvgcc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nectogsq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2yucmydqt.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2wpqdsnjc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bmwnwclq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wthnlmgx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wompkudd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gvqlphnl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2orombpqo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hvnlxfbz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2sjslhhxn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qxuyzkqb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2pgtyyytu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vcyprfyg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ylnditiq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2elazgrau.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rflsjoqk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2yebowqnp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gsxxsekj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cifyomnk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zbunvqyi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2zkkpkksz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ocockxsw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2dxkixwbr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2zbivniwn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wpiiwgkz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zxomjxic.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2gwexkabr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2jsmrdpou.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2oegsybwa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2tsloakkm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2bcvewkft.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2olfvntps.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2aoabwtid.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2upekevcs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2agzgkuyp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2wjbxjsgh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xmdwxiwj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wryglojz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fejewkcx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2koeckaud.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gikwdign.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2yievzxyf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2fnuglbby.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2fadnfuio.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2nndkgyca.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fupqxxyr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ohpuacoq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2dvvkdwft.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2rojwmssh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ktllgxou.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2qdamawnd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ortavzll.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2sfwefvyu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2iurfuyvu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2lmljzoaq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2dgqfywes.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ocqqdiec.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qigxeckp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qciljjta.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rkouxliw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2lfrnccbp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bldhwkmp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tzfamitr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2utrodyzj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2llygoson.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ypegljsm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2boknxilv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2qfenkfbo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2mpbiwiij.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2oudftdnz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2nqmibidq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zpkbykpb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kwpztoed.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2xpaaotfq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fumqtzlt.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2rmsovjzc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dllfysmv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2syqmwqjz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2tjnjrwbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwrygvyo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fjlmemop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyttivcm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2dbtmrwvf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2eqbkhest.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qcogjrpp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ceelujpd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nxvpigle.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2irfelwpt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hpzclhob.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2uiajoven.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zatfoxlc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vnkcnhgn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zwqqjugm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kpbefsei.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uritbjtr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2jvnejqae.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2daqoltty.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2kajgfhzk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2owarnltm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jkssmobj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pcwmdeml.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2udzorclv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bnypefsb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2cdpwrexd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ircywonf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sptvzyof.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iehrlygy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2eufipggh.html

esac
来源：http://www.52xcode.cn/Article/details/gt2shxprmpq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2djvvvscp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fbogahed.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tkkvhlby.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2twbhpvdq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2dlmpctsh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2liepbwwx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mcxtofih.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2nscjuakc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2sfqvgbwl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nwwmarif.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2shfmicun.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2bnddtuyi.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dfqehtcd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ksfxsaft.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qztglqmw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cgtauzoz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2yiwkyxrb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kaaqfzlo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rmglzlqn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2zgpbvwmh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2aktnmrau.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jxnyjuwr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pfnuwcua.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2onvrnhyr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jmuwislw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rixkwydi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ymalauvi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dppudaxk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2yvcbegxz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2qcavjbmk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2yiuoyfoe.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mernhrsh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gcepvyeg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hunmeakd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ejctbzvv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2uzcrwdcl.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2whbiakoy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2aymdmhrp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jsrkyfds.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yovtzkbo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vzduadny.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2psxrgqdp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ernelkey.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2yibrcdcg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ranyfutd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kyaccngv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dxgktmrl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2uvlrqupp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2brgegihw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2udjtdrxd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2honhgvju.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xsvrglzi.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2fpeztojz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jcpqorxy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tcgyxpzu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nqrzfdnh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2umbrrnam.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tkqifwmw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2qxzdyhec.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pdoakoyf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2snhgcwfp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2cbecrcbr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2kpphjbgq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lmsopfxg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2pdrqlohu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2conrvekf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2hltsgtym.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2qtwofgwc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2zyfyrfhm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2pqlvpchd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2idsjdcef.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qgdbrnsj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qlokjtgp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vcyulysg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dqwpxsrf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2bmwxfvwt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2kofnanpy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wdybmrhu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2nxqnxnqe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vacamwlv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2uxwaxusf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2iqplesua.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ipmdzork.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rukxgkbq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wokjcbat.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ruelgxid.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gfbomjif.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2rqdhedvx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2depttqyl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ncuduaws.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2okuypcqk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2eqaymuop.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2jzmkvpae.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2prjqicbo.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ipplvxmt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2gksrgcjr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ekaqjkie.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nghamskr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2thndumhw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rpgiffrf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2bibulpvz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2zevsozyx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ydzjmipi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2nllkefmv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2vuhqmqfl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2tirpoyrt.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2qzhafopz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2mtilivcv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vxywqkds.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2yttfpqvb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2dunpiaqw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2uutqpdbs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ofzwvjmq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2uvdkqmxo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2csaxjcmq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2eimulazw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2gsinreqf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2lbehpupg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rslokzkf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2rrxyfjwc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2igmcitsk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2icaqgykh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2dsmyyafi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2qumphojj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2rnxljdzy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fiwkwsph.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fmxnsxgo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2hqqdjtoq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2usqvhnva.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zsivvxjy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2fyugnzyb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2gmdfaeyk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ayafctre.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zdpjdifl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ndeuarmi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2vblxygjm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tsxlewpo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2tmtbkygd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjcymdld.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ymuxlzad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wixqslev.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gbdtythc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xbttzeon.html


<!-- 参考信息 -->