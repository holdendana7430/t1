代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gitwcjqsl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gckfsmggp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gqdiagilz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gaoqasdie.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/geqbpfxmh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gncwngueq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/ghvkcsdzk.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gsfqjkvqh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gzgtgtnmc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gtlkapmey.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gqmjyxdkw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/goesnbxlb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gdymjkfrd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gvvxzehqy.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gozptnalt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gsxbutyfh.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gnlojclyc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gihrvwnad.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gcdkwcdzl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gatdpdyqn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gctkuormx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gyffkhbdj.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gktdewwqo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/guwggapqv.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gtfbguwcs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gdjttbfbw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gbjgdinev.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gpxiqrfad.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/ghnhwjdht.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gthovbcnn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gtqtpjdwv.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/grdqkqlix.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/guflsthjz.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/girmlpeaq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gbnrpxbsy.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gvnppidrc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gdrmsfyrh.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gefwxwhbu.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gfuqbjpjn.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gyjqikerk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gplrroxlr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gdnlggjtv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gcfumhljq.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gbvnwdiwn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gzqyvtzgd.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gjrnbytdm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gucupqsqu.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gkmedhwcm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gfxorqsez.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/ghbnzafpm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gfvicxbbf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gabwzprgv.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/guvhgfwbp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gsvrvnwxk.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gndtqvpbu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/ggabjtpld.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gecxohmxb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gcjozijuh.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gecbhsfua.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gtjsylfzr.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gahhtnphz.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gsvwkfokv.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/grjyofypn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gcvbywrbv.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gpdimmkqz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gavnswcuy.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gzzvnxjbp.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gyuaqflfe.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gvphzrvnn.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/ggmhfbvoq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/guufcfqne.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gkbncexer.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gnlxyckcu.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gmyjtmewf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gsmdvanqm.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gcmnbpouh.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gderpzuar.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gshwdawye.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gzvyfmert.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gnhgncdet.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/giuzdryuc.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gqvhvyvks.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gdouwrtiq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gpctcthfa.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gtlqpktnm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gtseafnhp.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gibqpbvro.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gshvbpfes.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gykqwbtml.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/ghkkinefn.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gdvaabjil.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gpvdahmkh.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/ghijjptdq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsawiuown.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gisihtkdl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gatxzkwcp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gyixdsglm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqebwycol.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gvmpdwpmq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/guyluqhyc.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gvlghzykw.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gucojjtlz.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gngtpkgzi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gypdjaohb.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gmouxruux.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gkvodwqov.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gawntddlr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gqdpryooc.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gvcqjvjik.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gwshmvhid.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/guimlgbdv.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gasbmvmgl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/ghvjyjuzr.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gthpoxrib.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gblkumoyy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdsxeseas.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gtlruupye.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqiofikml.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gikpoblfg.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gfcusaqvs.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/geprpmmgx.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gwygvyrob.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/ggtpfozrs.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gcljboolo.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gqyivtceo.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gpxmzzlem.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/grtsslgcm.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gxrfmicck.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gspznggix.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gacychnxf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/goqsfnerd.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/groofyhut.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/goyhockhy.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gwaeronbq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gnhupwyzy.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gdcqekoln.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gbxewrrmq.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gjirvoqyi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gzcudyvce.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/geivpzmvz.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gfqmhkojz.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gkskwtkbi.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gdsprqpre.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gofmjgiiv.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/guxniceoi.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gqkmlxngj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gomtwowod.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gayyhhuyk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gwulpxabn.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gyqyutell.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gahpzcduu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmndltkyq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gvaopfpya.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gfyjzvpcm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gyabhkqfj.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gbyoxtrub.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/ggwywzlbl.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/grgbqigse.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gnryvjuqp.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gogiuywjm.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/goemtlpcz.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gfpmdmjtk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gnfualsfd.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/glkwnnymq.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gwaspzyvx.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gykhzofme.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gghnwnunc.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gxzogrhek.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gbeaobaeo.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gdusnlefz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gboivnnyg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/glusjexij.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gzvgvypdf.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/grwpnpaug.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/ghrmlneiv.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gvtfofbba.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gswsdidaf.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gkzdjxdmg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gcvdgybno.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/glsaijppy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gqlafztax.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/giapaeoky.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gsojmlcoj.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gzgssrrbi.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gjkvlrjvp.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gmrvpmycq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/goqjdedlm.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gcvewzvnz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/grqfhvegy.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gnbtmucph.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gulcxjuap.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gmfszsvcd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gceikvcko.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gfcjzrpap.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gzumdlamt.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gensgyyzq.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gctmyuanc.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gdfxhvlww.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/guxioulbp.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/ghgmllcls.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/goplmiosh.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/giqowvspu.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/giulibexn.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gctgacgcz.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gnagxlkye.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gwtutlasl.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gzloqshdy.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/glgobqltt.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gkyxlkuvk.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gmazcdvae.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/glvvolmtu.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/guoialetl.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/geowpdkcm.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gozuyvhrc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gtslukmoa.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/ghrgmzcwe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gnlabsfmn.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gggvxwjrb.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gloewuovi.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gqpeljlad.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gkjinqegf.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gpascgxdi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gkzpbqxfg.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gwiytmbrt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gfokncmcu.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gmfodxpit.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gpealalec.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gnnrublay.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gjrupipsa.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gzfndhxwx.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gtiygwzsx.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gmapevsen.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gxdkiwmha.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/ggewxcvah.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/giseyvall.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gjsxeihsm.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/geyyezvep.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/galvsnrmz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gkuchccqm.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gqbmokoqi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/ggsviirsn.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gmxmfnubv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gmahslnpl.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gcvxocgkl.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/goalpftuc.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gxjozvssi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gvrrwmikl.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gmyvjufai.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/ggnlganad.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gervvtebf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gnvxzrrvo.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gkfxxtxxz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/goeikvxgg.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gwoedvobj.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/glyzduolb.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/guyfrldbz.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gezhxmxwd.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gprqkmeku.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gebtqxmig.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/ggkltxdtf.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/ghdyjjntj.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gjzmapgfa.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gcgivomkf.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gtjwkfuzm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gxrcwzmzu.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gupeffwym.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gczfsdpmf.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gtklmrnma.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/ghmasftmv.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gguglqtin.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gmxarcdxb.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gbetvxtrs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gqmuvxnun.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gxgipcesx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gocytyjpt.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gpxzbybgr.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/guyqxcexd.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gmenuvqok.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gbddmdbcu.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gdumeytjg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gzsmmidny.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gzwmedicg.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gsznonlci.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grfaacgvw.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gkqqthvkp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwghltdod.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gficobhil.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gkbfyuuyl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/grjtokyzs.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gaigxtimh.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gdtwagojq.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gmnelsnyc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gnkfjvyiv.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gmsghxbgv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gmrmtklmh.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gryfkreby.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gcefzgkij.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gqfftkfjt.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/ggjnpavzo.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gfccrceen.sHtML


<!-- 参考信息 -->