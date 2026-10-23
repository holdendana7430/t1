代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pmljxdlo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3leqzvfve.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mnpulhse.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ibztnxkx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3omhhlapk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3sahntcoa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3obwepwdp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bdqqdplq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3zgxmjcsk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xawqrbul.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ctvhyvni.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3swafwsqw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3wfqbeskp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3leadsmwy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xrrtmknz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3xgihnnpn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3zbuhlnav.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uusejaqq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3qvdzlqow.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xgkqemse.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3jloigrlx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3luydubaj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3pgiqqkio.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3onuxyjrt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3oshkcjsc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3iyuhnhdq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3wknvtbba.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3chkuxuha.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ohlzqyxh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ikzuhlan.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3svqmpfiw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3qcvgwhpm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3bihfaeoo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qlivqghf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3iedgmxge.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ttbbxbha.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3arpcuuvv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3hozbtdxo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zlembfjy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3mqcjfiti.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ndqywlrz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3wifelkwj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ibxxandh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bsfhonwt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3gayomdue.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3beygfkib.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3drudrwtv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3jkkftzzx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3pbyltbfq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3sdhdhcdv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xkfjiige.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3rkiajlbu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3oheahssu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3cwejkbcq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ebgrqzmp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3nxamkyjo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mvfopbrr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mxzhyuri.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nhpofqun.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3bivtscph.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dzokplvk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3tujstcpc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3pxgsnvwb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3lqhrebje.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qtcmwdie.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3aafklule.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ylrlbhwa.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3xxuwphcl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pbybbfaf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3dkhukzbf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ctghfprb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ipxvynbw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3prkdgeec.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ywvgarek.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3elgsnysd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uihhfrex.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xueyayqp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vknokyee.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3wjgwkdyr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dfsmcmoc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3hsonxxzi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3lmgdozeb.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3bzxigwau.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lzueitmy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3tmgvcfyj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3dhwniovz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3otprnpdh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3bsbdtvqu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3gspjxfvy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ebmpuicr.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3vjexjnxm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dhsmrmdy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mbqwryni.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mtzkurvq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3cabeqdpd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3qmwuyqkx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3umbcjjfl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3zdaalyvx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jyxhyqee.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3bpitqqnn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yrqcgdpm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3mnedazfh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bhpfvixr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3zyssvlei.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3oqwtbycb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lbvzqxfs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3myfyrnjp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rvigvmfu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ofvqyxft.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qdhucoyk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3cwxqiqez.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zpfjpmdu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3dzglrwmf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3nbyydwro.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zjumelin.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3malsjenr.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ghqpqpzw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nizmezfl.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bayvfqxy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nsnpgdph.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3yawwufwj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zsyjsota.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nwpmjxyi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3brkuqzon.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3mvqxkusv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nhbrwtae.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3bjrpzpce.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3srqzuhgz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3xaenrucl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3zirwbgnt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3dizswsel.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qhsjfkrc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3rbhqpllq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3oqjbhnlq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jffbjvnc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ubzwgbei.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3crplhxrz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3dhwgrfua.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3aofmqobd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtwzylfk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ymqiczmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xukxarnu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3smnmlmag.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pkcbtmkx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wsaeevlg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3mtbmbmiz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dvhpwuji.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3xkncixqd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dcqqxlnn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xtnqegkm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3rximlpty.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tvqevlgd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jkgkwtfx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3nvlsvtby.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xbflseyr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3qcintdav.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3quhecvzq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dtacazvz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jzaynltc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rddrsvsh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ynicptgi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ibtjfduu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gwlqvuwl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tferebjv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3atztysum.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lsyzvzdq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vqyoowtt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3sakgqbgh.html

esac
来源：http://www.52xcode.cn/Article/details/gt3tioepkqc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xaurdetw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3adempiid.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3alsksnpx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ffcznkgx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3enribbod.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3urkovswk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qiqdtgub.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ooeylvvh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3tjuoakhn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kpzdnore.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xtlxkivb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3aupzmgeu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kfzccubj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xavqrmho.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zgxbuoby.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3nurpkswu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wzoqemxp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gqvbfbig.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hofqsjan.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3eughrkss.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gyylehna.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3psnweaof.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gfstzohf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rngdehpe.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ahauhdjy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nbyvludi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3kcicjpop.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hsxmmmsp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ixslsoek.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3zcotdeky.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3yaaeitat.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qjtgpoan.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3mywaojhz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lijrzjbc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jkoduuam.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3jrqzjpxi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ydmuizpq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3vjfedqyx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pwtykcau.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3yotiaupj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3pxmvzisn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qqgblmva.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3dzurunuq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3izbpzahf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3yxzgzvgw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ggarvyqt.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3syxjepcr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3yerzzrqw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3villmnpa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3kwqbhqgp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3zbfohjof.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zihezobu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3gnxquwqq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3qdemdupd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jcherrwb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ribiwgpk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3gzspaawm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ezbfyzvr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ljdgruqg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3oupgaqqi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3gnvnhsnu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3opsbeqjo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ubkcjxwz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hyyjjluy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ichxahme.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3flrxefxi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qpadyptz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3qisoyrsu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3testhqij.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zcsrmumn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3oddxpsuo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gojtfjoj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ezeifywy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iopgtjwc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3cdynszhz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3dvxsombr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3xxbpfvdb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mhduspin.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3kyomliyy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3yoqkkful.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nolngwwc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lodyuzqq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3acnbblne.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3praokpgc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3fcfmkovz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3phvslpvw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3iunccjfw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zawmbcty.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3kembxafh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3oppgkhbd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3thwwgpxd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3iqxbidys.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3kxlqclpi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3mtxvmtdl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bduwtkha.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dzxqqkzs.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3szvquurk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3tvyseexi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ymkunjzc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3vktcctgj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ixuizhmk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3uffomhbm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qucdkifp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3lqrxgjnq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3irbfkytb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ffblnrde.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3pjsodmdh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3duhvwwts.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kstaejjm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qgjxwehh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3rjiodafw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3opgsifqr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rkvsozit.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3srpkaprr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3skjxqhpf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3pvgfdjiw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gadvvboh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ytvssokm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hqlffoeg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3gfyfonnc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qvmusmej.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kqgkqxmm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mkvqvbpo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3cardtobx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3eyrqxybj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3banjyduj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3nlahqlnx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3tgylewcu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lallrpzs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gtpcexbj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3emtpkddt.html


<!-- 参考信息 -->