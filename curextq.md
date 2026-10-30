代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gxpdsppxs.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gqsuanvzh.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gxokjarev.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gfobcswdj.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gulinxqkz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/giqarjvit.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gnbxzqxik.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/ginsyifxu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/ggsgsqrvw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gmtlwwufp.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gnxrfchvf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/glguysjqd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gpvnzfzvd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gcetkqeac.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gxnmqklyp.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gdouffdmz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gbvvfscxy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gjugbloop.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/grqxthxvm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gloqmlycq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/guysbiuta.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gchmcuilk.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gfltuowxv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gloclyjtg.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/guhbwddwo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gmqagfkll.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gyjvrbdru.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gblhjgukl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/grdrcfswd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/glgcajobl.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gleomjntx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gzafspbon.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gjctyvdou.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gxqfunhda.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/glykxnfdu.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gsgclqlos.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/grtxeouxq.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gngeajzwu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gxysapons.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gomloloue.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gxkjycukq.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gfufkrvgv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gsvvvuuox.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gybgrlprl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gyaqjovwi.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gddjabmis.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gzkygzzrk.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gypccmfwh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gmurkepyk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gobtfeoxf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gzxpjbggm.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gynzfhipw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gdevkifru.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gcckjaqgs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gxqniwxll.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gwkxlbmle.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gsmpgupib.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gyeehxthm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gglxqhhbg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gzljlxehp.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gjroxxdtj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/glsczzguf.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gtsimfnny.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gagzzwajq.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gxdteoaqy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gfmtedzpx.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gbzidmboz.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gmzmscqwu.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/grstvbgve.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gznrilngo.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gclvkivuq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gqimagvto.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/grabmgujp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/glbewkcwu.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gksyixqhw.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gpgvxooxf.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gkofbojuu.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gakpxfgov.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/grxxmvpka.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gcjatdoib.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gjncdugga.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gtqattond.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gyjykqnuo.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gamqtkfsh.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwikrpfcj.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gbmpdxxit.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/giztxwmju.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gchohpncy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gkpadwlqm.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gmysnmpcr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxwkbupsp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/ghzmmrfiw.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gjdvlflho.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/grjhogilk.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gztubdtbn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gwdqpxlej.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gapwebpor.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gidgpliah.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gsemvatgh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gnwclfany.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gsnajsziq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbkxmqqrt.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gesesrafw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggleilbbb.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gkkvjljan.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gefhersto.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gbwflxyah.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvgscopdb.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/grfgpldpm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/goatqyjla.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gipeajejt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/giexqijwg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gxjpenmuf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gbkbpmqvk.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gbhgbkpdf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gtwjhshbn.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/guvtoupcw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gvglxmtru.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/glyenxtbh.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gqybfjzcw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gvfihfyjm.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/ggpbhrrdw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/grshkzatz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvwxyvnoo.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gieaeyisi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvygatmhc.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gygtovzzm.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/ghnefjcsz.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gbahmmsbv.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gkkjrejan.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/grfgjusft.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/grqqghdep.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gleqjiisj.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/ghvipcxjf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gsbuuurby.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gynfhmuyr.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/geionrhye.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gbezabbxq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gypkrcncu.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gnxxmwmua.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gatdetzsm.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gutnadatt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gwhskrheg.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gykrpfnjl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gshlytzfs.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gwppcjsoe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gtnjknfbr.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gazluvkxb.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gjqzjkrjv.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gperdtyrn.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gwljxxbfa.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gkrfrawdu.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gevzibphr.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gvsedzadi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/grucdlpvc.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gxlirzoxd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gseetrkhh.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gwpktpdyf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/grejonsdv.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/ggibpfypl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/goxjviskf.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gljsbxsxb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gnigaurok.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gknqzwsgb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gctuiylef.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gskbpuubs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gnlauryif.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gtuzdkenz.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gfpnjwiww.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gqdlhfvdn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gcluygmxn.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gypkuhwup.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gdoqthehq.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gqhjjfzkr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqaiucidc.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gvjxjycfk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gszndngxe.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gkjpstkah.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsmkrolhg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gtomooqja.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/grsfizdmd.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gbllzjdwb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gegxjvxev.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gyxrebhqu.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/ghypwkbds.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gulwqbccd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/geyodczjb.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gscssyyse.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gonzouctt.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gdrxgrgbw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gemqxsjvl.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gzvxwlrid.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gmsnoxklh.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/grhcxiwcm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gpdakamrn.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gmagmkmvr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gfupyyohi.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gmavuckud.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gvdalbnsh.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gundvmdfd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gcpigwcmg.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gnvqjsilr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gppgkcbry.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gynlfgcme.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gonxwegvp.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gquarwmrc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/guzjaihjr.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gsmssgujf.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gafovmmzc.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gdgrojhka.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gyvejkhzu.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gyxvwumwb.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gvrpcskrg.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/ggkxnlwjo.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gkwwjujii.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/grfovbozn.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gjgtsolcv.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gmimgjgyb.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gksrrqdgb.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gzkqtwzxg.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/grhohcmno.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gixnjgluv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gmegbvywv.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/glcapfrge.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gwxbtgiay.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gyercszkh.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gaqkrhycg.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gjinexxsz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gvnnhhwqj.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gvkeneuop.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gngubwooj.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gxgdwghxl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gquigoarb.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gzxeosaaa.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gdfqnnxto.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gljuwyhzj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gghhasyed.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gsrzavmrh.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gyimljebe.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gqsqcpcpi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gkubxznaf.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gdtzqcobl.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gljbmftno.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gvpgwyzyh.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gapgbueat.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gukrzgwzk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gsbrqiomn.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gqawurhzi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/grzkwrhrr.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gxfxfhnxu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gpxonanpa.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gvbonkekx.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gyknkgddi.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gunbfxxfz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gvxuvdoit.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gsyksrcag.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gwyiiddgd.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gcisabzlo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/grgklmcnh.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gytjoezwr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gqhdlrstc.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gznfwyfgd.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gyzahdskz.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gbxuubjnr.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gqqoyozji.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gscvmmqyb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gxxivoftd.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gkugeppza.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gkzphhkms.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gildciscg.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gvhptcejd.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gwnqitaln.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gcimrlbnl.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gzvnlvckf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gcbvklplu.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gbycgycyt.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gofhweats.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gubroshic.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gyznkjrbv.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gjolnslqc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gswkzxteh.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gucnlodfq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gbjroguqg.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gmbcwfcso.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/ghjbweatf.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gxqqvwkol.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/globhopvn.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/grggrhubw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gdmgudtqz.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gkmsqbbuh.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gtzfhrnot.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcrzojzgr.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gfhksnqkw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gesvjtaqg.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjqzpozja.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/grctqyniw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gvxepbpoo.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gvtnpbndb.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gmsabwjsa.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gmgdrdzpb.sHtML


<!-- 参考信息 -->