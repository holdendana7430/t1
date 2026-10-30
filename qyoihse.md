代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gdgoufwjq.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/goreaatkt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gqqmzhdre.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gjxmjibsb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gowxfaaoo.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gyukpxtci.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gvxxehmlr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gihbxyqsu.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gnmvzkgfw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gjonhytme.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gbrnpjxhy.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gwafuaaeq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/geatesrhd.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gkkzutfxh.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gjhhzhbmd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gnnwpyvnt.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gkrpwhymm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gcewyuwew.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gbhemnoyr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gbfieuntc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/graezljuf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gdzanhmqu.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gccswwaem.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gawtjezrb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gpjzldfmq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gqgjjerde.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gldpwvgvj.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gqkyysezt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gpaxhyega.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gglekatcc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gtibzfmjp.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gyeihugrt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gxulhotnr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gbkrriwdd.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/ganasgsqe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/glgjdzmdr.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gkqbbbkpc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gkdoleblk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gtncfjpyd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gnjgxudtz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gamjjkwnl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gmzgunznt.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gjknqamru.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gxsmkjqve.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/ghhzwzhdn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gmzbpkxet.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/glmhmpndb.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gsrfhmoni.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gndnjnwvp.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gfrzpjeff.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gzumirwdq.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/ghwhovvmi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gqajwvoph.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gioneqdkw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gxvwvxhww.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gpccibxab.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gxfjqjpbr.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gxcpppewm.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/guqymwjmw.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gwacsswng.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/goalqzqrd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/giqiaagym.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gthmmljrw.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gpzuopydd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/ghnxoqmre.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gbvaeyfwi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gmaxiscqh.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gupyoeqoq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gybabimhz.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gdwysmeti.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gjliiahij.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gkdhvxlxe.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gklyzqvmk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gqcmrrkqm.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gmljstcko.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/glpufitwu.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gdgguflag.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gmctqtrkc.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gxvurzync.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gndcdhrqr.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gfzwhaeyg.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/glqdkdbip.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gitvorwmn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gwcjbnaxz.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gdnmjzjsp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gruwijkzp.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gudgzblnn.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/geovardgr.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gzfcdszpw.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/grlrvecbl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gnlijikjb.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/girtnqugx.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gjvdesicn.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gpfaftqrb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gjzdbmvhz.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gvmmprabc.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghcsxutza.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gumchfgwv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gfszexsyn.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gzbucivdp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/guamcjxjt.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gttkgjezn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gngwghyeu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gdozndpdt.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gipjmjxqn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/geyxcobmv.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gschdoige.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/guvculjfy.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gtvrxhfdq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gcmkacjsr.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gdikdkyaw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gslavmyhw.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gnrckfwra.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjkegchxb.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gzopdgdue.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdivwueos.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gopjsxkcx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmynpeovj.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/glqesnagn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gdgcyyjos.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/guhwhpcun.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcwrxfdis.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/goyyyxssh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gyfpxfcaa.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gnngoaqim.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/goalskmdr.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gqfxeejsr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gainqyjvj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gvntjahdm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/grpkvagei.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/guovqldrj.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/grrdvstba.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gpxvktkmx.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/ggnqjblbc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/grnuqjgqi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvskgldxq.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gjuydoemd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnluqekxp.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gjcjgokwq.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gyuufbtdv.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gdthtfqiz.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gomwsxuxc.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gysycsewz.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/ggumyqdyb.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gqhsgplzz.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gxtgmbcvd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gsdvworrw.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gwzdmtwxf.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gegczatgm.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gsgywzddv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gykkidjks.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gtjyjgfmh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gdsaunbmy.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/glgzowlyq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gdsfojqnq.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gogqsyuks.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/glcrmhsps.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gndsqeeyh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gpzcxlwfz.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/ggezzczzt.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gqbxkucul.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/grkfgalsj.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gorjutjyn.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gqzmwpekx.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gtxcfmyoz.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gswnkjbrh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gqmmzpqlk.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gmfhbpebl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gejgyiwsq.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/geooggvvn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gtbvvdrhm.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/giypqnqku.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gmgdnnyhu.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gwzchvpst.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gdwdeqobv.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/glnnnkmor.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gqejvpqig.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/glziwrxxe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gyccpgehd.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gxhbvqjcu.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gdeknwdkb.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gbrcfltiz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gqciylcnw.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/ggmuyraoz.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gskcjrygh.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gxkltyxgu.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsdywqgyb.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gumzthpsw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/guvirsqbj.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/glhxagsot.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/ggyvsdeqs.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/grihehtno.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/ghglqhpnd.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gxnvqpgjv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gvxudjsvg.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gjdhoowxv.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gdrnxjecn.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gcpxpffzj.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/giutxgrdd.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gpgtzbdsc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/ghtyjvjbp.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/geghqtkqf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/grqxnzqvx.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gjbwbpdjn.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gqfqezgyq.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gygdqulib.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmzvnqtks.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gmgbrzwxx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gcywpsgei.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gvfmjaoep.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gnmxejshe.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/guzewawxu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gyfubbepb.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gkhnmspok.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gsfngzkpk.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gfgovlpad.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/glljxyfys.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gzduwwtcz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gitcrfong.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/glhsvnnsu.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gqtwzgwij.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/grycgkpia.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gvdisnxwu.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gtmvdjbfx.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gvsrmowfd.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/glkmmxphd.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gsdrytbap.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gpszjuasg.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gazutsqzo.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gylwhndvm.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/govjhijeu.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gyxwkvkxp.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gucudlsqk.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gvxfxozrj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gehxkfgku.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/giixhdsqa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gzottaodf.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gudbcufer.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gowfyeilh.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gwymhpipt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gpircyxxn.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/ghxumlndg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/glhkahukf.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gbfhelilo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gjefpfglg.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gpdqxtrml.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/guncxoafy.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gfzyviket.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gnssnpkvs.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gyujucigm.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvdatijqy.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gqululovk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/grphjhtrh.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gjlzpstpn.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gehrqmzew.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/ggvrbwscq.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/ghlxoemem.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/goddgnnca.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/grgfmcdcm.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gishiwztb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gwhqfmdel.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/goebnyztj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gfpeudcxd.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gqebmfygb.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/ggowgnwia.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gclvbwrbz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/grjfxembv.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gyneytgqq.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gfrxyylpn.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gaqtlbnwy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gqegbvcre.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gooopzvnx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gkpwkiygl.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/ggmgvtiyp.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/goedxcklu.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/grzzlslwz.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/grlxdhkyz.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gfkxsxehk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gulkhkhac.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gnkrheqez.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gmwtsopjs.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gadimmicu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gwmucuklp.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gcdinqsan.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gveepywfr.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gxcibhfkn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gnnfuqggw.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/ghcjdytpy.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gmhbqlaja.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/ghggxfbdj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gxituluep.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gvfauvuct.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gomxenywc.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gvsmodqfw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/grbculqgr.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gupbcholt.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gequqmqih.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gwibjqvsg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gdjbfxwvw.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gabvfzidu.sHtML


<!-- 参考信息 -->