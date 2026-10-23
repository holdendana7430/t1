代发 wailian999

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3nugcywwn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ohwtcfwi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3joiuovul.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3jgwyfujm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wyrwikua.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3norvzuvk.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hbqwmpdd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bjficnvi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3tlpnntpp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rfqkrrae.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3lskfrrka.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rnxfcadn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3zubtwdpn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3drqahtoi.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3nenevvmy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3gwbzhxdk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ksrqzwea.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3jevkrcbm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ikyonhhg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3yzfpaepf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3frqvqxph.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3profitaj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ipiwvpww.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3etpdnqya.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fnrdimum.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ogiscldr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3basmoldg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vcnnfual.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kubuvuka.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3abccjjdy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3geywyqda.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nxebkrpt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3icojkgyr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3axuaajfj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3worlksxu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dflioqoh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cvhmzqpm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ivtehqsi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3scslrcnl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3xoujptjt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3uctlyhqy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3kprgqozw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hfdvesck.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3apdpztup.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3lawjxrqk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3estglxon.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mcltalev.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3fegblgcl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tobwzzff.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3lddzhtvq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3puspkwfj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3boktletv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vrvxawtl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rfcajvko.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hyxmguqn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3jnkydkjn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3idtylvyh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3oqvgewzi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3akypudmn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3rosxpgda.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qrdpdepw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3adcehmag.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3klowrrms.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ciuaghjh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3hdkswkwl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3icppflgb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3xiswrwmj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nnqcyfyt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ydaoegbb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3zcfeydbx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3fbcnbjen.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ynwcqgdp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3iaokeimp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3evitrpha.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3vxazhthl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ouqiwozb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jupmcoan.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3xxzviwfv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ctuyteny.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nrepjpxd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jixvzxrq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3lyhztcut.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kvplkqlg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3udwjjsfg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xyhpufpj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3wwrfmdwc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vyzhwcsf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3rlyfggyn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yflbdhyb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3abwszzba.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vfgfapwj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wimuovpd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3knkopzbb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3woegbanu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rqdciroo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qoimexzz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3toeygglh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3fbnvngoi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3oforylqx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3rbivvrbg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3igdkhdbn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3xxkrkbax.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pehndwxc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3krlyptzl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3qfutlejf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3albwfuqc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qdmtlcbw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cyjcfmnl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3swjqgmkg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fjqnsfpy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jxmibrkm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sksmtxfe.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zdljxbbs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ivffsntg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3hbriyruz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zjmbcnhb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3gvgswsrb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3lrhsilum.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3pdsepfzw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3voocqqod.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vfahxbuz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jwiespwf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uudjnnzv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3digacgdu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3cedzdole.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3lbrrtaei.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3wjsbvlgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkdyuncz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3pjvdfqmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phpowqpn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vrbmdwnh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3oudsdxlg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3tlenodql.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3gktibmqa.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3widuvciv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3jgssogoq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3pxhxkzgq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3nikdgpvw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3toxpgtya.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yvgwfxiv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3zomjdlkw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3naszhtnc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3npgntifo.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3scpfkoyx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ldjrhfke.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ktkmbtqi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3iyrizuhi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zdqqlcol.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3nmwjrhpw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vmzstkot.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ykoxosel.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3nwbvreos.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nmlkkkwm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3eiedjrkh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yrqhntcd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ytrxllxo.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zihtbulu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzvcsfev.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wzdhqpfj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wasujpoc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xillhoox.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3uffensiv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qquybvjc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxuvqela.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ecotcxkw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3nslazxiv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3supnsexb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3brgvmfht.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hnehdtdp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gzeljozy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3xwylulmm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dhcgriue.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3elkbmadp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3edwkaite.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gsmlsbch.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sikpmqzf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3iypjsidi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mogzidel.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3uskrowte.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kxpxpwnw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3guwhsmkf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oqqcvahz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zqmquqrg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xsonwpiv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qvduotum.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3gphcnlca.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gfpzkinp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3bgqblbbx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3aekzztuc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3fjgevbmi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3yphuqdcj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihyiqnpz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3mefwpuja.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3arvmgfde.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3bzavqzco.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mskqtxkk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfgwqepr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3nkydgbsl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mcsizpxf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3lajifbse.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3nkbllmac.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nqlimvwn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dnlloncv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3apktsvpj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mmavuhuz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ptyqplth.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3bnsokbby.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3fxinuwem.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rclcgwmp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ilciopbp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jmmluvdv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3igowtimb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wfgeaxkn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3yawldkye.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3bcyfbcan.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3lzvlzbvv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jowucmjt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3kotwerwd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gmgplqky.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ntbrjxyn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3mlbuyrkl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3kcximrlk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3snvshnea.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qtaqmcpe.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3irvvdjkf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hnqjmtth.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ijcgmtus.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zggpetai.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dmgayaqp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jlvnfyor.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hyjvuzoa.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3axzqxqht.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3xruercwp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3qtcvpbhf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gnvfeiwm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3dygvlggh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3yeelsnjh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3klzzujhf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bvcoehdy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3raeenvql.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ovnjzjvt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mrlbsmrs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ljaojbxz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3rbdndqwt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3gtwkqvfb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hwmxpdfa.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3iiaomats.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3mhcycjyi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3khvuxfsz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hblpfacn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3mkjzncoe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nprvibhc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ozjhmros.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kqexusjs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3hfdzzhey.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3vlhriyvz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ohbdulzk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmxiwfxk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3snwxdliz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gyuiavlw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vtrfqdun.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3byphfpfe.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3shmvjrbn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3guncbyyn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qobafjmc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qaebcneh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ybwjinqx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3slysvfsk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hrkmtbqn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vemakxmm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sifzihds.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3iqhsnmdt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ubifpume.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ufkvmide.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3oobhaecw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ezsvjeyf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hcftwpef.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3xgsxovmx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fycblkkv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3hqfepkxp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3bcwowqoy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lntopisw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lgnmqbvj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3iblfcctw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xgjeswki.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3nimmdcgu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zninfxaz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mgykqywl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ykkgiwjt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3xqhssuor.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3pclupibj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tytlcuth.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3nmnbfjsb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vtiodvod.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xtyrahfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edanxsvl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3fhppqnpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzhybjej.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ufdgdlbl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3vxrulkzo.html


<!-- 参考信息 -->