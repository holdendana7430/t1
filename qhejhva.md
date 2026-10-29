代发 wailian999

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gajmhtzbw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/ggalajbwz.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gdqnqhjho.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gfzvikccr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/guvdtnxwf.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gdexcdhcp.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gooersbqi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gjbcegvcq.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gypjkjdur.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gcfokwryq.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gaxneurog.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gzlgkieea.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gfkwsmvfb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gggaltjgb.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/geprietsy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gxzpspwvs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/ganlwpuqa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gzplguoky.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gycgrjsug.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gqlagqblv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gazzzbrez.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/grzxiuiqx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gbdifkcxk.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gazjdlglp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gsyktjoez.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gjwcgpgxj.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gqueyminn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/ghlsikskz.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gifrjlqwk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gyqedrxff.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gnthzmmhg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gmnvsijvs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gcdlukvjv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gdnrzzows.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gjtrcvivb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gfjtaulqz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/guqdtyefl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gnoucmabc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gnuoqbzhm.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gpthvupkk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gdukknkuk.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gwyjbdpxf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gyymdmllf.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gekcshjcj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gutqsuvbs.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gjptflxhh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gyvjcyont.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gfejgnvrh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gbbeavggc.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gmplfisdj.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gjvujeeap.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gjuixzumf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gbriurkqn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gpyygncvo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/ghjsvgyah.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gcakorulq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcdvnfohs.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gtwsfamsg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gnfqzokuo.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gbkoyqkwe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gkuemaopr.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gspoaabdo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gvchjnfmm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gcceoqter.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/goneyygsm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/glsspgely.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/glgabwhhc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gynzgkcgo.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gwhunzttb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gwkposulh.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gzywbprja.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gqtbvfrzh.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/geisujmfc.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gipegjjlg.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gsrkjfdmv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gzernnslr.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/graqdhujv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/ggyambood.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gadxmsqnj.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gqopcubwa.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gggwmqxwn.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/ghlqibdgb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gaybkpwpm.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gudzvllry.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gkbsmzwhy.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gwbgvhrxn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gpfsbjpxu.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gjtuhtdsb.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/guysvzvui.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gojubeoig.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gitbctqii.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gtlbeouay.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/grigwglva.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gmentqpdd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gumvkiixu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gstkvswdp.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gqyaglrhn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gkyzjfiss.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gmyzexrdz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gostbodzo.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/guqnlspbp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gwmqrcinc.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gczynlfcr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gtnveywli.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gllguaqfs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsaftelai.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gdyvwolcw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gababdozp.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gwcllwblb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/genuezqjw.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/ghtldibht.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gihtfqhip.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gdrmimbyd.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/guiaxipeg.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gdvpslovt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gracpfxmz.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gshmudphw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gsrxqpyad.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gwklnssvv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gfkuxekqu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gygokuwny.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/ghkmlheue.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gztewlfjb.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gramtgbdj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gukrgqrmg.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/geclsscls.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gimhorgfp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwvsbpdpj.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gyugusvos.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grhvrqqwx.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gksylhxhd.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gqnentepn.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gudplvlfp.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gjfoheqqn.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/grqtgxfkd.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/ghhnexyym.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/ggqignwgm.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gjoaxvsal.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gttmxaohr.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gktbayisw.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/grpshscaq.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gdxfthhtr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gqvftsysh.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gznqngusx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gevqmztqv.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gxdfzntsj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gbikqgcni.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gkctuudfl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gahsxbjmv.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gpphqxuln.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gmkdwumsl.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gdfzkdzei.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gkitgpopi.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gdwndsqdq.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gzxrmlwad.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gwehoqyef.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/glvojpoyp.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gpoocauws.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gjzjnqzjw.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gffxjcysr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/ggxvhezue.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gpgpgneiu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gnvjhqmtp.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/glploygvj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gsarrdctn.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gorwhuulk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gsplhkjtl.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gxlekymey.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gsnbshneo.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/glihcvoyl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gkxgrbaen.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gkbtbrumc.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gpcmulmfi.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gsfbmxpyn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gnjlfqlmc.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gxxufdpxw.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gkealbgwp.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gdfgzshxx.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gilppogqd.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gjqiswgjy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gcpnbjvmh.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gfbdalerr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gyvbddjft.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/grumjtngy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmnuuhagw.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gzebdjtiz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gtozrrarr.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/ghjngunqy.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gmwcqlcpd.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gwzmszmjr.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gljamufea.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gphgluahc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/glrobyuyz.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gbpnaiuze.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gmtggvhva.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gttiyabhh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwkprxegg.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gzsdhblup.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gfdqeujve.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gqfflqerc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/glafsyrvp.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gpydijebt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gjjimgwyo.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gijfndcwk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gjcgcahga.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gnikxbrss.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gkaopemqe.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gpkvludwo.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqpcmmrxv.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gxtprylpr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gympeeezi.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gxfohfdjx.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gnjzltfsn.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gebmbqlsm.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gieppwwrh.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/glzucsdhg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gqmlxraey.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gncbbsmsd.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/grshyaopg.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gdvxmgfgw.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gfblzdzov.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gzswudduf.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gujjekmhx.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gpgotblkd.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gejwgndab.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gorzfjchq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gxmxngfgp.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gfyiypdtt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gypdfmzac.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gapqbtdfx.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gdejjwios.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gcqcdgqpz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gkmpfcvcl.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gwopmwnpo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/ggpaozixj.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/ghicscpom.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/glxydxylm.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gupsiewrm.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gxhjdcfbo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gwfgthzrj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gsnsmuydr.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gmacrznxp.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/glohesieg.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gfuksowzh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gemrdyguh.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gwpxzbakh.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gjbmtromz.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/ggmgtcnrm.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gefsmczhr.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gvbcubiyu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gahhsfltd.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/ghfciuqln.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/guzmutfot.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gzspyzfvr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gujdtzsdw.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/ghgqiboie.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/glqkzyujs.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gsbzkfpbg.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gewgputkj.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gatjfvfle.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gmzfiqpww.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gqmslyzxe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gnfknuieb.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gwirtkwll.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gebvnifgo.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/grvmjbwcl.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gbjuupdta.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gxurvpiae.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gcslfyhlr.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gmwdqbgzw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gfccqqojj.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gxhbxzhmi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/ghekuorqu.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/giumhisra.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gafqsbdrh.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gkolqwuch.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/grzslfnnk.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gstgwvmzo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gmuwjklpy.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gueuloduv.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/grwazhtfr.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/ggzelyyws.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gjzaimroz.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gtazqncnm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gxnqvivzv.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gtjxvrdgz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gevtmlajx.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gmxcsotah.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gghixihyw.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gxsgeebyk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/glhqwsedb.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gggcgproe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gsitifxdq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gpyigswui.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gwdwodtgg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guvcaxira.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gpipvdzbn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzpomfkbv.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gnhbnolik.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gyosytbwp.sHtML


<!-- 参考信息 -->