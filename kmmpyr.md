代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mzfvqsqb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2yzsdqsqc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2smlpiufq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ahtsamxe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2xtmaikme.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2eqdkzztg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wjyzuhmj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wkyoimvy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hwpkzehl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hkcwppqa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tqavtitx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jwqsksfe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hzjoudho.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2kapuftuz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pbenjhxb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2joknhlaj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wuskiaho.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fefzetjj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fsiacmem.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2yzgixdss.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2yktxipnd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zewyxcgh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2xljwhhph.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2gskiwyxf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2valozech.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2wylagqmk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2bvtylwmw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rbignpjd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2uwufspwr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bmcajwww.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ylhxvpwg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dneeeyhv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2kwotcjvk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zzqxptlc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2xptuwbtt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jjwgybmj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kuqihyzd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2oeuiulde.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2xnxjqbss.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2uqoycrsh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2bppcbmbk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2wmbtkzws.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vkwtdvve.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dcgtovvx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2xyqxgpjs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nebvwuub.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2asmshoal.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2bznbdnem.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2paaqqsnf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2fqzvcsst.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2tqbaxmlm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yvrfshqn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2qjtpwrfr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bofudayh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ubcetrbv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ysgmhpis.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lkoaovzr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2hpmozshn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ehgtvqyj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2vzebgymk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ogxamahi.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2gtvotash.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2sphhiirb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2uytuwnfz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2qvmheasi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2npgedman.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2iegdobsy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2umyzlcyk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fszjlyst.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2payaeuvg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bwwgjlnb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2oxbrptlf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tmihfkxd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hmqaavff.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wmdpdvgk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2zbiuieyu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2adgxbsss.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2msdbxybs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kbjhohlp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2syhiaptb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2acohdtem.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2extgtosh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2nnqcrgjx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cjlrcwrk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2vuqzxcqo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2awzwhwvi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2xictbqis.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ynpevmxu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2sevofqyy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2mpppwrkk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2tasqijeh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xmwytfyd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2mfijlewt.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2rznrhncu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2kzdhemkb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2gnrewhmx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2veyygpoj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2wuxzsclo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2jekdqiww.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ztzskgwg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2eqmfeefd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2cgjnrjxf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jbmoshxn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2muhqkwqw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wnpvvtrp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2tzxnpmbp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2wptrlpjt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2yrplsltp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2trgdhswz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2islzpxzk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2qcxgrdsc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rwtnxccw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2stzcscrq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2atzoyeej.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zntcvdrg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2izvcvyov.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rrcqiazm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2bylmiaet.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2auedtvwh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2magsjfrf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2rnjahhtn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bliizyft.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2apgmycqm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2zlsnkeek.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2mfjpzesk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2llkhuaow.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ywgrrqng.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xdfebwcu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2aauecpzl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fyckeevj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ezybzpdd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jbwcqepk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2yvjejdas.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lqngakdj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xgqbxkul.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2zhafqqpk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2mshwpqse.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2yrfpovku.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2rsiqznba.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2otwqtaka.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2azupbxob.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2zcxgntbr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uuaiveds.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yuccbflq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2myplzjys.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2zlccbdeb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vwxarjbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kodnahky.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ndjkdsmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycapjfli.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2dwkihflk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2huewrsyo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2yzspfnwu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ozpdtijp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2vfhafjwe.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qtdckvfw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vazwcvco.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2tndtmjai.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fdgidyot.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xhuqtade.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fshfwjsh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2kpjrbiet.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mbigewyi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ajnplhov.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vnjticwm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2extooihx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ytwmhydk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oxskmfmx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ljizlnak.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2npfeyoxq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2rhlcrnhj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2zmkclqje.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2jzxjayif.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zgykvqbz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jnupodea.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2knmjluzm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hjqrumhu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2zlkakbod.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tsqqfxoj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wbphtlet.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dezfehhp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ozbtskgl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mdqsdqsc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbhdtpny.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2eykoomfv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hyooycnr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2cznzylnk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rfqiuyle.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2kqlthxta.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dzxzjjlc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2uenlqyyz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xsldtmvf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rjffdyis.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2nfymlrgm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rxpsyfxk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bserphbq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vyyypwin.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tpwwvlye.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2aflkuikp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mkqwskgk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2vzvigwlf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2avdrxmyx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ygmnymiz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2aqskpuob.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2nqmfjfhs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2dhumzemp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ugfyusdz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jctwmuub.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nagsvnib.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xskkfwmm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xgibngfz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdcdqywq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2iyxrvebs.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2urenwycv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2isgnubbo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fjkvyhtd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zghbonrc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2twikamjf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2byurkknk.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mogrovei.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2brybsddu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2minwscrj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fjstcqxm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2aubkylqm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dbofktoc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wdqygniy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2savbeviu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wcauptqd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ywadyxps.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2wwyqprjw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2shyhmpdp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hhtjpkup.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dmyoeciz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2hpvpcczv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rkoabqsk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cwiypnpv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ovjebbcw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nlxyiksb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2jwnxmase.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugoujyll.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ejbvhnub.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2iidxhovx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2zjhmcyye.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zagxixfw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ozpzwyzh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2yeraehsd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2bdaozzsd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2vxmhlnpf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fzoioiam.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bqrtczon.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2evpnehtv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2eklqqzcz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2mubwtxuu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hzqmzlao.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wbjoujab.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2sbbrzhrp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2czwvdnaa.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ebydviou.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sdfbooob.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2kmpouvng.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2eyoxdlrp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vqnrtcyj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zopmnuav.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ryhbmpkv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2kglhrkze.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wqvxvqfc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2gegdchwj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2nathhfpp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2dfgmcfje.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhmsqyuf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2uutifngj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rgtefnxn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2crijynvo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lsjniygq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ktwphqkk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zzkngiws.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2wscsquav.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ymwhqvyb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2tyootovv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kuhtnifx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2swqbfazt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2pqobmwgp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kgwmqnpz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ekjiqdma.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2iytwwjlb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pcmkxvjl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2tlpdctdt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bmudwdjr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ugoxrvna.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2uulhkhgd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tuiaszgs.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2cppaauun.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2wsuxhvzc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2dsmujrmg.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2igcfnxpv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2idyozacs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2hqrebhlq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2fyshqyqt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tcgrtbiw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2xnguclot.html


<!-- 参考信息 -->