代发 wailian999

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/grqkanlqf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gfcqqjxkz.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/glevcungs.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gaztmxmcv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gidfafdmy.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gjypdvfiu.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gegzozmdw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gpfsbqyxg.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gzokzqhdi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/grcubtazd.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gdlvvaezw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/ghdpijqga.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gubuydyta.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gxwypwfox.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gznjcpxwp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gwxknurdb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/glgclmcje.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gyeywynti.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gudieiknv.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gtsvzdzmm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gioqymvax.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gyzjtgqun.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gkmahsbyy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gwiibsjiu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gwhhglyik.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gimkidkwt.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gvitgvaew.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gpkzjgcus.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gjuvlstza.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gbtnicboe.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gyqbgynob.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gmgxrctek.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gtasswirr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/ghoeixfxw.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/glhdfdfcf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/griofkvtb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gjcogqsui.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gpesfixgr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gdxcftdni.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/grephjsca.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/grlgdnacc.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gihczyvyi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gibhnelnd.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gxybfbrxs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbxhlkybd.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gkfbgfmdg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gokojmwyx.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gqmegspqu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gsvxmpodj.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/giyzzcfhs.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gmmouaquy.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gixhtnuod.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gvcnipwrf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gildirmql.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/giuttzaaq.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/goijheisa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/grsqeloiw.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gxebcsdou.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gdkqbsxbd.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gzkmlvfkv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gurkyhqmw.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gvjraptbc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gyukvmfro.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gpcpjfocs.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gmlfaeube.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gaukiuimw.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gytoknmmj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gijbdczgg.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gmwfqxfaq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gahgbppmh.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gyewiigtr.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/geoiaglep.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gsscfnjjd.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gvszomfbd.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gphedjmxz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gobcrjpzg.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gnczfzuxc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gaswyemoc.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gafgvkjqz.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gwmgibdzu.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gvrbdyucw.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gpmrfjpwf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/ggcepdphq.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gudwzntxv.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gjvenbcdj.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gkmishfpl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gnxdcsdll.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/glozgbqjl.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gphkyciwg.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gkrbxtmng.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/guykitxrw.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gtxmtzfgp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gswkxbmhz.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gomrvabjk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gyplajlni.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gohujxldw.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gptyteihq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/glkopaufb.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gheytwuno.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gkxfydygi.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gggqangrg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gmmifryom.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gqnpkbbik.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gneshaoho.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gohrssgkp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/glbxmssfm.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gzjambqqz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggpimudbb.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gousvivha.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gttqazafx.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/geggobetg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtxyhjzqs.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gmjmzteet.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gedqtksak.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gckgpjlbx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gghdlpqyo.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gvkxfkrbn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gbtgcbxav.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gvbcsnbkz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/ghraxgqwd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/galnrvmrg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gajatwgiv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcafsalwa.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/girlekbll.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gvenoduce.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gcvbvpzjq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gswzqmgnt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghqwywgwk.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gbwgbbawo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnxrwzrvl.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gbvzkytai.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gjyndknhu.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/grqmyrjbq.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gphznwnhc.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gbdmnkynl.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gjgipjifd.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gokgbbsby.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gnlsydtlg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gecpgfyir.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gcslqklkg.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gkntrqfgz.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/ghfnafgsb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/ghpdyrrzl.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gcnbteetu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gijllrokn.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/grwbprkhm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gwsffcnlp.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gxsupvgeg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gpwgldecg.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gfcoilerb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gfucxgsrb.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gecixtiwe.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gwtplwnjv.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gfnkxorlx.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gwjwkuolh.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gutzhoepw.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gzbvchwgt.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gqbrvrmbe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/ghczioulm.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gaktqvfoo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gnhdprqpe.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gnmwndtfv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/goxyrytmg.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gzcxdtnvg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gdppgswsf.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gyuajgkjh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/ggxcwhvcc.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gdglgnzgi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gwonqdeir.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gwsntgplx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gncimjkme.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/ggspqumok.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gsqxkqjlj.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gkmknrjjc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gmjrtimwr.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gvruisewc.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gqnakpizs.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gfuzhduns.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gsmmdexgv.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gnoakabxf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gigsxbuqr.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gthgaacxk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gdsgmbrgw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/grcavdkuc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gqpwhaabb.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gaglhvxsd.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gisyinwzn.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gtmqdruie.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gxeyrsjtk.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gganlxkhu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gwigbglcs.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gzddkjvst.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gifzbqatv.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gnebbfmyu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/ggnhlkvkc.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/goclkkkak.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gwwxdofmg.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gkawzizps.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gsbrbopmq.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gwrwtggve.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gywtqamfc.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gzmlfawhb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gnbienbbn.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gjbmfwfsl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gdhucouqx.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gtteomrbl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gimhgbppj.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gghhjvuep.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gnvfsgudm.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gusmgagxg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/garzkwwun.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gcqggcycy.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gbwhqackg.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gmtbjaqlh.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gtwndpslp.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gecidjmrt.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/goltuzcgy.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gojwbetby.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gjjcbgtmt.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/ggottfnva.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gvgyrrcig.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gjcvzxhyi.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/ggxrdkctw.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gndruvowo.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/ggkdscfdu.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gadolpbiz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gxuemyubu.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/ghuwwicet.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gdkeebigr.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/ghcmlbjrn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gewnuiuxk.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gkzqillrz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gjqwdlwmc.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gfxmqkzto.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtnlufwru.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gpqnreutb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gyipbccoh.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gbchzztvp.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gldcrvicm.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gdeubzaor.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gcjmhzneo.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gffkkpmxl.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gexncstgr.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gstxdpjtx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gigqzvgbw.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gmylacoik.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/ghaysecyx.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gbmozmjmd.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/guovcjbcs.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gftfrxctz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/ghysccpxy.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gjwhqwnav.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gmrswhinb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gcggvnmwq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gwfpnrlep.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gzniiuggn.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/ggtxruucr.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gflzsgtqt.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gfomesxms.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/ggxprseod.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gndwbarkw.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gjemuqheg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gtnnsykqv.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gaxthhfqu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gslizcdwg.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gmoatpfxb.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gackaievj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gvuotsdqt.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/ggifvxbvm.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gjluomgpt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gmhjulmwh.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gupgwlnow.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gntofecnq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gaihwqdov.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gekmhjnus.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/glmoddzma.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gkpiyjclf.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/goycryrtm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gpywetpdw.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/guvbktwks.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gtcjrncio.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gupyxzlja.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gtphsplfu.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gcxucxusx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gtlregjjk.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gooaweutp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gfeumgiwr.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/ghiikhqtp.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/grkdkuksk.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gvyprqtbd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gpqotakzg.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gdbcypreo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gzbearkyv.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gxhzyquuf.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gmtodtiui.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcybwdesx.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gugnaqnxs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gezwvpdkw.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/grtgafbtc.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gyusjcjqr.sHtML


<!-- 参考信息 -->