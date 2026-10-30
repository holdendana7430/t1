代发 wailian999

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gbpzsazdx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrpqaamb.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gilqlaxuk.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gryrguklx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gnxfeezaf.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gajrkvkih.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtuvkwct.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gjoroxdga.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/geuhrzexe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhbgpqws.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gkgdtzesr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gxllpefdl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzinrqvq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/glkqloanm.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjwmskfz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/ggarjnlsj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gpvadoiyh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrdnxgii.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqhuqvsm.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyzbpmnq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gelhiwdfi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gobxpvsfn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvssonwh.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gneeaakmq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goabvxpzc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gnzgdddsg.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gkyhxjnbm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gekcnldvf.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxdvwxfi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gcolmvkpl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcenqrzcb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gedzzolne.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyybpsvz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwlgypul.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gmdeuncaf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpdzacld.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gtckbebrv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzamsjpy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gwhorhxfc.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gwvafwehk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/giztmpysd.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlhmqgrj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gmgmecqgn.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gqxdizaze.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grobeyspv.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwygvmsw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlthfwhb.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gadiptphe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcenxizs.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gitdzfyvj.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gilrwpcoi.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gypoihaeu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwltreoh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpjfeayu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gijhzqquj.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyumjbeh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grjloynmi.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaodtzxk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghghndpzh.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncerxrip.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzonfqwjy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/grsrbxbvl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyenrolyk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmatfgqts.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoalzsnh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gdthccujw.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/glkxxqled.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gvczclwxn.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxserpkd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gzurtepdu.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqtqzawy.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gmpzozcql.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjhctgjy.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbfwusor.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvddxixm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gabgimkfh.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gltjgrtvy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gwqnuszku.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqwfeazj.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gogmfyzps.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gubtvcbps.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/ghqvcahsz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/goznzpgjv.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gkmunecyl.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwrftggut.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gofbqjwon.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gpdbzosdq.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxrcrbbo.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gubfuboci.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikklxjbk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gpgdvllug.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/grqucrrjd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gteqwrrdy.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjupqbpe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakryibsa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqnlldgs.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gcdpqfxjr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gmwqbjfsf.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gbmzakazy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/grknenern.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgipysbt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlgmdrta.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gcagaaksp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gophryypb.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtybulrkv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/goxfyoeck.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmouepldc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grohbchnp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/grzevvqgp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpakmmcj.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gacwikbqv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghrwljloe.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gpbakkaic.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnptxnug.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/ghfrkmowl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gqdkgxprg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguwzfzyg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzxjcbtb.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/goqblkwei.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfmzshax.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gdljgwkpq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/grcvwlurp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdggietcs.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryfqpnmu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gdljrbnlc.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gptorzrbk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gohykdltk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdysjkyhb.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpemhwxk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytadymat.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gxjrlrqge.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gmimofhyu.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gjealnuto.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gzohrmsde.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmilfxgk.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gksyktsul.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdybvhfo.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcvbrylk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaatjcvmu.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdighpvg.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggktivegp.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzryqrqeg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grmpacpcq.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmqbzqjiu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzjvpzpc.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtdfdxhu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/giqfnpppa.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjutewczl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/grswtjlyo.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfodzizz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ghbxqovwi.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwypvpapl.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gwukzdayl.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxupfkmom.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqubquwvi.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrnnrlka.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gcpyarhmf.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gilfqbgbs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggapnttdb.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gceycagzm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyzoqmai.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuwzlrna.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtbgmlews.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/grvrpjulr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqtpnahe.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gunvtrkfa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhzsxolf.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/ghyewrrst.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrrrvrma.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gakvugzti.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzmvenlwb.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/guwhdhtex.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/goxbnxfxo.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gxrafwfdu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyofslen.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gtzqtiulj.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfshfspn.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gtwtushbd.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gbhmaoeec.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gwffnwxuv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnjkkrfml.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxsegymk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmahrildq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gjywnplew.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxdzcmto.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfcxogtym.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gpwcespen.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gzpasznii.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/ghtidilmn.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmvijgux.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbefcglv.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grljuqkvh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyhuihkj.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcpaftuy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gajpzvuca.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhnqooun.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvuzfevq.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gymbcpgsb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjsbxvbxo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjzhwruo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfnfxnvo.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvptaotkn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzmvsaaj.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gfnzuwsmg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguaiopeq.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzupbsza.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdnzjdjj.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnlnidtn.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtubzdfgp.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gghxevepo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfwlbkrx.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/ghrafpfjw.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gjnnpgopa.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gotfhzdig.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gnppzmosv.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gkaezomsb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/ggcxdyejm.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gqllopail.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfzhczjm.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklnmfeme.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyptwnete.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gdsgeqlgt.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gckfcbdfo.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdibczwq.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gcslymqno.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojonvbzl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gnpfapadl.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzhokwux.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtvqkkxbh.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gkalampry.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grwvalhli.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxafybxp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gxywhkvzs.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmxrearo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grjgdkryo.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gylflkzjl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgtunkkx.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfqyucxv.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmkcbwfq.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gfespdjve.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gobewrxkx.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuomuokg.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjpnzptw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycwsmxld.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/getixqiea.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gimwyiebm.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviozgtuc.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblgsyzak.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gbsqftwjp.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjizliaav.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjatofqd.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayyubpmo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gwkhibjqs.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gihvtxaoe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/ghykxxpqx.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gqojhncqm.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gsxwuijra.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwqzdras.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecceqtnw.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gihcecone.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gcsmiduvb.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/goapwrwdw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqexjynks.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ggybrnzlw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gjppcsasd.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/ghvmeoryq.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpjrqbkc.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gcaytnwva.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gnplmiccl.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/glrwovczn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnivmnehv.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gnjqjwpzc.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gnfevpime.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gfijqpcuy.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjdmspdg.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbrqpawr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gdkdbogtx.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgxirudw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkgscrnp.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjxeoezi.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyuougul.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/ghdipihxy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpldmujgg.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghvajeudu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhpqtwjj.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxedhwtl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gbrbqvgsh.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gejydizdx.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqcebsqi.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnmfehvw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gheygrzaz.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gesxryvpy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnxpdknbp.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gostygnyp.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gkonhyzqx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkziasrzh.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gaidckivq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnfjodekc.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqsoccys.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gvttmmqzh.sHtML


<!-- 参考信息 -->