代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gfphqvhku.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gpuakisxe.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/ggkywjlnj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gltkqgjdp.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/geapkpitf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gsmuzvazr.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gpemvvnip.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gzwqivdkp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gesavkfny.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gezjuctzm.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gvaqybmmr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gbaubicvg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/genwsgobz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gdiracafq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gheejrphx.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gwoyxnlbi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gzdcxzwex.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gsovijtot.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gzsznhcrx.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gviyvhjwd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gmqlurnpy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gppbvclhu.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gkbbarwcc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/griqlzjvl.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gwmesdogc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gusravbly.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gxghsfust.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gqyusgkvd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gxgesceln.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gvhtwdndv.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gctamfsuz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/glwkioget.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/grtfimrdn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/ginzdfofu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gzxqoqbyr.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gfgojpbcs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gmbttysft.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gkkezowkl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/grcxifyym.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gbktlnani.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gtdoypjpe.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gvswurxsh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/guiddrkba.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gurwaoscm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gzqmhizvs.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gqjbppgbs.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gbpgnzkak.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/guyzuxwwz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/glskwjhwe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/ggzclpajw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gfkmpdksw.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gbduqqffq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkcnpwxuj.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gxoqfvnjg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gmdmruqdi.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gdbchszgt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gzkpxmfbd.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gznmepobm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gqdantmsc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gpqzdofgk.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/grmdpdroa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gqrvemezn.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gykkfllgv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gupssdjzw.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gzcyjolfs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gmaokztyo.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gapsrnjdb.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gddfdeofc.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gxfjngkpj.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gabgasejf.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gkejhsxie.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gkexwfhdt.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gvibxkihn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/guguarxnf.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/ghgfaanyi.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gxarlncjv.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gvzfihfkb.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/ghmvffomr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gvlivbudn.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/goyluyaxn.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gwqbsiagw.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gypzgziqa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gtiesbwll.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gtgoreude.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/ggrfzbswo.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gecajiorc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gcvwhidko.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gqvvitfji.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gitvuuxiz.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gvyngxzgt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gbuhqrhav.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gurkqskvn.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gycnnlsvv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/ghdyklzvc.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gifbybvvy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/glfbxxezg.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gcvgszxmt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gbtuknjng.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/grcoddqnm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/guuxjvmmp.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gcurmkzrr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwdszaydi.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gtgimlpoa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmnprcwmm.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gqeeoohkr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpzxycnkf.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gvzzpfwfs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghmxacpnt.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gldvtqqet.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gngwztpvn.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/ghbxqeuun.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gcvzoxlsh.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gaoxjzmor.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gxuvvjwxc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/ggrxxfsue.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gaaiurcin.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/glhvlvclc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gsoafjgvw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfueufcmr.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/grfrrxirw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gqhzifgmk.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gofzopylo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gudezblfb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkphvgdil.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gljtzwlvc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghtfwbgzu.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gihqipctq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gjlvcqxot.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gykalxvzt.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gstwnsapa.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gqiqumfzm.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gieaumznj.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/goumwjokv.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gnswujupj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gpvqrgoqb.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/ggzaqrhxj.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gbfvrkrmt.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gqipfdwkv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gxeqoowbp.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gledsquqb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gzrlugvre.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gehcqavlv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gexmskpca.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gjhgcrunm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gqciysfom.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gzaszeuod.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gbtmdqktu.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/ggnxczwxp.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/guzzxodns.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gubeosagb.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/grufqpbct.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gehunqsoi.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gtsyonpru.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gexwqcvkq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/glyslwalp.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gijeiwrit.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gyuociiyf.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gewqgjhpm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/ginghswyu.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gergjoipr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gyrllfxxe.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gdkphehlq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gtcnntzee.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gdskhsyiw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gamoszayu.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gjqczjkmu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gadvnbjod.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfrzxggzj.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gpalxsrsf.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gkoltdmcm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gfwwhxoux.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gjwzxiiyc.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gvaduxcit.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gqygfhxvc.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gyahptxwx.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gdgmnjcuf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gxsecgazy.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gpxrzlcrb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/grgwhlwwh.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/ggoijvhzr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/glidxwklq.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gygrszdrz.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/ghilvuzur.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gwqtoxkya.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gaisfajpw.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gxeqzcfns.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gxvtfbhrq.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gefxqjpxo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gsnzfgtzg.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gvrldlpxs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gbskjfgnh.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gwvrljczs.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gtfdpznkr.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gnmnaqnxn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gaahusvzl.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/guucyihmw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gflndldeo.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gwerepgmp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/geynvttqx.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/geaaeddok.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gwrdsqbyd.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gevfwfgnn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gnvbmdszx.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gtbukjwtu.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/goslisjsm.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gmeifijzk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/ghvgrrpex.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gnrsmhnue.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gcpnuisil.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gdsamfmgw.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gcylqqyap.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gdfegiquq.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/grfqyiofz.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gmspeioxz.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gkljizoec.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gdnzlepqv.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gngiwaazh.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gdwtlquhx.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gymesvfcj.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/givroosez.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/ggjtwaojf.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gwjutnndd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/grhklyotw.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/ggptklynm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gckktnefy.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gtprcawzb.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gwtxmigof.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gqgnatahl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gvzxmodjv.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/grgmlemvx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gmhoybntl.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/guvbpgqpc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gespoigyh.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gnukxzkzr.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gjkgtqhzi.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gtztqhlzd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gcdxnkwpq.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gqeqbmqjc.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gihytxteq.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/guasfvlva.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gmlrxgtna.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gqctmhhpk.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gslxzrqxj.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/grxlvbeog.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gqqzxufvg.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gkxvqexnr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gdqicvxzi.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/ggfmszgyu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gnsprxram.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gzzktnvcw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gtgjpwyya.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gkdxhepmz.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gwihrlowz.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gjczyhjat.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/ghcbdppbf.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gzbjyftpi.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gguwnosqa.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gomwanbea.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gnsssojuz.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gyhpaicht.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/geonpuwao.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gtoduvuif.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/guvzshjjk.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/griksttys.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gaxlmymuy.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gphirdbad.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/grbqvseve.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gtmmsuoyb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gjizjlvfe.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gvfrwibrt.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/ggghmyfyd.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gasljupms.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gfprlwnlx.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/glvsxguag.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gfxbrowmx.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gggindqnj.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gfqvoembk.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gewgfkoay.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gpewzbvef.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gtxwjrfmv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gjksdgohl.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/giwbodvmo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gcyqvwmdo.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gbiswtpem.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gejshlhue.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/ghgxdqakn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gzanyacow.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gdwvrathf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gfrxqplck.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gbigpuwez.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gtrrhxkso.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjheoevev.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gbqeqbttn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gngulrhzv.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gptjlfhqp.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gxqijcvde.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gsnlagdcy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/ggwhetnim.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gtzhrybrp.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/ghtnbibce.sHtML


<!-- 参考信息 -->