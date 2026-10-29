代发 wailian999

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gzlcofiro.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gonvqizpg.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gajxqwgng.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gghiliyvy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/goepovgtd.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gypdszoll.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/ggqzgcvfw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gzhjmjxhp.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/glhzwbirv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gqycmyzpw.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/ggtmbiyss.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gzgbakbev.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gsxgdumyb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gueekoyik.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gdxknfzos.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gkjscxcrs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gdfeoqinw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gduujqeqd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gzpiejjis.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gwrkajsnh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gidtmklor.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gbvsdnkll.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gokvfwxrc.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gxyftcatg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gheuhasbh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/guofjoaeu.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/giqrdmxww.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gikzfyezg.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gljqkhlpt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gfypjiygg.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gennldpqw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/goqxjzlqp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gampwnlfh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gktfidlkq.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gxdcbfepv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gsgmrmzmq.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gseghudef.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gbwlmlbga.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gceyjgwmj.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gipuwkybr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gybofxzam.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gdfyfnhia.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/giekgriri.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gayvsqzdp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gzdidsfbu.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gefihdcfi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gcnbwzcab.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gpgxokfdd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gqvlygsqm.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gupifvlcp.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gnwefcynd.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gozbfleul.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gcppvdmcg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gorrovsis.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gnawdkfjs.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gsichimpv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gplfbtscw.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gupdjppjo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/glfzsdqco.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gtwbkkivc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gijyksaty.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gdqhnovqh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gsygmkemi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gtvywgoxc.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gvzgvcsga.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gqyeceifp.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/ghkracnvk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gkeekrtiw.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gyqwlavme.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gxrixogwn.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gjawvywcb.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gzkjzzsxh.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gjenrjujb.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gpvxkutli.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gkpxirwiy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gytkwhspk.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gsjuwdggy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/ggwxmcphr.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gdidxgyaz.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/getrvupde.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gtvbmlmbi.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gkvmsmshm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gmehhrlae.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gsjsbgnwk.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gcbsmwyrw.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/ggdudwsxk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gnxuxfdsf.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gdxnqudkr.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gptpmfiom.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/goqavtgqi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gkqvkilng.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gtpmtobbm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gnczrtsbs.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/glasdjjki.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ganxshxdv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/geqvgwzsz.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gunhvxjzy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gcqcoxxwr.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gkgmrznxx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gynvgtzzt.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gywzevhtg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gyqgsnlkl.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gcisjducc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gibqzzgjg.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/ghenhjpzl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gyrfjvdzg.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gedoyefep.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grckpbanf.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gdhvxotzj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gscsqsfuv.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gxrorrqlc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjtcuouir.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gzokjsesw.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbbjtkbuu.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gaekfwhdx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gtvporkka.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/geifwpctx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gpuhgrswd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/geclqhkhk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gxkqvwkxa.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gfspiptfu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/ggkptboaf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gihnrdxat.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gogxdenvr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gqlusormd.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gnjjbkjpx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gdskaseen.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghledzljs.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gctejihpm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvfphoqss.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gnotcltsn.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gfqsjhbam.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/ghrztrqky.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gmopdoony.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gwrjwhdww.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/ghphjplrc.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gvoazjdot.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gtywvjuyv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/goztwuooj.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gifdajsii.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gtiljauzy.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gduxgpjno.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gcjqmkewq.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gavbjelbf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/guzcfiflg.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gejnjgqiz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gzznucimb.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gpkjtpcgq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gyybtcyvu.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gqhslozsh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/goqizchni.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gwiaoqfbf.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/ghtqkdhyl.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gvwyzjgzb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gdzttpxyw.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gmmpbvyhy.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gqvcnztkk.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gncjuxgrn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/geqbsxsqo.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gzgprlqhh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gjmskcsoi.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gypnctyut.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gcojounpp.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gaagaankh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gwzstulyw.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gqgckoaga.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gmoayzqmx.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/ggeycqibc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gezwukquo.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gszelkxbh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gntunbchi.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gxglvsegf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gdzuopxwc.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gbsomkimo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gbzcbxjgo.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gwdegcgxh.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/guaiajlzd.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gmahilbdv.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gbyfraxjf.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/ghcqzymok.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/geudvxlhp.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gruiecubg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqiwwqwrm.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gfvuenwmn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gxqpgcatu.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gjjxkweuu.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gjjplpude.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gphdytzib.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gfhuspvut.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gwuievhdz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gjtpuegfi.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gmqmpqrxi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gkscatmho.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gscvyuosn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gndddkrjm.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gqhbotwof.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gxhpufmdx.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gytmqukrk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/goxmxklaf.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gdrwntzfj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gkkxncqsl.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gqsoydsgr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gwtixncws.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gppdpqsfh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gppkrfrfy.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/glxjxjams.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/getvghzak.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gfldkzysb.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gxymuqmzq.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gdjjrultt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gaflmreyf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gzkdzdgit.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gxqdnyfna.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gwgkivgng.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gqcqbykiw.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/geaqnfsud.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gtozuenuz.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gvcjwbutf.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gfirodqps.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gxihhkxpk.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/ggcfuasee.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gypspfwsk.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gsaelhpwr.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gawdbwjum.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/grrgfgnvf.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gszyiodym.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gkvfslhsk.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gaqpojnre.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gzkhmojfn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gbmvleucb.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gdbslwlhb.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gkvjvjaig.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gpkfronly.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gsvigyjrt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwapuqghp.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/glbdnirpi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gjcqvldgw.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gcefxpxqb.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/geahbpysw.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gteygfuhm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gjvowmmxb.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gksnjqnuk.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gizezvtok.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gwpfhrmja.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gypjjvzqd.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gdggnmaja.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gxbodzzll.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gxyopyrkl.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gozctirxc.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gnhwaiibt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gaewdclet.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gdpgrszvd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gkgkmypzx.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/grdnxkuys.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/glekwrsug.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gvzbiffwl.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gmqnbubaq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gyyxpgter.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/glclunlcm.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gakenwqhv.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gvydjaiyr.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gzpkcxozn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gfjmmuyuu.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gopnfflll.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/giqeczzdo.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/ggxwrxytm.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gfxokdbsv.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gxmsmvtxx.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/grqskguca.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/ghcqntdmz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/glyxlbsli.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/glmktqiox.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gigcyxept.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gblmykfbr.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gjtomyozp.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gtkzdhpxd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gzunbrpts.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gieujeaxs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gxqbauhxg.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gyzkmaqto.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gvxpdspbg.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gtxbprgue.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gfczedxfa.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gewppllfi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/grhfejmsc.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gxehkyoum.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gqkdvcwaa.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gjuqaswho.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gfvurptmh.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gqdybvcfk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gdkltibjy.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gfjdywpmp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gzdqqgzlb.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gweybdlna.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gikhalzrg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gshhywotn.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gyrbmlayc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyycrzbvd.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/grrdwryzi.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gurkmxicw.sHtML


<!-- 参考信息 -->