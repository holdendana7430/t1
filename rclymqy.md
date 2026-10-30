代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/glrxyvihw.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gxmcmidrx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gztfikopg.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/guwbldimk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmjbvhkhx.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gjfzdxeiv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gcrlqxboq.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gpumhyrks.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/ghizqncoq.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gpvuhendr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gcmfpwabv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/ggliteaoh.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/ghvgyqhgr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/glohtpfcv.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gahvldvyu.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gzuaccqhm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gitvhnkhb.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gzsdliczr.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gmhrstojh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gsfyyrfyp.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/griljmggj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/goxrdcuea.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/grjkptpiz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gnaemcxvs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gngcxcjdo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gdyuseeor.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gbwjabcfp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/ghfvplmvb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/guulimmse.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gtwpmuhzk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gamajrxgy.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gqnkcncdq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gibupignf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gyzkkrwks.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gknwraomj.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gqjiuwyha.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gijikgokg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gixaohmpn.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gctujymtk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/grdhhcvwx.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gobnsysmw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gklnqdqxa.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gpaanjgwe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gbzcgioss.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gvsewzqok.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gvnloqraa.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gjxuywgam.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gjbnzoenl.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gvhcidcsu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gfdsooskl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/graqkuzlk.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/guomreqyd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gzjcdzoqk.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gbhvkcrte.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gfnmzpyqp.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gnyfzyxiv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gzighhxvb.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gwmlntqfp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gcggpujdq.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gxmezlkhx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gihhnfosa.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gynmkxnmp.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gfhmvbxdp.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gpjykipda.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gytvjppxy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gassnjyxp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/glbtgrxds.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gyvzfuduw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gtlzguhuy.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/giexvotva.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gqqtqdyng.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gyohevqjs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gykwzueuj.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gpnzxsrvb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gnewveelq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gguvethqp.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gumretiuc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqxdleiaf.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gtkysavum.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gykprdnok.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gswzsrjzv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gmlesncuz.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/goelsppln.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/ghyuhphpn.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gpxprhdfa.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gfxfszant.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gyrrshdrh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gtxprhvyv.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gxiwfkzod.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gjvjkshrr.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gwkiwaxot.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gtsawucnu.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gqyauliwj.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gxwwumvps.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gskovpqdv.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gpormfvrv.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gnstzqzfp.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gzkgfekki.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/glqaaxrho.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/ggwhjxihc.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/glbbocaxg.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gsmoiuayr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gmudufeju.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gsksazkoj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gttdfrxnq.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gfjhqhgrc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gyewfwsuo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gfeleszpn.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gwcpjxcmh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/guniwzxxj.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gfdiudrzv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/grrklkxkk.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gjzeiscnx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gadjdiqus.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gwvdaupsk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gndrxudan.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/ggnqmjtga.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gncqnfppp.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/glrimoajp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gxglmkhcr.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gjzqfiacf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxqnemjat.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/ganhcoidp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gavkidpdg.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gapwgkfom.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gavlafcrl.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gmxuptxud.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gfcmmwurr.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/glyihrcuv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gxtmdezun.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/ggmizinmo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gtyzftscx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gomlnhpwq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gadifvkzk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcdctvcfy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gqciiywmy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gjaszpehb.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gelrzrbug.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gemvzpeva.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcsrnsgvc.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/guvgvrnvf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghaxvqagb.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gohpbbxoh.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gvbcwxmxr.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gmcikvhmt.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gxkoiiemu.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gccumjnti.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/glpadxeag.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gcatsbrde.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gccxpexez.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/ghfmirmoc.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/guuzwvvdl.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gmzrfodkx.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gdlaapthv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gfxdwnlvh.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gcwzxlwre.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gvxmwpnpr.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gpqrpcawo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gkvshzuhq.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/ghipibvzr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gpyfotkiy.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gtaiixqbt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gfigcihal.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gojhldlzo.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gwtynqwye.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gvojsqodn.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gnajnoequ.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/ggwolhdiu.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gqwusepgd.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gvgopqife.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gsrjoujag.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gcibmbvzp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gtbtfknmw.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gxtajbikl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gqodcxzmu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gsvhemmtb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/glbpamkor.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gapiklpsl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gsfiwlkqv.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gbhmsptjw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/ggshcsyuo.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gobfxhkbs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gzzkogaqy.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gnkwodeib.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gusbmkcmc.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gkuzkzakt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gtowzdrdy.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gtjaidsdp.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gkjjtnjcs.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gpxukeifi.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gqsvnfxou.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/grpferxck.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/glvysllvb.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gzdhekqyp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/ghldwegjn.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/ggrpczfcf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gzwywlyxg.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gcboyqbic.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gwgqgzzce.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gyqqcazzp.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gqmqufrer.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/geokzrvwh.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gsuqoddjh.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/ggqenbupb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gctbszzme.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gjvsfffcm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gnpbiyjys.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gzuhborjg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwzkacwpu.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gkvcgzyeq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqakupqg.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/ggkevidkc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gqagitxlr.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gmgwavpbb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/grunwzocq.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/garciwahq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gcswxupfy.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gwkktbvwb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gclgycwln.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gqkudnguf.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gwmzbukfj.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gwydpqoxl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/ghlstlijr.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gauofdbpj.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gldgsfmpl.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gakgolmoc.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gitfyzkvo.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gfyqisbss.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gyflilbsm.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gacgopmny.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gejrfntow.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcwtfjqaf.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gucmxfjnb.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/giqebmhbe.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/ginhvlzvx.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gbdnklxuw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gasuxoqzh.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gzxfhtrgw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gatbsnwsa.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/ghcbgqfwk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gbudypiql.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gszexygwq.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gswygrxoz.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gxecjpkbs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gzacujaqq.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gircpgakp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/grtynstoc.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/ghlnzseft.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gtwjvakil.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gfhhaywqp.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghflykwhf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gadvmccli.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gdgmtzbqw.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gocpfvjju.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsxjpvbdx.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gvqcohcdk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/ghuxkdtzt.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gtrknrqwh.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gcvcunhqs.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gbarafpei.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/girqtxeqe.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gyantieng.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gdzkxgigy.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/geecabnui.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/glvdlgnpb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/grezkxmon.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gkllwknfz.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gloiyjqyu.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gdnxpvcgn.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gmvxackbr.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gqtkyuuxb.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/grhucoguv.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gqcfvtsdn.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/ghltemqfj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/guemxmlek.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/ghnoghrly.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gcjdyedhy.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gidrprtmz.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gwsqouxim.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gcrftfxfc.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/glfizhxvm.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gcptugybs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gnoxaclvy.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gisxsfyil.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gozgqjhzy.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gysxdkops.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gewcmflwu.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/glfebagyk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/ghlqiryqw.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gdhlhqeqy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gyklzujtb.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gucrkvzqr.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gsdbmddlt.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/geedguivb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gijtsyrhn.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gqddpenyp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gqfyhldrn.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gkowpiksi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gzcbafqlh.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gyjjqogui.sHtML


<!-- 参考信息 -->