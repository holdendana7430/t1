代发 wailian999

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ibnjdpab.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jbpywtwq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vqqvqrdl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2rirdqenk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2kfsqrrkt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2sezlxfoj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2lnojgaep.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hqzdujbe.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2rsjbbnkb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2guejzoee.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2dmgkkriz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rclizndm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2hghmgjzv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2lgcwbqwk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xyjmqgwk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2rsynhbah.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nwbpazed.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2wayohuho.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2fzkdyaqj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2pyidpnpf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2tyvwkngk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2pnbtmcrz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2qrmslnhm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jqzvjhmn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2bwqktvnz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2nipiepih.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2lettvuod.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2uruphwvg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2uoimigby.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ugxkyrzi.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fwgfyvoc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2inmxubdp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ezkcqrzv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nipdtmbc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2crrmhflu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ajaztznv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2vxhlejfu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xqngemua.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2sqknlotx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2wopvzgss.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lmvibohl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vdwfknvs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jctgmmut.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2eyqhpzwz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tzwcnarb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2gwntluwk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rmtfkthk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2krtktkjp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kzvjdpab.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2hqztjoqo.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2vbkgndfd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kcbqzbvl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fneqxejd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lbmqspaw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ksobebxa.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dxptqsge.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nzwqxsst.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2lnyrjdfb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nfagmjik.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2mthphaes.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lrfgwigo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2jybixtbo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ohivddha.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qhdslmik.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ixtephif.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iuwssvkx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2konhfqlm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jkilqazo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2vuujcvns.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2sfeleexn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gcgwluhx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2uitnvfwo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2eygmmszp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2szcdaefq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2twbcrixc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2hakweyiw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ximcxuru.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2kwzoazak.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2bbiphxza.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rkkdcnpi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2qkyqbayg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2kzrmbhyl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2rmgaxouk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2busnwnwz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2iovzfvpg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2qmibxmaa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2mlkhgrhr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2mupjbubu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dairirbc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2aaweltez.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2gmgypkkq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2exsuepth.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2vswkffqn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wjaqfgnw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xmccwgkb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2aolnfrjp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2mbrfejuw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zwrninyr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2muhysgru.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2kjbjjrea.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2vnxliiuk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2bzrxulmb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ombuxbex.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ubkxviez.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jwyksjlq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rwabegeo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2htteudna.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uzwjkips.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2senuavzm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xruadonl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yiiidvva.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qmefdguq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2roxtrlvk.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tgcxvhen.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2qawwxsgz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2zdnpknvu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2lexcmokw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ckxfllic.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2miemnxjn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ugmuyijz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2pozotabx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2eqoegfrd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xsheemya.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ghydktit.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hvwneubi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2whgeretb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2qrdjgifx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iisxuwmc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2amfjvfic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksigfrdh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ujguqqqr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pqsdbxlw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2fkknscyq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2fupltspy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fpygvfey.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2gbzaszip.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2wxwaunor.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vzwsebot.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2gspulsag.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2oahfqdqy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2xlsixybx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ifmsiyop.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lwestrop.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2dhdklzcr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ilzrhjam.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hswnrxzu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2lryhqifa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2asdunqah.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ldyahtzs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cqilsdoo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ewwhquec.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2pvlxytfq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2regtwcya.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2duudgxkk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xmmdowjs.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kjvoupji.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xnukkjvl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2rpyyhvgi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sphxjxrh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zqwytdyx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bgyuvcgy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2iiuypedp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cthpwwen.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zjrkoygg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qeapmuob.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2fbofibgx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wrolxplk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2bdhsezqy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kxktzsbj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2gukorwco.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fvmecvky.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iwchjjfm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rnnroopg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ltdegrzx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kuphhmdk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kvjoaiwt.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2wjoymjuq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mndluhyw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2kxufrhcq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ohmqyqvh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2bmdqcpst.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gtdcsbgt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ybjickdb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2cutakizi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2hxjhvqwg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2phlascpw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2hpozamyu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2uyaepjvf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2npgbtdkm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jjufjjft.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2siuxgcjl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zixvusod.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vccynnxt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jqucwcxa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2aneoqeng.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ebkkecdq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjkzdivj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qfyhxkfo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wnmeofzx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zyfcdcum.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2rkwavbbg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2dwffzzzp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2sgowstig.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2epyzayzk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2fdkdnidn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2dyyjnzfk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vxjnjxpi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2lgywzfxu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gpdrrite.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2idcfjswe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2yngksiqd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2omzlxggu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2djovqwij.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jjfzrpht.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2lwyiezsf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2hhvvftjv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2czrmrvlz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xehxapyz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ssunnojf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2zifdfdgj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2dsujhjtf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2kpuhhgxg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2itkapaiu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2arjweukp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2icohaurp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2xdiunfyg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2cbbbcygb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2eqjyixqf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2odgtjycy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2karzlilr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2aqoqekvk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jistwldf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2evsfjvox.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ixhpklkq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lgposgos.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2oxzehieq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2zyuutibj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lihanqhh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ixcailtg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qkmnkdks.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2evczuxnp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2zqrwrdas.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gdnnhshz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2nowwfrpg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ufabwejg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ypxjzlft.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2yxwozttz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2kyygrmbk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2epmuuqhk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vwbumkng.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2yaoueuls.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vfqjvoco.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2swrtgwoz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vxgrzyfe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2pcrzkpzo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2oylhrbes.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2zhoiauzm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2uzwjwgcf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2defnemwn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2mkksueil.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2fseiibyc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2qqwpjuwo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kebpxoon.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hygbnkmr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ihqwklak.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2zlevstdr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2uaqeulsp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2acdfgcez.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2jdlvphxe.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ldwpndol.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2thlfgnnz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qsjugmeq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2pwfeilcz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2dekzopmq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2yxjgvblq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xnqreqkh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ckeogqul.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2yblzenrt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yvqaagzs.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2joxmlkaz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2iystdyle.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2gbevwztf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2pifwvkpu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hmmdropp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2yhoapabt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2opaycpop.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qgokwddd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2oqfnmfvy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ouhkcsqb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ihxeujky.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2boeltxeg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2yyzmrhqe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2erqrphgt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bdyxizdw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2sjktdego.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtgyajwk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rrveegbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzgcyqor.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gmpqjtfv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2oxjvubln.html


<!-- 参考信息 -->