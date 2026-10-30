代发 wailian999

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnkaices.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwhdspcn.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazngnnrb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gpucdhxoi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/guukwtwbp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gildmphvt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gigbfcmui.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/grgdbjted.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjfyfnnx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gducskhwq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpapkpmsb.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfwqcbeu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gkukstoua.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gvryvgbzf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvznxdcrh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/grmpzccmo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnwtdkjy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gptkvbmun.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkrdmjyq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqvsttct.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhxfoqfk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gujmwpece.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gxughsxux.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfjeowpr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gllbudlsk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeiapzpy.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsfyqklp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghufgvzoj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjtnnflo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gwixtxpgk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/ghgstkbgd.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goukqpkkz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcceofuau.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gpnqntmbc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/guzuxeqjh.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/grqjyaumx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvemvimx.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gdzpjuyaz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gecipddya.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gzdozfjdo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspexglmb.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gckdxmlxe.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/ghvohqykk.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/goppavzjp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghujzxitx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyghpsivp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvutoornn.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gwkuytriy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gartdofok.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/ggxotetiv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmgnceos.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtslhjodo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/glyhhoenq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/grabytmlt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/ggdqaqttj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhnrawbu.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwvtuwvq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gubmrlwfz.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxugnpiw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctfzvezz.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjogzoukq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjjnzjcd.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/grbdtqbmf.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gwwbxouyu.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govolrrvx.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeuncxka.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyuwgipz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gmlccrmqa.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbspwzmmo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyghilzjd.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gamvvttbf.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gczubxqsa.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtiqiosf.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gqbqhmpoq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gkffcvywv.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gsweahynk.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxksjmlsx.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/ggedcyqju.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/grmxhbwuz.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwwvljbc.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtjmjommj.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gbdjoyped.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gdkimuvcq.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscrwgjjl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gnksvtvgh.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gexkfxvbw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsiplejn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgoqyznd.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gpevizujy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gojlypptz.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gzbtmuzcf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gvvomopsr.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gezltivro.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipuhclla.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gppezdqvi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gdquiwqew.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gtltppquz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gowootvbn.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdzzisqna.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvbkksco.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glodnbamx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/guqpncmpr.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghzbichmg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvsoaxvq.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gshfbworm.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyokqptph.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/giugyvqag.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqwpgimw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkbjaxav.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsaloujv.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gohtejbhm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnulgqic.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmezcrrez.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gievgfypt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqwdykck.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/graazbwmf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmukkkab.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwroqyhdp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxnuiudh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfzbipuqf.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gqctzqqyc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grnnuonrf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsqwqznc.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/ggouuagag.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gbzkmrdit.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfdpdfyn.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/ggxrialjg.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvcdsfyez.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqswiops.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/ggfdgozrg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcgunzou.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfjfrulk.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjqrtjfx.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyllidtd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbiucxdsl.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmhwxnvwr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gsyhtzgff.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ganbgyzrr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/geoddtaeq.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gqqlwpmeb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gsdaonvwv.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gkxgqznvs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gudidbtht.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/grdqdardi.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdufzsel.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grihmajhp.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmyihxrf.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvgmridz.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gucockyux.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggyrgoxfw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdthwkbjb.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/glbjumenx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gujwfzlql.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/ggawrhhpl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmzvhijui.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/giyeibpav.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnjcegif.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsmjfgow.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gscllxsel.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzokuueh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkixpcsyr.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyqocqyu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/giwkfbgcr.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/govqnbylj.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnvwczxn.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gvzuhhpdm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaisamdx.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/grzlikixa.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gaizuktnl.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/grmybhacc.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gruwentfd.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnfwonhek.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grawvlkfv.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/guugntlqq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkpfmyrqf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gefqsierq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggshoesbu.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/grausgjez.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gxcwbasyg.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gjflainlk.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gkdxfyqip.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gmwvpvgxl.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/grtlcxgjo.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqljrkxqb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgqgimyp.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxmmixrc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldahlsly.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gddiqxljx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrvbomer.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjzwreze.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaynstwdu.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gsabgkqss.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrigyprh.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gaenitczg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/guetqosxb.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gibkmjebb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gnhvgeewx.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlbhgpty.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfjrcwki.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnzumfay.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gmpkxwdll.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gywslkcfr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwlvdohc.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gawzfzwra.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gcypezulo.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gzsexvguk.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpfotbhf.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gchrhbvvg.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gntpwewsu.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/glvkjrccw.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwhbpwho.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxciybrlk.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gowfaqqou.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnyefduh.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/grpdvybhi.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gtnytjbmm.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdvrxouj.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekvjxdpe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gtgaxaszi.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/ghujwjbet.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gisbhkrzu.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gqmqqxnpw.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxrlphodz.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gwdjqmibg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/giurpjbzh.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlluermw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/geuhqrdkm.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvywlubnh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gwmqmvpyn.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gkfdztdzs.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glredwiqs.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/ggtftrrgv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxqvetlu.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydymuuvg.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidbxjkea.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaeixgvc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gwqgogzvy.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grybiarxj.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gghsaewnh.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gewwncyvc.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/ghedwihon.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzlwyelm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gncecwtxn.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gepyvyjzf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/giygdylug.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxkkcttj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gpjkshdbb.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gaylakhbv.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/geqnovapz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqpuyhep.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqprexcpv.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbmzhzie.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gecumalmr.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbvsbkip.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/glrmvcvuj.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlgzerhw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gfjxntbhu.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbrbmktj.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhjpzbvj.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gasnmilzn.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gsmtrkcin.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gtkdfhqzu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjwplgnb.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/guvpkragu.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gawdlnmld.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwcakrwi.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxyiojoe.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gofgocnsb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/geymtgrus.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gglyocjmg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/googepckx.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gchsvqpfm.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylqpsmlv.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdesjwvrv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzllsldbs.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuezwodp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gpxisghsu.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqashrhyq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gotcfqoci.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gmladshge.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtqngngh.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gdocfracp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gchsuedyg.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gsdngeltk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqaynzlsy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwhwckgm.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokrnwxrz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgbtygqj.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpdrstft.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gztlketbt.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijergelx.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gpcodcpvi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/grtnvqcqb.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeavrkcd.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/guljwasip.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcziofxbe.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/giilmiajh.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gyfrlkuze.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrumosvi.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gdiludkwo.sHtML


<!-- 参考信息 -->