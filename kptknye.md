代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gcnsgyjfy.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gixhksbee.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gbekpzfqb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/giodwfajg.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gaadtgkoe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwlfypwh.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxxdkcgn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/ggznsljbu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gimfegbwp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goakwnqlc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygsmudni.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gyaozkpoi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/glkedpggz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhbzbfph.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gcyqtinrf.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgbjuvie.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gvuptucpm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejpuhxhm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyypnuqj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/grcaxtfcz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gphqxhqjb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmvujnzc.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxgyzicq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gekbdkqnc.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gzqxkcdck.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/guecdwstn.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/guyhojfxu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmrbvmhs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gqgxhhmxz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gmmofuhen.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfogitbe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/grugoyvxd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvbsksio.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/glqauhbdd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/ggldvkctj.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpsvjwxk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gvfquysun.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtgjbmkb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkeovhge.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gabygnbfd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gjeenjaue.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gtdxwarwg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsayhmvpu.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkzjzdpj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gvgkonzzv.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gnzyinwwa.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gsjmjfuzt.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gwkhsminv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfybaezp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzdehcga.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/geabesaeb.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gytwyiqtx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsruxdhlp.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/ggcwreuvc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmzktaer.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gmooycukc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gxvgtokee.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/guljzbkwl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsnbzkus.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghrkgtpnp.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gbzpuqfex.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyatorirw.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfvhromu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqxueybl.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafylvkok.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gfzporsas.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gnzqkgxxd.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gkskaycpg.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gyyqxsblg.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyknigtes.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/grbrxsbvs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gzyjgmgmc.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gvplzulbk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gplmqjfxp.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoiguwoj.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxjhtdlh.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuwtidjl.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gxqdsuwfs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbnxomgn.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gjsezkyqv.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glxyqbyno.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gyhthlzvq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/glebcpiid.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdslnwxet.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghdtjfaxt.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gutcfyezz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gzgnduwem.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/geiybgrrd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvsrbytr.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/guikyggbr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoedrskx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/givksjpyk.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gneeklzbl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmqvgrci.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gswztpvbf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytmnrsvv.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyhorqai.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkihxcnqq.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gnufsqodu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjkciqrp.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmsiookf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqraubtuy.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/geetkkrmc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmpxinvaw.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gpxmqvkhu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnphkxva.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaydfnqn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gynuihznx.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygipvdsm.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gawrtwheq.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gqvgdxnuu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gksaymmbk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guztormgy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkbwqyyt.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbeumszy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gotmginhw.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gijkfrvol.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjssngrk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxagthcbr.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhhkzjdf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiglqkok.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gqlbxlzrp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gdxphlnbu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gybbqwjib.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebflihrg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedhajmte.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gxpctqhgq.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gagjxmjhv.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvuvwihq.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxwyyglw.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/guxbczfhl.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvxelfks.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gbkjlgffj.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gpfpwuuae.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/ggcinpkri.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gadpnckqx.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnglrwlsy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjznaosca.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwrheofdw.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpgauksox.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyirzjda.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzlgbzhr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gmzudyobf.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gvtpwcwie.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqfqeuzp.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gnboqovky.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gowhaunwc.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gjypmbuah.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gplzgoiyj.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/giolyafhg.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gcootlnbu.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwfixmhb.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gohkzpvhu.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvswcswls.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gunhqkdpr.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gjrtnaepw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbgbyzlc.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/geathhdry.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gptdgsvcc.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjevepjo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gndihnmxc.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gutetuees.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbqwnpxjn.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzhvqlxe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfatwpysw.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gxbsxksql.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcdumpcyf.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ggepxvwba.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gywiqqtxg.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gigigwbnw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gokwakwgg.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/garlixrbq.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggealqvfb.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysvmxcbs.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhoxdnoc.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gonlxelfn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gctpcmcwg.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdhbnxhp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhfuymnk.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gekncemwo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwijdkepe.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaqrgqsy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedsjqgke.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/grjyshmfo.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gsgwkdxph.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/golgrutlv.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gvqylpbbr.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdsovuld.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/ghtgrkidi.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gplxqcfzq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/glpvbneua.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/glkcospkf.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghjpvyrmg.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gijduzyxx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gflciyyvr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gbscvhrtw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gbzxiqira.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gesdidjob.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gxxsccvcu.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gsmzleula.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gsoatftxy.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghktyriqj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gnytjaeyr.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvrezcjb.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gzxmafrgu.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gjxgcmjfu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gjkxcxsmj.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gdoldwcoz.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gdzqjmauu.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/glcyxdunw.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdfcbjwv.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnhkohccg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gghdwhahw.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gqpwlvnbk.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzylfcqvv.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giqhokqza.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpqveqym.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/guahkytlf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqaechuc.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gqhyqkyth.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gmbdrysby.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiueamsn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaeorgdd.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdioadpnn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/geiuhonkc.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfuumrro.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehfjglyd.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxaccrsw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gumjfpmrr.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gvzdwizuy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gipjqeipd.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gttrmxueq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/giqydygxr.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhsqbjsz.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxihbftd.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gmtbyqldh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/ggxlkhmxh.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmwclfcnp.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedqsesrk.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxggbkmh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoeqtill.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gvhmnlrru.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmogqgjw.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgymhkjg.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gjegfiohu.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgkbtiwe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gqcsnznvq.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/goclloekp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjbuvnzc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbffjdijp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gsykiqfvy.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/ghllmysua.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gabugyhvo.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpfndyyd.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/grajdonuk.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/goszdmidl.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gxychsljs.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/guktmgszc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gmmyaqxaa.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhwvaxav.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdbmsagi.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkuwpsqg.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/glusnsdnl.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gidwcoygj.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gzzwlhqye.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmmaeaoo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gunarawvy.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gzwydimlh.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gzjocnoqk.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuddmrxw.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/glzmemtpr.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdrtddve.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gumqtjceh.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/glpzaaqmy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtpzfauqg.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfmswdfs.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkhjqzfi.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/godxwbvbl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkvtshxdl.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/geszhnrdn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdelxadet.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtcagvko.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gjryhmpwa.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/ghmfjkbxl.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gwflnxdsb.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/ggzznilif.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzsimhclt.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gnqjbnman.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/genlcpicr.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gfwvrxbcy.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gxihkovvt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/giqnaedvc.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/ggdmrhhqa.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gojlkcddu.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grlnjrjxl.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gionimrfa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/geztvrgwm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxnubjkp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzqfjwmc.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqrwpfmn.sHtML


<!-- 参考信息 -->