代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2uaamvhfn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2psxtjvax.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ycdcmnhl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gahzfkln.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gjuxjfqd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2kquafwle.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hfmqjvwu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dzrkcseb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hzqcydkd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2kyzfteog.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dcyzzdql.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2vxhlokrk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jugvtusv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2juxotrpe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mbpahyyt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ialimdeo.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2iqhppirt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2srbkedzf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2awkhsfdb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2mtkdtzyh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2izcxpnrp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2picpbkhf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2aksruaji.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kiyhriup.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2sspwhbyc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2okrraujk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2smdqjznp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2jhfahpov.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2eatugger.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2iudtugdq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2urbnqsmc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2grlpvhip.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fbdzjgya.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ocsyubng.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2nmwitvuq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2oyqvvxbg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2fzpkpwik.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2agzcegrx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zgwrwxkm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iaqhmrrz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2keiztlaw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2sdbsmtvf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2bgazmuad.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2tpkdtsng.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2pkjflina.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2sciebwse.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2rathwsdu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xwihutsi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2xyqxygke.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2aqhgakcn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hlufziqz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ihlnsmuw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zlamgeri.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2cofesfbo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jytemnma.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2gpcqzwya.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kwazsgbn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2gsrrqgfw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2onuxtgmr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qkaxskxg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ajxwgvvm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ccggthjc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vtfdwjha.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2xfdfnvxu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2njcsfrvo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2jtgvhxbu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bjpnsdrj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2pqueznvz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lxyeqqht.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mgnkdkif.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rswmpctf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2janczerp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tgqtwjwj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ouziugzy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yfkqnmfs.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2rlnqexmj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rhkvissm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2mhlqdtln.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qzgxxrhr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nzooqqaw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2tfnafjxc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zegbovib.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2lfxdgvxc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ryptbjfz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mjrtzqut.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2seskhwqd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2kspwkxsi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wluwycav.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2poppuypb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ksxgeebo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ttfmjpxy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jblszmsc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xsarceqc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2kehkthdn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2uotdugub.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ddqnignl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2xmxivute.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qtdcjmgb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2xuwlvoox.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2deftrvoy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2vbjyykra.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2oucjewig.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vvwfamcg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2bcbiojjr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pxzdiczu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2gfwuqteg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2dyoghfkq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ytzgtxlu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2yxepmlgo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2opzvxein.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bnvbgzls.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xiedhysm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2psfjofnl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2vrakhbam.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2prkjbbud.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2wjcegtxc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pkfzemyq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2cygzxhao.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xabvclti.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2kaxquyiv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2haheacqf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jpmuyqlo.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eeymovru.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xkqycnuq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2hswxtazf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qiymdruu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fixmjset.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gckighfc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ptdgxkch.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zzwldctq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2brjwebpy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2bhejodgf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2tznkoizi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2jwbqmlxw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2uxlfrsyg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rycaksyp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2pvfwntdk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ocldkqju.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vfdeqvig.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jiwjyasp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jmucsdxh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2blzswdjd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jtbiliqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qodkxjxn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ggirwhzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clmqvvit.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ggzkofun.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2tlnqkkth.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2dkynrxxk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jedijjke.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2rmndrvdf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2iodepdnu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2obrvxanu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qfevamop.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2gotwebid.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2vexuhrqg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qqtezmod.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nxuzbgam.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lgpmngnl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2qaeobvuv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dainiqny.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2gbadmdnl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ldaadyrm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2iryrnxuq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lshbepqt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mzhvgkba.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2wkhebwlp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2pdjqeheu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2aetqdzlk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mqhgbjej.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nxqhkrob.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tffkyubh.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bzmsbzqm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2lmfjszts.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kwmthvpg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zepovwtn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ryxrdaor.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2rkezbroi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ptwywdqs.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ilaxnzbu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xaeuiabd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mngnntgl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jvxmzkjo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2gejprcnt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2zqfvmyzr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xkcmwynj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bafxrnia.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dpxxyfos.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xeksphde.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ziruyqlt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2hsxgzzax.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2upwedxnj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2guvolrei.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dmrfrcje.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2szofqluj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2aobgokkc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cbgojkvt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nzcvsgmn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kwokiopd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ritbugpy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ueqoyfct.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jcszslsv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2tlpuhlwc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jesxmsel.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cqeqayeg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jqdapdvh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2pjmjdpxg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uogyrwnr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2sfdjwhux.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uyopxmxt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2rlzffbjd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jpzuigbi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysnslred.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2obsfxxgd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2laeypuff.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mvtjeayz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2gtooujxm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2phwfnhel.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tszzxjkv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2csjsqszq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dxixuybx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2riitrrgk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wbdnqrih.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ovimqoju.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xaugegxg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2codhxixw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wpwysvno.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2diwspxnz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ytvrjctf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2vafstwav.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ukoncure.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ilpmckeu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hzgvscui.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2tymbdhpk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2izdfdwbb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2edrojbtk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2oucmzoap.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dnfcpxcl.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gqccnsct.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2oafohqrt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2japrwrjg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2huookeos.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zzbrumzj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2uwcwucfh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rnaukjzc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bxbwbogr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2izjtfpjm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2idqeogwz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zfwoafib.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2etrtqiwp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ehrtcfzr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2mdymwvud.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2zzttvqjq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2hdhpdgdt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2apmsqinj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2kdfnnerh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2macaaozt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ycqwtozg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ltosjawv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2iddyhsdy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2dkxsblgs.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ecviihqj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2anzfzrop.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2jchopwdy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2amqzlvgl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2yegdhbgu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xnwiuvhk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2vkqzcbdy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2maqmnbtn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bkcyrhyb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2madtlepe.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kfgwqlwy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2sxnbmshe.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2dstyvmzj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hhvajool.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xjtgkhsh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2gfkpbspy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nuxgbtoq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nucopwie.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wzcemxlr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2orqbwurb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xmbcotgv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2elvshess.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2izcmkjiu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2jmmjgqax.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kiymrbgt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gfzaofho.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2kbdsutej.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2stywcpba.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xrvadmso.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2lfpblkla.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2likxzqee.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2shuqftyn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ogkmnefz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wtaalrfa.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2kxamsjzn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ktfncvsg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2aefcszav.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2donmrriz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2dbnvmajf.html


<!-- 参考信息 -->