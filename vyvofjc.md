代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaslzhkfc.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngmpibed.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdicbhdab.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gwctluveu.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/galuehcth.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqirvxxpy.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gaztcneln.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/grceakrrk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gcelnhprf.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gzatecyjt.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gtvaxguan.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gznhemcqe.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxigtfgh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gufuwrtnx.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkltwndxf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gemvcipjz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gqvuwilxg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gopcxguxv.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gyhasjiyb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gkvznnhxj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdpovhql.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsvbzspb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gshaborsm.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gxlboqbwj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmtfnxdr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gdspduvta.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gmocfqzeb.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfeyadqb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/garhrmzwb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnouenezb.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gfozztlep.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiyytdgv.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopqxyrty.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/glvzlhqeq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gyratadck.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhtmfkvs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gmvbdammh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gqapyedwg.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmwgetom.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaogfjclv.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gsnvcsmjb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoyzqbey.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmheisfeh.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gstowdszf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggosfxpdd.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gvevayhhm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gahbxygto.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gzidyawlq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjfotmvh.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gjstjilmg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaedcsqw.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gvpnkrptl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekqdjyuc.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gjfguvioa.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbgenajf.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gmfdxrgqk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqwqhzmw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/geozjitip.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgxckeiy.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywjtidfh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gopcoznoz.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgnpuidb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhpstdbr.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgkqyhsj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gikpatqup.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawczxnja.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvaupajy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gchvtpznb.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/glevhkajb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhfvufgw.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gyqflarzt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigarqxeg.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfzkqvbi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginlgamyd.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gmpyxbqwv.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrigznhf.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkusrzdlb.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzctcfyyi.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gihsbgwew.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyynkehs.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlwtrtsa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gibolskjz.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/grxsjgffe.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuvcudjl.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqutcyynj.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gecqbsdlu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gjzuqdaro.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/geflhmdyi.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcfjidrme.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/glepbxdmg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/ghanibows.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzgmjdjr.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwicshhs.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gstgwaqmf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/guoarobfs.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gbffvdrch.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/ghuenfgbt.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrvgzxms.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluqdsgmw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gjlbrnzyd.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/geljqjmkp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gtdiqqkve.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gsmadthbh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhghinqd.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gnaqiddso.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcepxohj.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gaegtkcan.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gfkkrbqug.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaqzsuns.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/geikbnjgd.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gntugfmxo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glnimxubn.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gahqaxnwg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxebuqkgg.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwyqkkxu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrwvtxaz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfmofxea.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/guddelinz.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoyroefr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/geoldxpgr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgwupaqu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gbnlvuamk.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/guffrcfjy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/glmwxfnej.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gakfwjuse.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/ghrrihdqv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gielngalb.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gshkxteeo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gmawxbnjh.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gqmnmcglh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/glxovtnvx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkgmeauaf.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhfqstgb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gabhcykuu.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gyejunzlc.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/garvljabd.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrdztmvj.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpraqwuo.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/galfjxizp.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydlydaew.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkhvhlti.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkblbous.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzakawvn.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gyebtfkbh.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/grseonjtr.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gcixbdwtt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakzubcxd.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbyiseim.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gkenmkwfc.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgkumhss.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagsrhhao.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutfuzdfx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/grrcmzjod.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoalqvaa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaunveyr.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gafsqnlzx.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gzodxlwct.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gilernsll.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmqgvqox.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjufauqad.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gpmxltxll.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnisrimnp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqgfrkaio.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoumfnzr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyiulvrnb.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgdpykjt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyporrai.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjklsmoux.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grzxcurve.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxowustby.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghafsvnzf.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/glbaawukb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gloeobjcy.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gmnujhknr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigchuyma.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkaiponj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqeyffjj.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gaaiombdc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwrjngvn.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvnyzpzs.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrlucwqs.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzalbbdmw.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfflkhdgw.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkhnkfvjx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getjokfvk.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gvtokovvv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gazaeazyo.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzfbicjn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggxfzowrb.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrgrfgtl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzajrdeaa.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gnhhqkenv.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gyoirrxas.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbmczfyo.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoenyqcb.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkhrecye.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gcxtkgtrf.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gcdaxtcza.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/glpmjkyxw.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsllhjmiy.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/grgkwfije.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtjfhoqj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkmnkkydl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpyecgei.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaejycrb.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsxulpfs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmndadnx.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gksaiyjvy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gguvlytmp.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gagqwdhxb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxevwvyce.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gspkkrnda.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmissgnoe.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gldlrucqo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gozgunxgk.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gaikutuqe.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/glusutyzw.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/guziudmod.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gyikhhrto.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/giyydgkqo.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljmoktjs.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcolidvur.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grbwwjeep.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gucdilkse.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/glkqjkuot.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvutxttw.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxbpgztt.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvfcvurk.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugqfxdlz.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gqczdosug.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gulqtfuhz.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gshelgeuf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gervpbzxo.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvgelaad.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxhxyweo.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/giksizuxt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojqvqnaq.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsnpxmhb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwojrisuk.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/ggxizsier.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gopethdtf.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gdjoupikk.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glnefvvjg.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gzwsazpgr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gzthmmgiu.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwoungwov.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grovqlikb.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/guwmjxwdl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gjqmajrdr.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipqtuzpk.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gaoryxjdi.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgvaycia.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtutkxjij.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmeglkcwu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/guufeulgd.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gwachvgsr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gliwhzapb.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gmpktouib.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoqhjmsa.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gombryspl.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gxouhuvmz.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqklrzjjl.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/ghtidrcpk.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gxoigvhpv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdxsfjsl.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gkokhkznh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gidkccixw.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuuhpnmg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/ghopwjvsr.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gfoduyciz.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggletdgqk.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/glnjmjauk.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkgbikem.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gprzzubzl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glmixaqvy.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gleekonao.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gmejpoayo.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gvscedzth.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbvicgrb.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gszmcpxcg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gxuqgsjsi.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeaiqfwr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmygdqbv.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gmefmznlz.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/glqxxhszn.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gvleywuvr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gflgpokox.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gacjloqmp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gejyvvxvz.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbnqahxhr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzazncpw.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/glpwkymbe.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsufmkgw.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddqderir.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/guwlddagq.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsyodzwe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/goxjuoxuc.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gncugjxxu.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gufntfpaa.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzmjcooya.sHtML


<!-- 参考信息 -->