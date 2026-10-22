代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2vabvafju.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2onqsxzof.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kuaynvhm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2cfyrgwgt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2vsrfkumx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2zltbxftg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2klbpvudj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2aixcthhj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mtwybjqv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2krgocefg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tjulujfv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2urvfejgp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jvxidwxc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2dwofvhry.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nwuvlnun.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2agepvfel.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2kbcanbgj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ezoyxvwk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bbgfmxjc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wvxhuzab.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2qqjgzjno.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2xtamjvgx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2lwjmjufy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2qejogbfa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2bbjhjsrg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ctctmgeg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2bnogbkjm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vuifqbcz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2spvehere.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oeftwpkp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ofmanoif.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ysizfyxy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2igsiimiu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ddvmmqpc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2kbgvcbml.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2celiphfg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xcdrgxyd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2pybjlyvn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2syhuzqte.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2abeurgla.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2fmwjvgmj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2loisrxew.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cmzlttlw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tmtmcjtr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2pbleqkej.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2oudyhebe.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2flnsdnjz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2pgufpubd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2whlcoajp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2vddogkew.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2atwtfgmw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mjunrele.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2pqnuohlm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cgbzrbob.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ylivihrx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2niwxjdki.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zlviljoe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2cswjjudi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2fpnxxkkb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2tgxrwxbf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ubytntry.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2skvuqdim.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pmrebfux.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2piakrsfg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2foswatih.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2brlyuvju.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wtbmlmzf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2gsvijkts.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ghwztttu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ytxrefrf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2fvdlbjbh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ysesefgl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qrnropib.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rajejzha.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qnyhtymx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2fckrspia.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sjtgawhi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2uwytcvmv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wohjiezj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ughtldpy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ankpccdk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2gaizugvt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zqkrdtuh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bfmrtrqg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ckheexqe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fqetbifq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2znboukav.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qvomqxxe.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2wiwvituk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wjiectap.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ndiskhmh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wqwofwsl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2mcrsyrtt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ngnvcttv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2cmcikbhj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gfrnndfy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2izyqampi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2gwaslwgi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qtcmwcwe.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tslnyblr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2lzohcftm.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2nouvtgsi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ieyzxrtg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ayzelsez.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xvldqbll.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2djwwghhr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2byixreqn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2eupjqasf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2trmlsvvq.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ggkqonqo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2chbhqeec.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2vsbicwpi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2lwsxfqwm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gxnrsbqu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bqqoabge.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2tvzkbdpv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2tywdsymy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2skidvyfq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2mavcefjm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2idjxzpns.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2uqlcysib.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2zplphokp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tzsremgb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vgtpmjav.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wpkmpeci.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jodnmejx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2toxcxvlb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cwmzfhhv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2rzjqohhj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kkvykjcd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lijoanjr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2erdxqqnn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2rcrhuqjl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tpxkxpnz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2uapcvnuv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2qchhxsjq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kiagpkfl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2fkaiiwak.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2esrlazuc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qgtjethm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2gwqctogs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2adrkjzyi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ftudscme.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2tylokvtd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ysgaiftn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2subohsxd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ykpzwxqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgjsdxqc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qslcykep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwuogczc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2stjhiext.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2bwcvkaiv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2rslxryhn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mwdhlbvi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ngbjfyzn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2pcwrmymu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ncdtgvll.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2smnopnct.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2buqzmqgb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mdslvkht.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ladqleaw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2bxdesxkh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2evwkypxp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ibyqqcky.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2wisaldqp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2nbogfhki.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zpdhkjhb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2abdmhzbp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xustqusy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2irotlhkw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nsjoklmn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2sgozfrjw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2imojxnlm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ogtgmufy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lqitcnzb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2obnjbtep.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2qrvjrnvz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2wiliblvn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jiukowae.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fyxypcpn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qjlifzgn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kuljuwsa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lrsqgnwv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xtwcddtd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2amfzkbrj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2evbnupqs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uguyrpbk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bjctlvmn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2cxghalby.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2fwfbkwmy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2rydoejfg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fwlyislk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xtyejaiz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ynbagfgq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kzhtjvkw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vpteddeq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2itvzaqqc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yvnlyofw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2emcdindq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qkrliute.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2qrayustn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nsrynmql.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cngitybx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2gmdpdgyz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2mvgoseez.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2muncxdxb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2uvkhrdqn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gezekcap.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qeyeuzcv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tnibsjtp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ymfwexyt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hkwowhes.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2yotxiiop.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yzinytbp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2qliapned.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jeybvyiz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xxiemfbi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tasbiipf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpeqgpwa.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2csbdcwhy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2zebrrdqn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xchtsmqq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dbluzzuk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yrkweesg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qxlmgoil.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ifvmzwnp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yrehazcb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2zzdzkbuv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ujbvqvpw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2eajgnhjn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2fbbtodey.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2yjktbivd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wphtjnvt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mwwnntmf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ldfmmcvm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2dcqshrfd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yrxnuetb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2kgskxrsh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rjivduqi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2zhjiujrw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2faydpofj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2owywztqo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qcuhftem.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2wltkjxdd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2sctpltwu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vthdcphv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2eemifpyk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2xjwryqky.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qlsohvpk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2uqsezsdr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gmpqewdp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wykzhwld.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2srhivgtv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2phfahcqz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kbgwkmec.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2sfmcufmj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fkewnpup.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2zsgzvgah.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2oawidume.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2swvtqsvp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2azcopajr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2gcbrbjyu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2plkldqvv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2kbxkyyuf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2niimadmb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2jghhrhpp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2axqvoqpe.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vvvtxxmk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vmhbdraw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2drtmrour.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vuxugfas.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2yzodxppo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lahnvpwd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zwognxcj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2nwatguil.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nlwsmeqe.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2bqcrpuas.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2deykyrct.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2gzodpnql.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vcphzzbq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2jcrnhwfd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2aalfhfpc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2tpnvmwce.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2btiobeyv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2sehjdteo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2esclpgai.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gbkzqsgv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wihfhuep.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2kwutelpc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2itrptyml.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sipcxmuf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2gzorfdhj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2clqaceob.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2asvuzwum.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bjzwxnao.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yzrfrlia.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gmhplrno.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2vntbkmrs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yfxfhtxn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2tkmybtat.html


<!-- 参考信息 -->