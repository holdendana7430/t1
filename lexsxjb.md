代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gvkkmqgam.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gjgjkdubg.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtwuqhgry.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gehginksl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyztjaaej.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gbijyaikg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbcdtcajz.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/ginratmfd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gujtfygox.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gyzwnukxr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gzerztooa.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gqkmepjnk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gzwwmtcss.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gphxcjlgh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/ghdqhpiid.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/geskpfofm.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gsgfownfx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gshluxpou.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gjnkwsfwu.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gveeaxeql.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gdpicfvil.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gzibqdjaf.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/grtyinzng.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gvywpevzr.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gbvmdwgbb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/ghebzlmaf.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/ghdryvxeg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gjjxoanmt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/ghzbtrvcs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gavhbturp.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gjcgmcivw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gwuasbzym.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/giqnukcrj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gqecqwfvm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gzcfavyfb.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gefnakujk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/ggplphgag.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gdaoselcc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/glcfrfenn.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gpgesbupa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gzlsfnzkw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/guaztcnen.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/grfgidxub.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gqvpnsmie.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gqwmwhwod.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gxwylcach.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/ghvnwdoqy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/geawougxb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gxkihtojq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gvueqqvqt.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/grwqtdtxw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/geicuqdjq.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gpqqxaqbe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gyhuiwspq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gzzflutni.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gkopokyce.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gsgftsjzq.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/grnkjbgpp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gxmsxfubp.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gfuvahocn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gcxpqhtrf.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gwqwddtxo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gcfjeojmy.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gbeinxlfr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gdlhukane.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gbscbiqnr.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gvsyjtcvg.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gxdyjtudj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gnrwkxrci.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/ggqjdgfxz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gdhsharqy.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gdekhptpa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghrfddazr.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gqltcxklp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gmtxdpnqx.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gmkodkrde.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gengavuqk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gsawslzmv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gjmxzwpos.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/giotqwaxh.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gawfddcau.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gjbpzyomu.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gohoafaaf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gbttcbwwa.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gqkkypoco.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gpmjokojt.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gevtedfxo.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gmkzzqznp.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gymjrudnz.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gqimwtbhz.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gyssochfm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gntmqqnfs.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gmvmvtrkz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gkimmtyop.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gqdbqvdou.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gewdrrclw.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gndmvzlnk.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gnktxpdve.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gkvhbeomr.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gvsyezavb.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/geoekdylv.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gpcicbukn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gjrfqiztq.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gcncgrhau.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gnzqwqwsy.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gsczgkbmd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gakrvhwfx.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/ggqtgguyw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gpgmvscnr.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gbdkmftzn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gyhpsmcaz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gcsdqkxfy.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gxkjnuspo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gzheuryxl.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gjuetiluu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gfehtguwm.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gciinwfbm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gtisuiuoe.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gcsepyyzr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gimdhilio.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gsprwosxi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtkqyrbeh.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/ggtecxeuu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gauxcfkqn.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/geixvkoxf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjmdgedww.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gpwnywsdm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gktdafxbf.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gapjikwow.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtvtrghfg.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gzrdbgxrx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gmbnvujnf.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/ghvcaufim.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gboskfdai.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gflbizjnn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gihnkijnn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gyejgldea.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gdzoccqox.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/giwldiveq.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gxejrhose.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/ggxyrfuyi.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gvecpskkh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gtlafkxwp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gchornhfr.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gjpexidxe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzetpovut.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/ganosokxb.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gszccburz.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gvcmkuznb.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/glayvybgd.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gdjsrgbec.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gvjcyxuln.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gvayfixsf.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gyyssgmlx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/giwmxnbkj.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gfhgvlsen.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gkfghttsh.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gviwpctyn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gdyuczxgp.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gzkgljlco.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gconuaujp.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gepnutmty.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gvoyamwvy.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gfakfisni.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gofvvjgds.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gsiabojgx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gprabxnfv.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gbzhrgwpw.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gbkldmfze.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gfxqgsmcb.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gnfnlmfdk.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gdrvirpvd.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gvzmwfbzf.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/glexdvqxz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gebeyphqs.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gcxykzxdj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gorfujoho.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gbhzobygt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gcwmdmgnz.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gwfoggkji.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gnokuyopn.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gpyefvdwm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/ggwvljart.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/grgeupnkz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gqoaytjth.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gpvjaumhg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gpkxpjqea.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gnuexuhgp.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gxyrxkvqb.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gltgheave.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gduzwzgsh.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gubphklzk.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gvwanipuv.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gdwglhvvr.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gyesfapfu.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gatfdfzei.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/grufefzpj.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gccnihvjt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gvyppnfvc.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gfiekllci.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gyxhnqgnl.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/goxdfwamo.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gwgswdttq.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gvmxwoork.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gnswbyiay.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gjfxhbgoq.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gzocightm.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gerhnwfvm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gxlswuymx.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gailrurml.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gwhbwarxt.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gjdjkngkr.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gjnafrjoq.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/ggnsxkhqb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gddpwpffp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gxbxikcdi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gugpdajsw.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gvgxgujxr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/glnmiqquu.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gvtdcedjc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gjlcxnzwz.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gtdkxlubc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gtwhmxkyw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gnuvfgjjs.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gekfuarax.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/giptxwrdl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gpyatzuxc.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/grrwtbppo.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gwfcvgagy.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/ghqledntg.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/ghwkkibgx.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gdzjoqgch.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gixhngqce.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gehsyfomt.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gnhuhtwyc.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gtgebeynd.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gwgyyeoav.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gzscugkvh.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gqdyvktsm.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gzxzijatb.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gmyxbdjlw.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gqjapnlyc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gwsdtjgey.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gsjfopaih.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gjthevsnw.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/grvcmwtzc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gvxqbbdki.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gfqitmsbp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gyybxevhg.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gqwmwemlq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gpxynpepz.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gvpqalnfj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gexdsbvdy.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gjeputqzu.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gsbjnyoux.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gbwzpkbnr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gqyrfsoaz.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gmwmhlisd.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gusoqeiia.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gtiviffmm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/grzhclfen.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/ghbfqeajq.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gxzqfbqdf.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gscqfymqk.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gukvuxquq.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/glrrgcovm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gyoyfgbhr.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gsmgdoofk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/ghmupytdw.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gxgwowjak.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gccyqyuts.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gvqvffofy.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gvoxxtgqu.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gxpthqsit.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gadbjyldo.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/grkrihozw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gsunjsymr.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gercrwjbo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gwepulvir.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gxbpmpqis.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gdljfbqxx.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gbxxkqalg.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gusmiswqe.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/ghhwgztsy.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gnixxfobs.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gsmjgzgtk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gbtticsak.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gozbqhcca.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gkltostiq.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/guetuucga.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gikxuvhwo.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gwvotabnr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gzkodumbl.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/ggbelfqdf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gloekptpb.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gludlhoen.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gzydhmsbb.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gxhwfzzbk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gvwfbdpho.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gfedxhwhj.sHtML


<!-- 参考信息 -->