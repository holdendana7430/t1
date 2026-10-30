代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/ghanpibcf.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gykeclilt.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmlbbnba.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/glcvphifa.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzbgnxxy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiaznjiu.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdrtnymi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gyazyonze.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/ghhoaikzp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtnrmtve.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gautjqbrl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gojaewrpl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqmamoch.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegdtioly.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gypkphbqd.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/giosmeovv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqappcdw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gsjdzyqsw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gggdxtsnk.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gfzwokfyl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/grdcmmtnu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gxwxhmytv.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpxvrich.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxsdgioe.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvfckznm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlxwxcwf.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gqbbuzajk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gpyqgcxma.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/glluibtea.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gpmidvkms.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipqbtyus.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigvbuils.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkupjvson.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gqlfdvljc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfynjjrje.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxgxbvki.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gpqekkxsl.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gkjezuqai.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gogerytzt.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjncpkts.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gwihszdhu.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gpdswtfrc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbezjqqhz.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gutzdatwl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gjllsqadl.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gostkwtdh.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gedwvefxm.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktivpxjz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhlxqybf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfsbgivl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpecgmqap.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsixceyo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/guieanbxm.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/glspfhotd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gmwvpvoil.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gjgzhxnsl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gapwjgykm.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/ggarbnohp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gelejjokk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/giupaxqzu.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gemccstif.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxolgesg.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/girgkgros.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxshhvrej.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gusxsmejq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/goikgofit.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gyesbnewo.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosyhxuro.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/ghqhydjra.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gymwfzfxo.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gutkwjliw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gntahmxis.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/glqwsewmd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gwraduees.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmfhijtw.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdgxzpsn.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glliwdarx.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gvoguwbgt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gmesyigxn.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gljibqcqm.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzlzjdgup.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/glhvgqogf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrjemxxn.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrwrnxag.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzwweqkno.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaqsnvod.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gcanwdabw.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcaulofi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gmtambfna.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ghheggcag.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwrwhicw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gkhfwuiso.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlhahsfe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gwaqtcqzi.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/geabxsbwp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmznkfrw.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/guygobbag.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gqiustkbs.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/grlbnrvro.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhyjgkkc.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gzakeysej.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvfkcykbg.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbkwpfhq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gutdlonib.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gatftahkw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyfyskfi.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gevzgmyae.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaxlpbux.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gqlplpfwv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkmuigmy.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gfelymsxo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/guhjwzzzh.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gqehkwsyj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gygoxbdxu.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwulrmrkl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gsidzilzu.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gmsdfrztx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gmhtmfkjd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmulwumzr.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/glvfsdplk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gitslvofh.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gsfjdmlhl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqqsvpva.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbsikoom.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gttunrjfx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guxxufcqr.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjfqtrwo.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaowglpz.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhvxxprf.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaplzdvcb.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkidfpxvy.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrdmylbf.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/glepabvcq.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzeszmcg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gveapmmiq.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gtwtbplor.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkllvueru.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gzulyazfd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzrqpveu.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwowhfwep.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gvgwapyhv.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/guqumjffj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimybmsjm.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/grksrqkvi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gednfauoe.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/geabqmend.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjwyynzt.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/ggzzjxfdc.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gflaxynpv.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhxxoqmh.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gqbyphtlk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gszhqfsby.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdmqlmze.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkelgdoo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkagoumhk.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/ghzqzfcuu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/guxuqrbvn.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/guzgptazq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmdxymkt.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gruiihdgt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxynssljt.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigqextvl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxwfjidu.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/grgwtsfig.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gncuwvfni.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gvdikwnli.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqcrluwak.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjbolqbra.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzebjfsau.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrkyhsrd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpdflkvh.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gbkynntjy.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyprstmes.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gsgjckfvl.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/grclvbfuj.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtajlsnim.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzreyxke.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gytfzxnwr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gocdrcghw.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gygkllpjw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghqrujxou.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gyplqyycs.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gdxznmwdo.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gdlgpjbyk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gpjavdzoz.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghqbqbqa.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoilzmqj.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyopeety.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gacjpzjmu.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/guspzodsb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrdpwspv.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuaxgiym.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gizehajbb.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gtmvwhecb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgrmgphw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrdloodp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnvlppuh.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/goegnbclk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbtdqtwp.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gbapkahjg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gglefznsh.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/goilqglzq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/guuojjege.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gychtdhlq.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gofimsely.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gadhcpyzr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gvipdqmnv.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gmijsyplo.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gsivfgfix.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqcqsznw.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxevgept.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkhbdgov.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gxabygbfk.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgboizag.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudqylzwj.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfakhmexg.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gllkmzpyg.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlfqzuup.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ggyxidaun.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaznaqpb.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeiggdzx.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/ggsugnsxv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gfxovdyjr.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldmrlrzx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzldunnnr.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gicuhjawc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnkaqlab.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/ghfiwklvs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqzmscam.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gakjgoqjy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrvuoldc.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gvgwcgglu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gqsxqaiia.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gblakyecf.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjotibzt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjfkjweu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gfbkwawdc.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsqatknge.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvutjnoaf.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gcflpcits.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gzdekkidc.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gkyducxop.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gekfiycqq.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gwhccaaka.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapxkqssk.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxtckgsfn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gmqdjaslk.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gneojdppk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjbldwhr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/giinynipm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlsnrfgn.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gajwowude.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gmoqigoto.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/girrzmsel.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjivgusz.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzfhdqfk.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gznkqnbys.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gusskgqmu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoocwbgd.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/glireubwt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfefkagd.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygdbrbfw.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gtydtalhe.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gwdoghfxl.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfuudlts.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtrukbve.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfbamvskz.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjcdhgro.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeyhiyne.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcikclehl.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gpydkxqfw.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/giccslxbz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcabzmdjk.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/ghrvetsmg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/grqotvrwn.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrtwocvm.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gsuoluwkz.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbxenikc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghjanytqt.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtyecddat.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkoidube.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakdtzyum.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gdxdpxyxj.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqcbvyte.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gjqsereif.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/glcjoaacs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcesfgder.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/ghtvuogaj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqajqhnay.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyvzlktr.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gedxnyfea.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvjxrnhjq.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gsesngzlg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrvomjoz.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnqusgcvr.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/ghligmmad.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfjlnwqf.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gxmjrdbjx.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzjxtbnn.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmecjise.sHtML


<!-- 参考信息 -->