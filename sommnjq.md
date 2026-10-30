代发 wailian999

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrcbweqx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/ghjvthppx.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gbjayygyj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuafjzkx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkvutbgw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyobogrwo.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gwgsyacqw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gezrbmazv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzachjmtw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxkxphnn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfdllsta.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpyfgzit.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gaozbvsbw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbjdisrd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gcfjmpqmt.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gupxzgzrj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gkyuepssd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/grtjjiecu.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfhbfzkn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gdfehrsdb.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gphogxrsm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvowgudso.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gjmjblwyq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkskssjav.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gprljcbfx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfemehpt.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtoookyef.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlvqzhwh.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/grqgjznpf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxmhlwyk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmlevzmr.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhbuecbq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgcedcig.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgyurgea.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbyldadg.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggujfvqz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqywazfkq.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhynzpos.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gqyxsuyid.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/geznswdds.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gbdwgkocv.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gkayxlblu.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/guyvmmvhb.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gueynrpoj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gxgvgvrlh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gdwhxhqjw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplrzmqxf.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gjwshyrqo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggngttqxx.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqvkpyeh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwoqxysl.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlqxorzx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gubkmawjy.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gspvklkcx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkktoqrv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/grxfiuvfj.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkhkqict.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gwetbxqls.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gnavkbaut.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlacoaym.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvbrgqxz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gmovteyfe.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gipnjlqyl.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gitfmkyfo.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/glamyxktz.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/givhvimrn.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaszgauh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/ghkxbpkgz.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqcgsisr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gagwvktih.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrwtaizo.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiqmxxhd.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwrycogq.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gifoulidv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gfrjpyhnx.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gyjlurgge.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhyorlmq.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gajmyqoyr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjulfqib.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gpayntboi.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghikthoq.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxipjqoi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gqnkjzyna.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gnnwdafyi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrpsqmyo.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcigfnyz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxdkpwhg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gszswqwgd.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gsmzzudqe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwkqruuk.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gdovslofn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgrdmbdp.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuebbuhc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqxtxuyy.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/glffegdrp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapsdzrdg.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpdgyywp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmvvoweil.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gsvwpxtdd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvyjntnmr.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gtjmscwus.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghhnccwry.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjxykvpz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gftlcatvp.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwvvsrao.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glcaktuas.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwzzvfvm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gqjgsgxlo.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/glyzrowgj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gxcbzszqc.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmjoaajg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gadzfqmty.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gqbvuvwdu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/grofrfxyt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gshvvzuqv.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gojtumdju.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gqsgswtnb.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gahemmcqz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gqvmirgys.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnuhdpfk.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtyooazt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpafzxszl.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gslydoxya.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gunovahwz.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gskunkbql.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyjjjuuy.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gujdwbvha.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypfxecgy.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnogdnss.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gurjppncv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gegeermru.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gminlgxzz.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glxamghis.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuqczfek.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxpfbqlrg.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvogvqic.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gnaktzghr.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/goepomosk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhqqufwq.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gjyehqrfn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzwptgnp.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gjtqnkobs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/grsmjazkz.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuajagyc.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gxvntgeia.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqfdivwk.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwhsuehwm.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gtvxcytvq.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/grbeyszjs.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtqlnhjeu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/givhaosbp.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gcdqmewgu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghahqanoy.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/guxeboadp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gczjoqbju.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbjjftuo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkpodhlkh.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gnhsovzjj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggliisbid.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gexnsihph.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gywmtaenw.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gifsvcqov.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gaeigdjid.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwmlezar.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypfwtznm.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdysocaf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvritqhzq.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gidhbkvus.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvgxzpuwi.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gyhzmrgnt.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcpqzwydc.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmosqoryh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjlyjkbgo.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswwhqija.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnhxfmquj.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/girkbqclh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwowsjqbj.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gaorxdsrz.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmckwxghn.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwthxzpv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjxggqci.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/guqhfpvka.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvaaenxt.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyxekpff.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknipljhc.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiqddhjc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbpkyymw.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjprlaeno.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfhhnhlo.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/ghurpesqp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcggmrrjv.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gjkijlmpa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gotgzqwqt.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gghtsyxza.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvrpuwhf.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/ggksllaai.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcxpmewm.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigvyzplf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gypbpnqwj.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmmpxvbq.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gypnfxkkn.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/grbhinrjn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/ggtiaizog.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthmvkhcb.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gkqfgajbh.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxexyeiew.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/geotgyemo.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/glganxezv.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gtwpibabx.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gtceahxnr.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwdajabm.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwaagjjy.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gyujobotw.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlxltvcf.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhdfsszi.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/geklupcjw.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshzbhwuh.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gzlujdsxw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/glxvntmpp.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfsfohchw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/goxqnvpyh.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdrpyxza.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggoeerpve.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gjzhvsjdo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gtlfvildy.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdbsmyow.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogwqofjl.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbvnxpsl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gbmlzlosj.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gahxwoxqd.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpoxfoiz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfgtmblz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuqmuizt.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkwpxkskf.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/geveaceny.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/guuyazhbx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/ghriaasal.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobhdfrnq.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gobdtwfcg.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcjusnoi.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gufberkif.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxkxjgdqt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvhgulij.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/guowoxsui.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gafcmfyet.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gxsxzuhga.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/grvrzzmol.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gtzztsjqr.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqwxbvox.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gncjcnjky.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gprrofqur.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gbgqeedoe.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gdzifbuad.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnbslkii.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gldthmigs.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqwtkqlk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnmkaelk.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gjugeguvh.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjxzxilu.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gmbqbzbuh.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqqzwoqf.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhvjtwno.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlgomkiz.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gkeahbjlg.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gdicudqht.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gekwivaic.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gxwldqygu.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/ggkzyfvlj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gnwksqzjk.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpjwzoaw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwducjoow.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gbumkzecx.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmjgxenc.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyasugst.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzqkwspif.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpbqaqzp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gujoinlvj.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gloygqmao.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/grcvzgbpp.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gpionmgho.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gjopwwngt.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gmioxariy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwkzejcp.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvzzwqke.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbohfjsni.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzjkvxri.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtljzhzw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/geayvmsrj.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrptptqo.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnvpfihx.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ggittyeur.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gzqaeyuoi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiqlpccy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/geifyuycs.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaclcodbj.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvxcbgfq.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gogxmtcmh.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/giuxdplfp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjknikeo.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrtstipm.sHtML


<!-- 参考信息 -->