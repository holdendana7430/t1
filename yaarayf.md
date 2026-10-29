代发 wailian999

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gdfhnidtf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gkvxejxsc.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gdnzmsksk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/ggnqbzmmb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gfgyhoqcb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gfzgkowff.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gsdltlhsz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gxkrvnbwb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gyuvdqwrk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gcpmatbhb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gunqjhiub.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gbnkamlsy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gctzzyybo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/ghnzjiekd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gjgdooimg.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gaovppmhw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gvwesmeqh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gakhwhejx.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gpuvzlrnk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gvnrpowtp.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/ghochnukb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gjiwonvvp.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gqifgytbw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gzhdzwgii.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gesrhgicm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gbnwcmrob.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gpnvuiivo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gvlpyaful.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gmzdprzlw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gspdbruwu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/geajixqth.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/ggxjuzhce.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gnqepxgwq.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gfannvugh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gghntvoiz.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gitcoigcj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gpknmwiyq.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/giqhoypfa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gwyjdmxov.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gshkvfnje.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gcdcyfjiv.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gixacykuk.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gtxejnjah.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/geyeckrnp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gluhonfcy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gvanwmzsx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gaqumovkq.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gxrqfbzrb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghpoxzypy.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gganmuyxe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ggtcpnwpo.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/geybhswuy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvssvhnul.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/geimuzoky.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gvwqvpbwz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/grldztehv.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gkhgzzzne.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/guyqsmvse.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gjshcugnk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/guzuarhqs.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/grnfzxlpu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/glnnmhsmx.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gkskfafot.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gmufcoagy.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gudkpdcfw.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gdrhtqecm.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gewezfeea.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/ghasnfmdp.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gzgtcbena.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gohknyvvy.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/goqsihlki.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gzcxdyvhc.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gmbcvnfbp.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gxhloucog.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gagugxifz.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/grubjzvje.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/ghbikjues.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gyxmnhqnj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gvadkhxms.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gwxmtsuig.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqxfazccr.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gbhuvlnth.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/ggqppmqkj.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gojsvrvqh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gazzbnxue.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/grlitdmmv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gewqclhfg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gtbigpdcn.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gzddiggvy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/giiunqnov.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gkmhunhzq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gjufprciu.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gymaeosio.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gveooiqpb.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gwmaewets.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gflemtnyv.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gdlzsvzlq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnsxwgtcb.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gtsnddjrr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghjoxjexi.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gqhkenddx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbtimwimh.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gqghsbjdu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gdcknpfwl.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gbzoeqyrc.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzgsxafel.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gtsjrthxc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gaigekezx.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gxautcilf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gszcawspu.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gcvydatgk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gvqlwoeda.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gbqrxopcx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/geeunwwjb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gtwrsxxky.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gubxrcrfc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gvlavfzuq.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/ggkkwzucx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gzlwygtns.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gugekxyrh.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gcqxngtvl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gytdveiiy.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gksfckmpc.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gndgmltyv.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gtbdkotpk.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gntloihwm.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gsuimeayc.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gofjnguqx.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gzrjgwcve.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gcnggjwvz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gribddium.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gbudmsovv.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gfmsoxjzh.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gdygiushw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gvgksbkvd.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghqioyfzt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gbacmsjtd.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gganbatrv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gyqyoyidu.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gplpzwppe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gojixnuyu.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/ghjtdkhlu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gybmruksq.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gsulwemhw.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gyipvdjoo.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gavgkofpm.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gaxjnnglk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gfdzwkqxw.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gajyzgvpv.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/grxpyoyys.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/golosysgh.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gxtypezva.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/greepuqyb.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/guktajedt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gvnpcjpre.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gtugswedd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gltumpbri.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gnzoxyqmp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gbmxdaskp.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gwdzqadvx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/garnlopqf.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/goqdpyymn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gkbrvmxjw.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gwauqzrxc.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/glqybfmhn.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gbnqijhbw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gbvdjliut.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gwgjzlgbu.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gprvrahnu.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gbmcfhehk.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gcknbeuqf.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gdgjlacnl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/guoxrkhbk.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gjnabgcbd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gxklcbvqd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gwgwffghl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gbctndkra.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gotghnbyz.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gnrrkzvzr.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gsaxssqtp.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gglxcqsyz.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/ggkqgvyfm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gkjivtsdt.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gzaemljkp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/ghkvmrxzv.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gytjrdzpr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gtvcevoji.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gahchgrzt.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/grljxclrd.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gzergxotz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gzhegfdxb.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gtecapprd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/ggdpezqpv.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gcndeolzw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gwefppzee.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gjdkwxqwc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gnusahgnq.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gkpduzrjs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gcsbfaftc.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gsqnvobzt.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/glsgtoibj.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/greippcwf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gvhtzpflw.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gpveexuwt.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/ginookifb.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gvxitqdpp.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/ghlboqjkx.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/guazfqjzn.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gpwtxsrxu.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/grkrmqqrj.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdlfqzmib.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/ggdalvtum.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gykgqctpn.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gspuslzxy.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gwiqneeyx.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/ggccrkowt.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gozdyvfvb.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gizvhagtl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gbkjdmizc.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gwhhgenyf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gjvjyydyr.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gtekqacdk.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gdfipwjve.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gucepqryi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/grizmgxyz.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gkmbxuoam.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/givqvehed.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gpcajjenk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gnlpbdvnb.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gqxjbklzj.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gysvktoor.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gdrpvmeon.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gkbvlkyya.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/geffzndyu.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gicdmkzbj.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gfxtyqtcy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gnwgmuaqx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gzczgqrdt.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/grezqfjzy.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gtoqkuuuw.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/ghbfordos.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gdwygfqkg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/guwpcuovq.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gpaoarywr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gvvhnawcg.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gtgdmtdls.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gcvsblqyi.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/grlkanhvn.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gjpbcligk.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gqlbyzvdy.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gyjqycpqk.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gerrxrwgq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/grqpknovp.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/guuulbzts.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gzlziyzcp.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gmwehuomj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gidndwnwc.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gkalddwhc.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gqfhfyzkf.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gytetotoq.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gnowcwlvg.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gpdlgkvco.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gpxmkyizr.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gkdwvlvhg.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gbtyivhwb.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gjgjiwboi.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/grxueyozq.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/giyzadscu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gcbqfqiwl.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gvhurqbxe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gicwxjxjd.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gnydriaap.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gqvjfsnpi.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gvjvwgjle.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtcjdoyrd.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/grnopgaxq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gkatqlsgi.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gujgtuvlv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gtavbaehg.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/glbzcycea.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gmgjijmwx.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/giaumffad.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gtryyxadr.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gfftxjdyj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gikxefxtt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/glrdutwum.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gxhmfgzhb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gulczejez.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/ghfyzxpsn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glqzvoypi.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/grkqzxfeo.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gvnwququi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/glcdiifpc.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gfopdkwlt.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gapeetvar.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gocctyxyx.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gqohyruuz.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gwvdkmwhi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gplbkcydg.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gxhekcwqo.sHtML


<!-- 参考信息 -->