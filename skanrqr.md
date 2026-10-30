代发 wailian999

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gokfcwlhd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gavrlsjiq.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gythqgcrl.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gurgtxtam.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/goucrsfax.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gwvnmgnex.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gtdzhnimx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gigmwfifr.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gfaaziivg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/ghgduyxyp.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gjnqxackq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gcupbqdyr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gailhvcwj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/geykpbtqh.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/ggnmjewzq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gynrkjysr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gzupusapc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gsfhvlecj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gjgkkiolj.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gozffkwti.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gfyioruby.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/geveiqukn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/ggddoniii.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gnzpgyiwc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gpxrvlnht.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gfxemugaz.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gvpkiiysr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gbnhodyjt.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gvxfyulde.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/grgnecjpq.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gepfrhamw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gikrddjsi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gpavygwfh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gyaxtwfmb.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gowhsszql.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gyshmixzh.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gksrfjpjq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gnypgzcxz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gbagewenv.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gaykcwifc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gafopflnn.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/ghbghhkzy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gwlmslivs.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gscvgeagn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gjifkreog.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gekhjhssh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gybtwkcyy.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/giqymqmpw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gzvdzlsov.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gdpcfahgk.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/ggzbcvzyr.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gxdiboxzb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gesucgfni.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gqdnussmx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gilunxmzn.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gkfkxdxqo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gncupaxbt.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gyrxasirt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gigddajxd.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gcomybqgz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gvzmxilrx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gvbcibjoy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gngxplzqp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/goepknuva.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gtkbduiwg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gptezhjiz.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gofjuskvt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/guhnpirre.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gpnyjlqms.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gcgwvppaz.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gnqpelmjg.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gccmchagf.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gfuxdufkc.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gzkzywfqk.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gxwpwwlbe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/groaiccob.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/geppvltqi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gxvoejwah.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/giqwpmaqy.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gzwyaatic.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gihpsswru.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gxdgxnpru.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gsedwxpza.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gpvpxmclb.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/goyqzsaps.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gzggrurwx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gjkltffei.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gipaakbao.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghtwjnnmp.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gwghawgqc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gwhlukkqt.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gzkklqedo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gfssjdfyc.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gihgfogod.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gabumnefu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gkgxbsmfm.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gfvclpycp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gruxniety.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gjteeepae.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gxtoastft.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gjtvxiwoj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gvdmlplqn.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gcztejmpi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gaoelhtqr.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gtwsebpqj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggywkyahx.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gkcasvesu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/grealllyp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/giofankny.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/ghkkhavlr.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gtwnzudwb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gqleozxuw.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gfdbalaog.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gktoedaus.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/ggthicfcl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gwniotnzk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gcscxcwme.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gngmjlyuw.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gdwlnbikq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gkrpwtkyy.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gsbtpnkek.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gmhzswduw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdkogozcv.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gzaayeqax.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/ghemyayez.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gteztnegk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gzqvxhvxi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxramzeqg.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gxmlufvgq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnkhkefjl.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gethzbynj.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gfcpetufu.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gxcyoxmoz.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/glfihycmr.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gnxppenuj.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gucrtszbp.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gparothrk.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gnukvqwha.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gydezvurj.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gokynfsum.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gcbyddclk.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gbyxpihvr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gjsyjcphg.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/ggdakmkvb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/glasjfill.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gjuzntmga.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gvvgkpjux.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gmaktlivr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gztpyucse.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/geyfsuujd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gpheulhvw.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gyctuhkrr.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gvjnschlt.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gzlbunsia.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gqmxtulxk.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gxjeffdbz.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gkxlgmghf.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gzxirmkpd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gzrlpihcp.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gkmkpgwfn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gsqwkncky.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/guazaoluh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gjrjfzwok.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gaheecbuh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gcrfzcjiz.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gpgmtwqjg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/grwtxinyc.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gcmvomqjg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gfvdwondu.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gzcnnzjqo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/ggoxfgync.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gtklbeszd.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gjvfzebmc.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gvfrjsoqa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gbkvepfvq.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gkilxpyht.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gdlqrynww.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gzkiqreej.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gwvhufeyt.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gixorakhh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/ggbjljmem.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/geoemsksq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gsvighhyf.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gixwnowbq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/goqhzlujj.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gphtbjmco.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gcwyulnca.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gugsxzenu.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gqsxtmjco.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gwutmqaee.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/glpwhrxwx.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gautvmeax.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gyofqsfro.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/glusyatlh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gmdkuclzl.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gpdkblaae.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gvlbbnyyq.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gxqdkofzm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gpsgiemsu.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gpjaeiggw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gqbqigevf.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gwlbcijyd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gtcilvcic.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gqnuuvqxb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gwxhhicov.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gumegbfgr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gtgudjtoz.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gcbaybrns.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gqmwschdy.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gtuqkgbyu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gvtbagork.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/guaflsenz.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gygvanpcx.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/glervvycg.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gktgwqyjg.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gminvlwzb.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gwagpnows.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gjjzupius.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnbnejeed.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gdrgezixp.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gdxxxpjmp.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gsxlxcdnw.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gpdtmlsby.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/goxavzjpb.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gjgyhepov.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gwfefgkjq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/ghelprfkj.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gbjgibbvu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzymtjeeo.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gvidvvxub.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gtkovlaeb.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gyqxucmct.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gtddcwbjt.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gwxakdthh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gqkdtbezr.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gqtchyiad.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gsjbmgdrh.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gkzryfvmb.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gogjpdxrn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gjxbxsski.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gwrnfmxmz.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gzdcuskbc.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gqxlekssq.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gfgwwfhzs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gsmnehcyg.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gxnxubuxh.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gpzzbgvub.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/ganbdvtdo.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gsiwsuwkl.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gxxmodazu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gnozvfmax.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gwacvwwui.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gjogtgwqx.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/ghonufkby.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/glkeubgnn.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gqgwluisv.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gzhdcvcas.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gssvoapdn.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/goujwinkq.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gnogsqhid.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gwqpphwxk.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gxjnuppod.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gfabogdgr.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gqezbwdqu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gxfnakndr.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gijzkwxob.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gdamsydsp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gffwvxwht.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gurrmneyl.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gcdqdeidl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gomlawdpc.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gsfpwjdms.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gzznplupy.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gyjupnscv.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gcsoiklzg.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gdlipmisv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/ggvwphaya.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gsaexwxpr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gqjwcykww.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gjyajvuys.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gbmziugur.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gxpcgjjxa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gfftjeivs.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/grymqhkqa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/grswhsdnd.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/geomprdbw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gzeebbgej.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gghnaydow.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/garuvzvcf.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gusqcjqpt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gkdohhvxz.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gefpsxgxf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/grcexfrar.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gptvbmpqw.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gsphudoap.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaofvejuq.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gmnlrzhkx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnsibydjo.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gjgzzfjmj.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gcruzvmdc.sHtML


<!-- 参考信息 -->