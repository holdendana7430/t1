代发 wailian999

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gspnjuuic.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwhbjjcl.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubonuvoh.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnlvvksz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gidvdxidg.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gixxcekzs.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gcimltaxg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/ghhlhprsm.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gypjvfpic.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjwquvcw.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gopoxuwhq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gakxevqtm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gitfhxpzo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqlmmdgp.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gvxjbbywo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjnxnsei.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbizuria.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/geplqyovm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gchrezhui.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfizrhxa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gremjvshu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdgkhyry.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gmbfzqpff.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gddcputsr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gamvnqqhx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gcursvchw.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gwqmuwyrd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkfsccal.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gisbibtat.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/ggqkvysih.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/grlipzxpy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphhaxqlf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdteylinz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gcglcoblz.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gttrqqqmp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtffcdmzm.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gheodhpev.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsaxdsjo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqjpqtmp.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/ggodozsik.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxmspbpv.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/giwlsnfyy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gbotlxume.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgyeuxxg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeeoovgo.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmntkgzs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdfhzyye.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwpugdlt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvxflcvt.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbdwysae.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gmvvvzdpy.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnplbgya.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/getghpdfp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/guwwmxkta.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gnqgfsauz.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/ggtbjyanu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmkpwskg.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gzdlpohkj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjkhrzly.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/ggrwhzuhq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdxeqdhp.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmltvvqi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gusayqjjr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxteeigv.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gjshcwaru.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gksafecve.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gpaxshoyu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokeecqro.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gpnfzgism.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gprxmyaai.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gosabphyn.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gcjgrcxwi.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gparjupqt.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujoyacrd.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvhtvwbv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gxjmknrph.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gnntcxapp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gxphvdnkb.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmujklrw.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gasryjstz.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvgzuian.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmlnsirz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/ggnqvkgiv.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gncvwcouv.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjcxpgwz.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvoooeyu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gnbgvdftl.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gbebdjxhm.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwfcetpe.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdmtpaig.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaylyjms.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gmlfyybbk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gqhpgmvgp.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjypqfoe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gxkuivdec.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gxogzurww.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gturqivda.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfbnxskg.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyhbymbk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gvicsbjrc.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzurxxyyk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnomjjquz.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gymwzhvdr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gbydmqime.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gahjuifdq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzowbqtmn.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gijuvriat.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxlrwabjn.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlesoljh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjwdginte.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gewfrrafi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gypbnnyih.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaupzngu.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqdgqazx.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmiaqbdu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimppekqb.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gpikdeyex.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gtferzpgz.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcbqvjrn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gakjknxvj.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/guudadkkx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxzzivuh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgbkjjra.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrewdhkz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbsqonhs.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/giojcmthw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gzxlwccis.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkbnsssia.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gvwgjpteu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gswwtvyfo.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqjrazgz.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gczkfojuh.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/garsefhos.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/ghundreom.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/goijmqihu.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxgaviwkh.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuvmtynk.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/geepkzzkv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gutqyyost.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzogosnt.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/goynvhzvy.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepqpkkfm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfxzcburf.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gryzhlybd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyutgwijy.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gclzyyipe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwetnkuxm.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gipqdihdx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/guhskhyhv.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxxpvuap.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/grpbsmuxk.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/garcrbyvh.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgzaqeyh.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gxpgioojf.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghemlbabt.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gktmtgtin.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqntjeyt.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gepgoizab.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyilgmqze.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gkxufhvue.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsbxfzjwq.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkdqxkmq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghzqjxpfm.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/glawpvguj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpwfhlji.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giugzyjbe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtbhmandk.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gnumkijrt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdynjhmr.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgkwduok.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxapafffj.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gdiorlibs.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gifpwmwis.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqpgfgih.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grnwsgzpp.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlzmtush.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/goeajbfsj.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gtstnmsdj.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsxvofaxq.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grjsnwudb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/glnquwxdl.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdaefvim.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkfdiufsi.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gqilxtzsl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrxuvscy.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxcfwuvgg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkijhokgf.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjupcstl.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqrcbhzp.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpmfjozf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gieofoezz.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbpagxaf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gnhszfbhw.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gaiovpidx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjwunwgg.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gasnyfann.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gddtnqqiy.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gajblpcvq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/grzvgmyus.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gulyqmvhd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gazqsghew.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gnyjeuunc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/goxhhekrr.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gkbnynucp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoecofmp.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gwjjqsose.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpzxkcch.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkhhmhdwr.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gaxdujgsf.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/ggfzdciad.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdxvqmas.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gtnjbctqf.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gofvihzib.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfqcmxch.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gryhiphnz.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/guzvaupnh.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwopwppdm.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gjsbtfjog.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gesknnwkl.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gariaixei.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcmbqsyl.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gjscjukba.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gotpefgyw.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gsukryagm.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzijqkji.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gkgpbwxuv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbgiymgn.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/glbbcspfj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwvdsiols.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gcluionbs.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpljnciz.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjjjqovx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gfckniqvs.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/ggbshxqhi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grtqtvcyn.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqexicki.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/guhngweds.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzroknyad.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvzkdflq.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/geedkkcjk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gipwueyxg.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gscncfphz.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiqwwoem.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gsigdxqww.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemrdbewf.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuilimbm.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwqyswmw.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjqamzta.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gukrsiijt.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaucsjkaa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/ggstuvcgi.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gylrrottp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrksxuqa.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gjybpejdq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gsqihxjsx.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gluhwloji.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gimmqlabz.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/garnbxrsz.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gdwrnftbe.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gdopungml.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gexjqlmyt.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgnerooi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gulewvcny.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/goucfrkzc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkyrdaei.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvrejssc.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gbvjffbpo.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giprciekh.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrsaqrdw.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeqhewmu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwnqyfgf.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaxgmber.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgrxllig.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzypsnlq.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbuxrmil.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gqufstfvn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmuzpava.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyimfwdeu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/girmnknnp.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcntrsbj.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gshxbuoig.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/genxpdpeg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpjousjb.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkpcssrhj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gxqnbgsri.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvngvrdup.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gedwwtjjt.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gljneuzgf.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkonryfk.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvcbaemj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gowvmdhkc.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflkecywy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspuxhbfr.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gzwzbxwnk.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqawmwhz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhwjxpof.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbiqjtjt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghnssvzbg.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsjrgwhr.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gqupdegqo.sHtML


<!-- 参考信息 -->