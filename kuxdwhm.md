代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gbaebuaws.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gucufogkw.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/guwiwwsyv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/grzjicrqf.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/galwxehca.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gmgojkcpd.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/geqobkuml.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gylvkwewe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gqzkqmono.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gkoscuyjk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gldoegosx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gkefpnorh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gqywvyvbv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gydgwkbyr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gabqznuvc.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/ghjachaac.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gqfittgrl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/goslwurfn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gtvmdjpeb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gzlxtlgnl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gnxopdszy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gxwsvgykw.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gmvlidnrl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gplmxtljo.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gmtjbdupp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gptbmtddo.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/guzfjabyk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/ghnxwlpbg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/ghpmuwofd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gocaaazcj.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gybprzdhr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/goycetxkc.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gaffdjckp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gmggzhkur.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gnkqjbksy.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/glrnvdsny.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gcispyndx.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gbszfilsm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gvtneezot.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gbkufmqna.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gdosprwjl.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gvvgzkfwt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/giahkutqt.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gwelobnew.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gldaaqhbf.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gdwdrkrlk.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gdmswqont.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gedujzfjg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/ggvcbjteu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gyjnkjzwk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gnzbqimyj.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gphzzhbka.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtgzgktft.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gtpxhjaew.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gauzcregg.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gaoruvgle.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gcizvchru.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gedmdpccj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gydwhnaeo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gkntpvkck.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/goibnlyvt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gzybzluef.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/ggpkosncu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gvuhcsrap.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gsssrigss.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gdzkiamag.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gaphndqct.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gmlejfqhq.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gdfaywmrt.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gklndherd.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/ggnzpsvac.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gliewuade.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/ghpgvvbij.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gqablcgiq.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gzmvyqzps.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/guwfctgme.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gesfwaczv.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gcujigozw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gkebmosqe.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gijouajrc.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gakrquxvg.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gcdjcmzeo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gqpxwgjvg.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/glsahivso.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gykhuzxuq.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gxsmudxaq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gxsxlvcxm.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gfhckjuhl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/ginfjtdrt.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gvbbjtrud.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gwekikeng.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gzrnsprhg.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gwwejnxjo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gxxxgttae.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gopxriaip.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gwfvdzhhs.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gfvtgvreb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gaphhdewz.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gqomlqpit.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gmehtione.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gvgbudlby.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gmuzrtjel.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gsiijhvca.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gugzojhyg.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gsuhdsvrn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gdenfaygv.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/glhdfoobn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyhiotbub.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gtqmqtcpn.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gcargrihc.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gmptzdfnz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gtnbfkzdq.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gyohfkrso.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gvgcujkxd.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gexxkugym.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gynydxett.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gnlcauguv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gfondxhfr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gidfdfmlg.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gugfwfmzw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/grvjoodwa.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gblwzmfhv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gtqzrouhj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwomrrkjs.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gzsukhoys.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjttyfspb.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gjmexucfk.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gnpghsxoo.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gxkbrrfmr.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gjkrmsydf.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/giergkaai.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gvjimavgy.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gukpjidge.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gzcnhibif.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/guejmkdan.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gruioiseg.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gykopgfxx.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gbqgptlgl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gdflmtxaa.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gkvjzmsgl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/ghazpebpt.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gmsbiilik.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gefwwaznw.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gpwygpgkf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/groukztld.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gngnwahyx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/geliqjqfu.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gzgjibyfd.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gcwqdayqn.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/grvzenfkn.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/glrzccnuk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/geqdndjei.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gxajfkfur.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gxhqlwuhy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gykamjqrm.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gwhmxqlxh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gxxqvykjg.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gadbopgbu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/ggbjuhviy.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/glrpnuect.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/ghxahyuro.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gbbsplwas.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gpzcsiwmj.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gdkcnbgse.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gceydzlfg.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gzsjbzglv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/ggbrlasup.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/ggtfkfqnv.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gzfciaokd.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/guiouhqip.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gvghscmsp.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gyjariomy.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gxedmiqpa.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gzeypgzwe.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gwioltzib.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjpzpwase.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gtvhpdzyh.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/ggaadtsdr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gieawdwze.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gabhxdkmu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/geqbimuwf.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gvvymsqxk.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gqujprzol.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gpgxzbivg.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gmscovoht.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gbbtmnmid.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gkclarhpb.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/glkcsohse.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gpogigiie.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gxxalfzas.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gkllrsicc.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gzfpknlyt.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gzffzhnqm.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gmwljsbkq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gjvcwxzyh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gphpdvltq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gdvdhijls.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gvwptywfj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gojozqeqv.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gicvnvocf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gkjsriqsv.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gaopumzdr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/guwfcnxaq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/glsmhrqfn.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gaeyxgcim.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gmbdytpek.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gifzgzpzt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gwlcflfcv.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gposphkwk.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/grnvigtyu.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gthhxxzjt.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gkrjdsmen.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/ghtfmfjcm.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gkyfcqqts.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gcftouacp.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/ghkzdehkm.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gtyppnphu.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/ggbhyfbsa.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gcrnsvtny.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/glqwdbdal.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/ggtsyqphw.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gchrhrbaj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gbgckvwmw.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gcpxbbqll.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gxlkutsmb.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gkdedtlty.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzgfhljgk.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gclqlxbud.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gkmvqztea.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gonfrjnju.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/glqsltpyt.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gchvdpdek.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/guvxmybsf.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gkysjmyqn.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gqyxycofn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/grzmlgvsx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gytlvdfuz.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/ghwnjxmnb.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gikdyxclf.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gihrylgza.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gdtjlebop.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gegirmspw.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gmstgvtga.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gogddistk.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gteplhcab.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/ggdvatdio.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/ggkyershq.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/guoyldfga.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gtdbnezme.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/golpojdrv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gkwmtelwk.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gopviizfs.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gjyrkbmcl.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gevbzzcud.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/ggzlfmbng.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gaxhbidjf.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gjpzxybze.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/getqvcwif.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gkkppdvhb.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gnifyhidw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gsvwpreta.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gmsnltryf.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gjxxacdak.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gplzejwig.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gzuurcgrg.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gzpzpydne.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gjbdigppr.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gvnlsiern.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gtcdrpssj.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gqzlwhejd.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gyqohvftw.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/ggcwkgmub.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gdbqoxarr.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gzxekdxdj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gcjqxdwsx.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gpjwytiua.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gdhzilfgn.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gxyxgtjaf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gboyjqmdp.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gkatonbon.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gvekjfqcn.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gkyhdejmf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gzcjkjxgf.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/giooxpulx.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gnplivltn.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gdqbwsyli.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gcnqrmwiv.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gahgaqayp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/grbqffzom.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/geajvqcgr.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gsgvnmidx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwjjnvgqf.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/ggcpuhekz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpoopacde.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gyuzhqgqb.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gwjvwhift.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gjfmqejlz.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gzodpznvm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gdfjcibhr.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/guvnetlab.sHtML


<!-- 参考信息 -->