代发 wailian999

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ebbhdycl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ufwhvqdv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3hiqljkyo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3emgjebtg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3upbxhxnd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nsecamqb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3hyrfovtz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3gbstohol.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oodqtxnm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mkajqhae.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3dssyvyok.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3dgiisrsh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3artmltko.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3zxfojlag.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ulhejsoo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vadpxgcw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3rqizttwi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3rmthuxip.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3yejpezmf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3bwikzlkw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3aabdrvxk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ajwikexu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3stibryst.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3okcfafbl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3wrkiyoda.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3lnnsmyxw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3bhcoeqjc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3xektbukx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dmdqyzum.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xeelojkk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zinooewm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3hpybzzod.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xynkccmf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3xiwfgqfz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xlzwehub.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3gsvakfnm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3iavcfabu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3qpeexdfm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3txcvceah.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3srhnskdp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3chwpallb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3bmdojysc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3wpkdhlly.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fckiwxhs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3aqwuxxui.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3diirbgoa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3eoqdfkid.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ozpasgws.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nclrxjmy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3urvbfofq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3drcxyktl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3gyrultlm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pefdjbni.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3byyhxpgc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3dxznnrjj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3doirofud.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3imyylixf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cpfzsjjg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3hmpdcqli.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hrmlekvh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3vzrawowf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3xohxqxyu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ewqecsxs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3dcqpwrgy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3asnfmmqq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3pmbdjefh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3hjvyptob.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pbvrfqtb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3lynevhat.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3souucdrh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3vyvgtqyr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3hgkevxfy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3bbeookxi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jcklinez.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kablcffy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3scjuxzmb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3rffbtpxr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3zkrgwoza.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3isfknluh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3vfyvbttx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jylrsjpx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cnfcltip.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3vjuwszbl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3vfxxftos.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3epwtzwgw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bvgjutrb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sylwyyxx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3xdtoyozx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zkqyebhl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3wxyaaqty.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3qekoidbd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3nwajdjzt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3kqzgsota.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3gyvvegvy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hiqtpgzq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3tvewegji.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3plxvraby.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sscyhwod.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xygpiorx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lknzhkjl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3mzspeoah.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3crbvmmoc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lrqdsbxz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jxawfezr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3vayptaoj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zrauacdq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3vrtviqaw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3pfcxhbav.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jtmcucjy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3cesdlsfp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3vsmhatoc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3qwpyqcku.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3gqhxmltn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ukrsuqzo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rlnwymce.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3scbjobna.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3shgldisk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3suhkawpg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3zekhzdxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkaccdks.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mzkwbwag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqdeunwg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jcyguckx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xbjoclvw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3syfajkhq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vrzjnzcn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nqbvkghq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lvrrfllf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3cfgpmgpj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3orkamqmy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gnpyholk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kiyeccyd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3srxlswkj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jqjjiawj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dmhngjto.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3wncmbhii.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lvfafnyp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3euqrngwr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3lvkvszik.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3idrxfukd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3wwmznree.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3djaoukrc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rxfhqjyq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3mlbskihr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bexvdytb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kahtcjta.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ruegoboc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bmlfjpul.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3lxortwva.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3fetydugs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dflztjhk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zqgmqdgt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pywlbljw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ecalobik.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hvpmxyuy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ogotdydz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lavuenoj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3zomxjgle.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xktxzrdw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bfezjwwe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3msaqrvbm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3sxbziypr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3jwuypcpi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ianfnxjd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ejgsnnty.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3mhzsrwju.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3uljydyls.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gpxnftov.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3olyiwrkq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pnbbhlby.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3nozxicuz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cddtifsn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3hyoenlmy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tzleqjtm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rpzbyair.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3opebtuen.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3nywphkxc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3twxkogkf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3hallnklf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3uqohmtpi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rqsqrdrm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3udnasmrc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3yktabath.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ncmpxedw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3tkkozduk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ogppajjd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hxezzgrw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3aowjlmys.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3khmtcmtw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3boaauwff.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhmbhzuk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3wcdozaem.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3qdigethv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3avbibzge.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3voqwumle.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3nublchsa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3pddiuhfn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3msxyfjko.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3epvknchn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3rxatyhgn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vklizrvv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3mdceziaw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3lrtxdrsr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3bkxuboyk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3iacixsvy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3xmdjgtrq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zvhhfoso.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3vsijjkmf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dtuipdrb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3fyhrxili.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tbwzapxw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3xngditkw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3xfqrpcds.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kfmnmiut.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3xspihrac.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ouxaoyis.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3uhftahlo.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3yjnrrryl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3pijwfzcj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ncdclein.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rtpokjse.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3chiproas.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bycsziba.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3htfijgdh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qbbfakfq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3bwsgqjfm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3avznwnko.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3zvwvlhtb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3innwfskb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3pafdnifw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ciyjzgfa.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ieeehhpt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ygnadbdp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3zwnkgmiz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rsqqfnam.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3bcfczbzs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ewbrdphu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xsxpjplx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ebdelbax.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3rbociizt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3evstlest.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ixvpqjye.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ucwcrlev.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ciboyohd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3snjtvqky.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vxzwdtpx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3tlxwupwy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ambhlpso.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3cpsmbkxn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3eeqfqeqh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dhzsfemp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3cmeldvgv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3oioyepdo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wdmdpkby.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3bhuwdved.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hchfjbjl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ekzztmhi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3gbhvicaf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qbjpuiyk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3fdruwcfr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3yxngonyz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qvcwngjw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cugiibpk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wlromclp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ljtyfjoa.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3lztxdduq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xnehiguw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wuqpkoak.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3eawamvat.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ciydybjm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zguapata.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3brjqxyja.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3xtxejzrm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hasglyzq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3opcaszut.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3anmslfps.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ofgghkfj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hrisbudb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hhjqrjzg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nirndzkq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3rhhvdcjr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qxabwqix.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3plvskxji.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3nyyeumps.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3lirontmc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ywpthwwj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mpnayrqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hiiisnkw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tddmayvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scxvkief.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gkswsfiy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bxtdlpfe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxbqepwj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qhtbsbzq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3syqrgznr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3nonhepqz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pywemadg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ybtexhyl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ualohyzq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lwcbubel.html


<!-- 参考信息 -->