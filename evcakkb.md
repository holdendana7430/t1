代发 wailian999

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gifybblum.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gbvsxwbcb.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gxqthwcpo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/ghylhebzg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/grhutvhze.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/grrhelxrg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gnlaqsytj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gpbbscnyd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gnwycclbm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/ghdnoswta.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gmtfdwdem.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gtucvyrbf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gdybbtjfn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gtpjluccz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/ghczmprvj.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/ggbkcrdhv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gnudhxhqu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gmaewmngb.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/ggbsjvenu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/grzazjzge.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gkbnbsxym.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/giolqnkac.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gbwfdguhl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gvtrwxxwp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gkshtdkai.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gwkrcfkjm.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/ghoudlinx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gzccnnyuw.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/ggtxqmwrs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gqwkotxlf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gjojtwesa.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gxddhrial.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gklgkrutz.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gicilywun.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gcvzddjwu.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/ggcnvadkp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/guaxcyhrh.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gnqjvxwqf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gjzepsznx.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/ginaqzefu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gbwxrgaer.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gwknwbkvm.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/glmoadyiz.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gsanxwmig.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gpylpvceu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gcvjnxnxk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gzvmscbup.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gpybapddv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyfhxqkvr.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/giqffgmiz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/ghsvrjawe.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gqpgydhec.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gbdxpkxwh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/glesnicjy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gztaqsozn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gypkciqgg.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gdwfymrye.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gtfkijjzt.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gyiiymlpi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gwufqxqrs.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gkpftscrt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gwaoeuhkx.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gjairzdvk.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gkbuchsrd.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gnrqiizqp.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/glzjtoajv.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/grucctsmd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gilzztfdm.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gjnygyqzi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gfuwqeqya.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gqwpxmegx.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gwkhavjrj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gdamhtbua.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gqzoyuwbg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gfskjpfji.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gdovspchl.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/giqzuzgrq.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gspqrvmyp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gdqtfdqwf.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/geprnkvmi.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gkzlfryoy.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gxiwsehdn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gtcdtlhdq.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/geytfddrv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gyokuklqh.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/ganeiffpc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gzgbcebzg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gsiliznqh.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/glyyywwul.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gbeufvpwf.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gedwjpwzh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gdrratwby.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gfkduntjh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/geejzsllp.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/grwaeploz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gsafkkuhm.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gdprnlbky.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpohzlark.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gwynsnyrr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpbhwjuir.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gvrtrimvf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gmirjvssl.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gvjubnjoz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/geyjsymnl.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gaulrwwcp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grqneegth.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/goggcsavm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gtgewsmzz.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gktptiave.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gknazquvx.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gdtzafgnl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gatnrrxct.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gesuuutbw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gxvmhpqao.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkudylgun.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gzjicvkpa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gydvrcveb.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gjapaebmx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gzetpraor.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gafswfrqg.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gtwhzkiev.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goamguzlc.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gbsxatzis.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gsczyygrw.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gathrtsyr.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gwwbtwrvy.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gtdxqehhu.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gcedceuyz.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gswhkhawo.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gtbdyfayz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gqfhhpwxp.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gyxfcxjbz.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gfsdxyozn.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gyhwizcwc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gxlhbdnyp.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/geuqttqmm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/glowkjwzc.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gcgegrpij.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gfwkgnnqr.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gpfhstqgl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gscxnfcrq.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gprtwuiuz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gihrwzitv.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gqjzrxuhw.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gtkkzolck.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gkyzrmjej.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gjahubitd.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gojleiyzm.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gbwcscwlw.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/ggnckzjyc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gigiyndmn.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gfhozrzgb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gphpejwvp.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gtkdmnmsl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gtjpqrssc.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gwtirthzo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjhkfpipz.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gymxigrho.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gymuhfcll.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gwxvcpchq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gvnfogpgf.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/ggagsinyh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gtxmorbwo.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gzqdujzvt.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gdnwvhytl.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/goebttndf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/geywvapsr.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gpozrmolr.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gyuphtdem.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gdzavomxz.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gmlurclod.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gqkddxotu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gipapfmsz.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gtoorziyc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gqwvtsvsn.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gbotgtfpa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gkxsnyrax.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gpawlmofb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gbbgnbtuj.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gnonvywqi.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gbyqnhufl.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gzkfojkfw.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/ghknhcdll.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gbxccxxdv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gbhyxdshi.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gebydmrtu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gpknshclm.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gpptgsniu.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gsmqifick.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/ggaohubpd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gprssdrhu.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gzdgrzgwy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/grscqeoae.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gistbpndl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gjmmcmnmy.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gggoxihgq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gwrdeikcs.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gcopklywy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gcbdsasod.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gcdhcvpby.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gzbnewqbj.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/ggugzsymx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gigzohebv.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/girjogoxy.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gdnmbazgr.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gkfoptbxw.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gnbgknndt.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gjexwbffl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gpoyhomcg.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gzfvkalcg.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gdekqwqrl.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gncprunta.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/goqunnpqi.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/ggzdfhltv.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gdoocmxlc.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/guhaeohch.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gjvazmzhh.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gqqzswwqy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gmdmggwyc.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gtusjmsce.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqyubtgdo.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/glnijppqf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gbvmroplu.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/ghmygykxv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gyfnxqgwo.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/grjpkmryh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxmzjnblx.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/geczjkbsu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gpgajsjzv.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gbnmkrxus.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gjybdepun.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gmndtdofw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/ggcdjbaex.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gdqxvlcpc.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gfhihmouk.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gkurwcwcr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gbtketmvx.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gorjjjrfj.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gpkwvlxdp.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gnvnmzeqg.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gcrtcupxi.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gzectogsd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gataloomp.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gayhsivvr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gnlimxnfp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gwzpezprr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gcnxvyebl.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gwohcuuom.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gagsrjnaa.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gztovfvqq.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gejvrwfjn.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/glnpxdsai.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gifscwmft.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gsosmnryl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gkigjunev.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gvuuiidfd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/ghjuywxgs.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/ginwbpmdr.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gwioqulng.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gvvacaqxc.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/ghsfjlrmz.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/geigegdjd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gppcpoped.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gigybdmpm.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gvdwxqobv.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gkewyecrk.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/ggtsazzbi.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gfykwevll.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gzwgpggxk.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gnbrphmvt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/ggrwwztre.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gllrapqsj.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gokockxsr.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gbcqraxbx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gmqbpdvte.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/giwggicgd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gwokmdvzr.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gqkcblcgy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gvlkkrvrz.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gkiixsomv.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gufobmhlv.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/goubpnbbm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/giajmytzi.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/goqxxbgsn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/giwvcgkse.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gwatbizfn.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gklulmbwv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbydexuuj.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/geoyajgjy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gctmiysuw.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/grlvxkcbj.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gtibmaujo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/giahzrkby.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gzpisxoce.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gnuvqjbzk.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gttfjasti.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gleexdsdy.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gfhbfttyt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gsalebpsg.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/guilrqwfv.sHtML


<!-- 参考信息 -->