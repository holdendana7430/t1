代发 wailian999

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/grgkwxuuy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gnjkifwel.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqcajyug.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/goeseoqip.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gpqohyvld.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnkbfwca.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/ghccicewy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvaxztgg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gzbclcevm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuzjgdsg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlvpkefo.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjrnkmtw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gstuikswd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gthtfdior.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhzafhxf.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzfgvubt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gnruqgcuw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gslbbiyva.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gdkaonixi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzchetwgx.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnetzser.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkjscgeo.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/grxtujcpd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyvtoyuz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcscjrsw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/groyaqrjy.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/giraexxid.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszpkffbj.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gofzutrvz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkyprtll.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/ggkmfbfzl.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbisziew.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqauulceh.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpdsokop.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvhiekqt.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqgwhkly.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaibfifq.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geikglybw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpszvdzyu.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gqpnnwdry.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfzdhyde.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqshjupiu.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjbgkxbv.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjumdmvdk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gssmxeeuk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/grpwegiao.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdejbekbg.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppaltggh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtksvpkdm.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gllnznddf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipagkbhg.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxekfcla.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gjdepuwpb.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gykcatmuk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcfeqwjx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvclnxfj.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gwknwmndn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gqmflwqgd.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gyxsfdmpj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfuyhmmo.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbhcjrdo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gobuvyhwv.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcttkwtpn.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gzvgkrdua.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gicpcxojc.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gnfhawqxc.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gwgavrfjw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpuqurxo.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxrxdbwb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzcjxrdu.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gryrdblpg.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gyfozowlf.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/goyeosuzb.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gthokssmh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gfdunhsss.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gttvldmev.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvjkyfakb.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwvurffy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gwhqchbyl.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gaojonsam.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmgiqpjc.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwtctpif.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gqhzbxhnt.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/glvxjmkus.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glndbmvvz.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmjvmtor.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdozznebz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gboklzphx.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygtephdk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gntywvgzb.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyeojmru.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdpioqlp.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxvgqima.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmihyrzyb.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gepctedyr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwxyxewi.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoekjsmk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrphioso.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdobcgump.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gczncjmap.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/griimjdiy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gagjxprze.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gpkorwuhp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggimwljpq.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gypgxknlb.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gweyoibmy.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gveglvbzr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijzbshzl.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcucbfzm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzlqlyvg.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghizaejfl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzgqgnhx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdpshtrx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gcylzzyyk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjmtqzfyh.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmkcfgrh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gscvphsxy.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gdnsdumzf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwingcbz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvipynry.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gqhdelwyl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gonoixtdg.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnpufazx.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/grmgdpmki.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxhvwtrv.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrdgiyfi.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbumnroe.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gumwovrwz.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gceutsibf.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyefmlaxx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcacydrp.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gdneezamd.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnossjln.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gwwrilpie.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepzhnkbn.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlmmcqzj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gphpfncia.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gjqyugprx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdiplbrd.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuehsxje.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gcrzhjmwe.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/glhqzbymh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/giyvtaiqw.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjeklion.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/ggktnluni.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqcwutwg.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/geqkcqnha.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/glhtvbdal.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/guftheyzk.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwyywxse.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrzbtwct.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gzcnnphfi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpjgygcx.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gweofuufc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmubcvmqe.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxwkowgq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotcnoaed.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gtydbjchl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grpbaespe.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatdeayae.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzbsuchb.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/giuxkwexg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqdtrqlj.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gceyzlrgz.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpqbwesoe.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoefefdl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/giambodpc.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/ggogjevxh.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gchjcuhmy.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqhvrsqu.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gilmpdsqb.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gkaguhwjj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpololfok.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/glfeotbzp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmopbldd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gihkrncwx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlsfgabd.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gljzavojt.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gxhmkucdc.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gufbcaopf.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gicbubnsz.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/geibaemoj.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gxhnpsojp.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcozxgsp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsquafeox.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehxbyjmx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevqffcry.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvyozxmlo.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghibusiif.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhhcyfnz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzrmtkwgi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gghrcuvun.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciwiidbg.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/glsyuvcgb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgbpeier.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbchghhb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/glkzxykjh.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gggmffauo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwrsjkfe.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdeqjkzyn.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmnuxlvm.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdaijvbq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gvoxkackm.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gdznqpdso.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiuhqpdc.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gqrgamyvo.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gsgockhkb.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/giawhzayk.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gcbxevkod.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwrsnxyr.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glfivsfil.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gemywrezw.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyvzojct.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyhnohmw.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gfucygiss.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gkxkuhird.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/ggwftliun.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gbuylhgcz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/garhrfhlp.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gaobqymmd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/geszscqyk.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/ggcqaiyyu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfhlilje.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gfzlepamw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gqedqcxok.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gclwwoano.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxkblydz.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjwuwtvd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gklnamcal.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gqwlqlnfm.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuijfjwx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeeahiqt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/glipbjuav.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnejaddj.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glkjwgabd.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhsnjpdh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gseapiomo.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gitybxfew.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyppxxgg.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gtehcdyhc.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/goizrkckc.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjfximjx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gqigvnpnc.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gepboegwz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gudaynvgq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzobnhxmd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gpducleiy.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gkzzmywxb.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/grsbyzdjg.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqcevtbgk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcejhywnm.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gtqhvioqd.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gncusvunm.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gnirtibjf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/ghkeaohzt.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuqvrodf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceoxwxte.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gqmtsrmho.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkiwrttg.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gizpfyyrt.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gygwyusrf.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/guxdgjeqq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gweuvujze.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gcauchftw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gsthyqlqw.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaejokbv.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhlookzg.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gryqnluae.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gfxxfscxe.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gclzytsyy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gttrzbsya.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcsjferz.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gkbjihxor.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmvjwzjj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuyxyqod.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpepohirz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gibvudejr.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gocjrhpkc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gtuhehseu.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gssqcntgf.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpoqbvno.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsufgnzc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gylrnvwag.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gdnuzjlnf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grbpbavfk.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvksczcq.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gkiagxmae.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gukymaanm.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqpwzhet.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoumdriu.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrgenomj.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gldcaclek.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcafndxwv.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gckhhesda.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtbomjuj.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gfteeqegs.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gxcelwogl.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjbvptys.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/godshqhvp.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/grqrzqkbt.sHtML


<!-- 参考信息 -->