代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gfvulqkvt.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytfrpnkc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gxqiitfgi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneitnhpd.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgoxgque.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidtxrsiz.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gpeuhwxin.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynpknrfu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gomwlqkvj.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlzqnafb.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gvoywqmqk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyvqzkdr.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gqgltvqmk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakzuyknn.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gudamvvqz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/ghpkqkuqq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhcbokng.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpykvrwl.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlmfcbrq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gxctcyvkm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gizsiytdt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggntqdglv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqfoyoyj.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gayhmsgax.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gyxetyttr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/guacupsxu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/giglstrnz.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvjbuqqh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gflkxyxse.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gbbcdqhtq.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdscxhjt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsohzddwv.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gnhyefdyq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gxamjqbxo.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/glxglkpwx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gpkpthykn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gllrfojwd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gwsbftube.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/ghklzmpzk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gidrhmpil.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govssjocc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gtdanzgzx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbksjfxcs.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbgpbgyg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gumfpwgph.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjaphxin.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gnwqsgomn.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guksqbopn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/geaxzaccp.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gaskojayq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtmderoo.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/glshxaoer.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gkqhuxzbr.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gvziaebzj.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gtkldyvlt.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuxplamy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvwhvuan.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gviezwpav.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqktodyk.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwoyrbzy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghekpadjk.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gclhatuwf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gxjmqwtyh.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxzkatvp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gkyptxvlr.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/getbprtyw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gwchyzdni.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gwlqzwmay.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gilvjqanc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gcyvpnfft.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gslbarzrn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/galgoogsf.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gwnehtmtv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/guqwhxwts.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gloatlcjd.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzobhoyh.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gnkwbuzmw.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnaasukv.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesbdvfyz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqmerpvt.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/giixdyifd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdkyqhop.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gqvzjjanq.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gqbhhxtfj.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gkitvhudy.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/geowqdvtg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gjxbujdem.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gxplvkclj.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtslxuusj.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcdshvco.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gytxpqlbn.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gijuujnre.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmauyuwhp.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/ghdsxmght.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzszcicz.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gycewfaik.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/glphegjbq.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsqtagvs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfbcdetq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjaykuvr.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczqugqmx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gkcjkaocs.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihufxvtq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbutlxaf.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcorpdkye.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gadqnqjur.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gndjncjhi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqdmryir.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gjimbickf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gawgjqdvy.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gedremngm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gkwvwahgl.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbbjogjmr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/glguzisbw.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxqdidgk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glpsjdlyc.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gudcgbfvv.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gglozxjaz.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gcempadpc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gktknxkcc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujfvzwhi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gbvsnkpzl.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gylzhebbb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gpqghyuhn.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gocgpieeb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxlcvinw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gaqodoqdi.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gtetnbumi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/grmxioabk.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gvgbnuoog.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/godcqtood.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfzqugba.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gagotmepw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gubroqudt.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/ghdsxnodl.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoirncul.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsyralmt.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/grhfxpwen.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gkpxdrjgr.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgsrhqru.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gfyqggpkv.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxitctib.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzeewevz.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gknmqvmmv.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwszvbgoy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqdarmbf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gquludqgu.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhtosvox.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gkckacxfx.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfckfpbp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqppeadp.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqsggotq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gzthfrucf.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyxqdmpa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqlhuxxg.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofworowi.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtocfxedq.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuuiisab.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkhicape.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonsjadxy.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbisfged.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxazgcdn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gusxegazc.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gvovuethm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsyxkonr.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpnmhlry.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwieshqba.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzqrdqva.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwabmgydo.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpqpbulk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/goanflwhm.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gnytrsrdx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/grpezutpf.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gurbkffqi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptfjbgiu.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gogsslkmn.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuwjxviw.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gdgdyecdn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamtdkgsn.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgoaiyxy.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxewqodb.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/glqnrmhth.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwpknqynj.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwyvamln.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjlhpors.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjectoef.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/godvpfoxv.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gzxhmqjwc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggnwmgeva.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/geekmuaga.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/givkpksud.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/ggphvxcgh.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gntprfghz.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gfyzlikof.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgrltptn.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtywrqtyx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gptqvxxdk.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gqarueacd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/grvcwqvin.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvowfvtv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gccnagijo.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginbvgqdc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzobqexs.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gimrqmqyh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gettqmzdm.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gbgkrgbpf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/glhwerxhd.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gecqijrdp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gubeepvwr.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtctnmgz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gpffjzeqd.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gszaknqme.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsndxzqy.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/giqpmjyyh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gsrpsdpqg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gldhvzdra.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqmyprrt.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoflhjwi.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gpdhbpswx.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmbjltif.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfipdtdp.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvvbzogv.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfmjecfhr.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvutzkcfg.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/glkxhwhme.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/geitgjwhx.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/ghyxxjyop.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gydlejskf.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/giyuvymqg.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gsshfltbb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrobfsos.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnzjeflv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmuojfrls.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/ggeidjsug.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/guuheaawu.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gdrvwecdl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpiqgasm.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gxvnhaqvw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyemzcrge.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gqjwyekfe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gulluoiee.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/grwsbmeaw.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/giiducxao.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdqbwesk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/goywcyfst.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/glcoqwjev.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpwvgxqzx.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gvumcpfcm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gbrmkpwoz.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gteanihzm.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/giozmmuwy.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbcepjiw.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxefzcwx.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnzkvtgr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/ghchlxdcv.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiemkgoz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/ginezattu.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gfbyenytn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gfhplhtff.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ghglnnjiy.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvdesdnh.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccnjdixr.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/ghwwbczkw.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/glccklhdg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwfolknl.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/grycwavlt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gskugaymq.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnwhogaf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gpahhamdi.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcwmured.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxdpybgf.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvnbqogg.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gljuusqsb.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoonkyvw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/goyxvvrrd.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnntlwlyy.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gomaxsgbz.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdhoaqoy.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geagozusw.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzgjzncj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gouncvmcw.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gevqtaqay.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/grgviwney.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gjukayiac.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwclfaio.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gpgkujpvb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytwxhabp.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbckmkqm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxtbojlo.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/grkdlctyl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/garbzkrdv.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvktrqah.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gmluybxlc.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gixunvmto.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzlxrrdo.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkiyfiae.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtjiiemsi.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/grgmgxamb.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbtgczst.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdnrtkpg.sHtML


<!-- 参考信息 -->