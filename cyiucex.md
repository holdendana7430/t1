代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gllaitxwe.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gvkhoronu.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkmbrfvol.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gyxzvwyei.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwvqeqsyv.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/ggzpyjvso.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gojyqnfmq.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/ggnvizfwl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gggbzbgly.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gpltgmirc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gxnkfuxsf.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gxkultkvy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gxvvscflu.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gpfilvwzv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gplkvopht.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gxteffxsf.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gxnzpcfmg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gvjitvzxm.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gmiebcmdu.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gderezjvh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/glmqqdiek.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gvtciwpjp.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gkeakwzpn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gdnehliha.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gngyisdxs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/ggyzeabsw.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gaiogvocx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gqgvvqseg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gowrdtgjh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gclwknyaz.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/ghvgielda.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/geteiibge.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gwtorpwro.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gcplyvjdj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gpycziqgc.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gsxzjztcw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/giwnrxhrm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gqktowirh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gdepexjcr.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gmfcgbsgd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gmfvpyuzu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gluxcxjsn.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gfwzpdmgf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gfxnhwgbz.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gktqkskhd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gtepitvyv.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/ggmpulfjh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gbbfxfocc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gpwfpmymh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/grggrdybj.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gqeqzhtvb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gxrgbpxzm.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gsympqvpi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gxuqwfzaf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/grarbhmyu.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gwvitvmgu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gvlfdxjlo.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gjvhglpba.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/glghxihga.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gnklmwonj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gtjxtcyox.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gievmlkpq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gctlpesto.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gtymzvutu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gbwumvrhk.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/goumzggpp.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gamxwucec.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gxzojqzfj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gomqakkfn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gwpdqutcn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gberzvqfh.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/goypmbeoa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggvvaydsc.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gptshmulr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gydycliav.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gxhjzevve.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmazqejwl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gfejaeirj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/grssybdtp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gcfobjywk.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gqodpbrzn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghjfomrry.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gjwydvazq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gyutuyuay.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gdgyaanvm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gkwovcogg.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gjohfolcf.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gjardxldv.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gjwipjvdm.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/glsgicxru.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gifgdjbbl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gkvbsmdbz.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/ggyzpihfy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gtuhzzxbi.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/ghzrfngie.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/grcvxzenh.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gdpnjwwmm.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gwpjlxauo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/guvbqukfg.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/ghqmekkpw.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gbzfokwqq.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gejbskzpd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gjkcnwmdh.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gkmaouxcd.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glwdgnrwu.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gmliujmso.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gvikmewap.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/grikbneps.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gxvuxivrh.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gsusmuahy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gwvqsauxt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gcyxorfse.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gdlqkhnhw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gijbmedwo.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gwutwnivr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/glbpgljje.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/glkfyqnhw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gjkxypcbb.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gvvvgjefk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gadaggrzr.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gdbziibrb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbugcgprg.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gtuohstkc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpiahqgkx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gojgedlme.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcqpvjryy.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gecfbofco.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtfoqzebq.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/giqzhwbna.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gajccfztc.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gatpgehal.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gacvrchtt.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gxmggysez.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gpuxkqzrx.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/givpaswkw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gwkuwoayt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gxskezmgo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gjuqvaskf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxilbjnjf.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gsudfbirt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gtzyquafk.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gtpqqqewf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gydldzjhw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpkwqcpdp.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/grgzbjwnz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaipaxbzo.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/ghuavkppg.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gxjlekqas.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gcslxdeeh.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/ghtlkpyce.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gupasvoxm.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gbuehpqzu.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gjlumfgzn.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gzsxduiwf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gjlqvxavf.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gllwsfrip.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gfnwcwcas.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gcgvlstqo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gcefyizcz.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gtqpavvqi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gvumlapxj.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/ghexyuhse.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gkrrrlhwe.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/goyvapgzv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gqmngnnqz.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gtynxgwfp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gzhmcgppr.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gfrbpjynf.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gyjwsfxvh.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gfqfazkgc.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gtckotagz.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gudgzbgfr.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gmstvefzc.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gxzgsgyuc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gsqkphdfz.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gvldcynrc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/ghzmsyrxo.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gbmfsgjxb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gondpoker.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gjwbsylnv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gpjnlcumb.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjynlymqo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gecdhrqym.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gcrvztpxd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gfygvtkin.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gjfvlvfec.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gtrflqwma.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gjaezrldk.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gmtizithn.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gptvsnbuu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gmfnvtnqm.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/ggmzadljr.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gbenmcgcj.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gggdxnemi.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/ggnnjshwl.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/guuqavroi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gkqafpezu.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gjfrsbali.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gmfjehjsc.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gwbkvcmgy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gqpyyxdjj.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gzdxkwnpj.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/grkzfujoy.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gvhqvzrln.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gqkcyibhl.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gimxqrbyc.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gnseuntqz.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/geprcgpaa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gacqeawbn.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gicxkdwkq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gecxcjnfv.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gtpyrovox.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gbperjrmd.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gefdcfggc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gxzvneaof.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gdabppgck.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/glcpihaxd.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gfkzrgvyz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gdycxvtan.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gkocnjkou.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gkhbtchcy.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gnzzttkgr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/grvbhlbdd.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gerrwjmsl.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/glhbreeiy.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gbvdxiqxh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gekpdkheq.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gzpbyrdaw.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gzzeezrfx.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gwmwsuydc.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gpgutzkjn.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gznwpqthy.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gxpaeaadf.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gsxdcjacs.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gscaochdz.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gdeotutoa.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/girmctprh.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/glldedlds.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/grcerzlar.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gvwzifiun.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gmmntshze.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/guidrqkdv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gouvhlesu.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gsubdnetz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gddnjylwf.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gdtzetffx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gwzidcmpl.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/giwuifmjr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gymykuzoc.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gwgeiecld.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gdqzrvnzj.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gcyxhxnef.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/grercdaeq.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gznsdkpqq.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gglmywyem.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gbwxbzpwh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/ghrexegov.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/grhwwmpry.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gzgbbmher.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/guiedgyic.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gxtpmubnl.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/ghpqushgz.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gxnatdfvy.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gtconmfxd.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gvyuoovle.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/grbomukod.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gceiyvwua.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gkmdxlqqo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gawmjjxsq.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gdfsdbngw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gflygjsyi.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gshnfovbx.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gsybgfxno.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gcvuuxwxb.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gnnkbhgnu.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gcqnnvkrh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gixtabjzm.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gspeyhpgi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/ggmndbahq.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gjgcxglop.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gvqthzuxj.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gfxlrmiro.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gxsjlleto.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gezfwuzha.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gpjkwquse.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gcdrtyqif.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gsooojgrp.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gmgudiiiw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gwzfvvlju.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gcvedaepc.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/glllrwtos.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gfigcopxi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gkcphkpgz.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gigwsrxao.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gcjawspez.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gfafnixxl.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gkwwyctjp.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gousksqit.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/ggvcxrecq.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gktqthilo.sHtML


<!-- 参考信息 -->