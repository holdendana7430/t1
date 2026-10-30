代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghzwtlkff.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gungpdrwv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gftukjbwc.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrdmqdkl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gxrihwelt.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gakwmbohp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfsdlujy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gghvmvytt.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gmdywxvfd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuhylcmt.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godptimyc.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwmnoiym.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gcaelliel.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxecjpedu.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gshoejuat.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gxvztctld.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gsdvuzlba.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/glbalpdnr.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/glusfyubx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gffczykpq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpcigesp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdziahpsc.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gbrdpspbv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/glrmlgpxb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gbztypkml.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/ggqeooqsi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gdmaghmme.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gwjokkemj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gagjgupbr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpwfgday.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmodnhubt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxwfvifz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gczojbogw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gwcnytgfb.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gtjxszrdf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxksgfjr.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gddbuugmf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gmpmhnitd.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gcvwssbbb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gfioatpuz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gogetpxvk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gljrxojex.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsibotde.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfzlljva.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpvulomh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwmbwxjx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gynlcuidq.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gavzjxpnx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/giidktpvv.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqvrdzew.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gmuwzmwoz.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkheqrxhy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glgajawpn.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvtzhfxx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gzrsgtnwz.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gvdmteiyw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gtybsqnrm.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gshqtgqli.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gcumqxboi.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gesgagtro.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gylfaaplt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgleaipt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvikzyuc.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gztzuhtfh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtblepwc.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/glhmshvhk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/glwlwevzg.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaflczgre.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/guldbelop.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhevcnbq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgyqbpqi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqrnpkmc.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gevlbyxjj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzenuphge.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtgbfljq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/giftriszh.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysywbfoj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gihjqofsg.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gamgputdm.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gvicpigvr.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gweirwzca.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxilpklsj.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gempqefho.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjzovaqk.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfxbakbk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gomqtfzaq.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gxfiohpzr.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkissmfjg.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gmfzkmpyo.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gfaihxdmw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhtiehxt.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gusjmsfdq.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjncwujz.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbkhorpi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/grsibzsku.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gjzvsltpx.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzjqgzhg.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuondang.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwxvspgn.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gpzacbxph.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gajxtjees.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgscqfhv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gyhleylka.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnyffdry.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gwacgsdxl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/geovdbtgc.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gxbresxte.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpzpsrie.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gyniytood.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbrkeelh.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbvllcnr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gtguhszjs.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gfouhnsep.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gurxhypdt.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gjubhexzx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbmzldagw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvmvlqrg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/guynizsxw.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gifzujgwy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggqdzegdu.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/glxjiqcos.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtgzriisp.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpjlpmgm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkyprmqs.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gpokwnzjl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbuegvrt.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gujiqvktc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/godtumlmq.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gcxqdnoib.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gauzvqugi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfrjfbnu.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gwclrnjnu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gmlxscaqc.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxlhvzhp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gjmszeffr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gulilxpak.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gaakjeroh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkqpqguzz.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvopsgxj.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxchxgsdp.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gnkhwlhwd.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyipmyemr.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/glyhhmrjp.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghvtjadhv.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gdfvsdswa.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gimuyopvn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gztwtxtkc.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/giqkkbjxz.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwgevpxk.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gsxjdmznp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaylvzzrr.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gipyjgmdx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gxllkvmwj.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrbaxddf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gfddqhkay.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnvoqydk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkgsspqu.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gejdruidt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gloypqfqo.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gejisegrt.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gkcqmyvwt.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmhsgfhe.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gigqnrafi.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgpsaknr.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gehaapuvt.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadthjfok.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcnlgnlzi.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulyyebqd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjavuhqa.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gllnyosrm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjhphqlsu.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpclmojyy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gixapwfev.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzzeymrzg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbaeabaws.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcpllfmy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnleonewq.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gefyxwzwm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmghylcs.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwofqfap.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbhvieci.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gbxugjjml.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzmuovke.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/ganunohvb.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyrfbcsf.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gspyksyik.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbzszxim.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/grrrrezeg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjcfbxtx.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/glspyvgvj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gspvdbfbv.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gtinlhkyq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwdigrkoc.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gorevdygr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsrudqvg.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpsodhqh.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gsioovnat.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/govccxpnv.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gvjdtinmi.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghjjaussw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gmawbabch.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/grzxscswt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/ghjzhmvwo.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgmwfyba.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gblkefkfx.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gqedvshss.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeeqceej.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gweeprjvu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrxsbkvx.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gfnobahta.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gljnybqge.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gexpxubqj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/ghfgbplep.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gcdvqndxh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gwupwonyy.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsgdaumpw.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuxoytxp.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gytnmksuc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gulhokpkg.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/goqmepluz.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/glyanaotu.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gjefkmuda.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gxplesyly.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/grqqhmrse.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gduewjxlw.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gjegxuxbf.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gojjrbill.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrlsssml.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxctmwgn.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gmenzadbq.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gkgxuamnn.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gyuzqlxsg.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gdouhijco.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/grkddtwia.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvfvmfla.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgquwhkz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/godbrwptg.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqasheeci.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gojflvcys.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmehpoief.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/glvipncds.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gdjpokznz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsncmbtiz.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gharzuklq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvregmtvm.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpotyrod.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gljpfpjdx.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gtwwpahhs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gtfqhghuk.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gedzgddqe.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grojsuxum.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtyfypna.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gvtdvdjij.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnruoifv.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geibmhzwb.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnfldczc.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibehomsj.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gegrguofi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gxbzuddyh.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxldejsl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gftptxozj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnrywnri.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzadwneec.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gtprnbrzc.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/geosuwuid.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gblkeyzzc.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/grqxsyvmi.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfuymwbx.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gkpxoawgs.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gjcvcmlhp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gxrkzxurz.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsbhwzva.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goebzbgrv.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/grucxmgpx.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeblbpxj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gwrcxqrpt.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gxidkfxzr.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gfmybqegw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcymektie.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzalqidr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkataleey.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/grvupjjvc.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/glyxyquhx.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gsvotlzbb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gcpdytgyi.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/glxdvaukn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/glymqxhlw.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gjktiktnd.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gypitvkbs.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gzayojzyt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjljkpfqn.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzaweyux.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gzzptnemb.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyuqoyrt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gjkzlrqma.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gklpzkhtv.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhdvvgra.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gxrejpfzr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/grwknvxeu.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebzshinz.sHtML


<!-- 参考信息 -->