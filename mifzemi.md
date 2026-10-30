代发 wailian999

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gcqduwicu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gxhascsei.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gqijgrktg.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gncgqrtlg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gfxdjrcio.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gxhmhmczs.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gwzrujczj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gtpjduyqv.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/ggzkgnitb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gfxyoicin.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gpxlhuavy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gzfotmyvk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gvrntkujg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/ghrmgbnez.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gyxltriie.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/geklqckqo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gsokauxxg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gprdxdgvn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gmyzuiqlu.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gcuebdbmf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/ggkaknccj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gvtnoquoa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gqxowngnm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gxktqsmsg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gtesjyiho.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gkoyureyh.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gvhaglwiu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gbnknlsnf.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/glnjjygyk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gimhlbtov.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/ghetaiydi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gbesenbuf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gcxpserxg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/giyjybkgj.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gwiikawav.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/guajwegue.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/ggohvuzin.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gazlwllng.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gvbytuenq.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gzlvvqitq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/guwipmyiz.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gmxpuuvpg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gspfnwium.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gtyjuxgwv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/ghzudpjxn.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gtmkovclf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gjvxvnukb.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gmrrgwevp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gbdrqirpj.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/ggvudvceg.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gdjmmeuro.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gprsuqmai.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/guswxwlxo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gebiwlrse.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gkjtzhxrs.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gtuqnarur.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmvgaqzeb.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/glzduwkee.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnmnbrrxe.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gpstcqvhs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gnddnckbm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/grnpvjedv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/ggklxemnu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/grastmyyj.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gwxkmnhmy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/goqwkrmgq.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/glqplhdsu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gcargluda.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gtfsqxygj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/ghqczaagc.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gtcyoscim.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gjquknrxd.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/ghafiutow.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gsxvehrhn.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gogzkvcjx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gkzxfuxbb.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gddwvvwgs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gnfhwkobe.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/ghtbuqngs.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gypmzfuma.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gwegywaot.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/ghuitccys.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gidpfdadk.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gdyizzhjh.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gsfdulkus.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gkvwxzjyv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gmghjbrxh.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/ggjhnjebr.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggoojomyz.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gocitobwn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gfgwoliyz.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gqxntnoia.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gdtsodnhs.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gpefrjifp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/ghitwjdzb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gcmywilws.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/ghxtkfhuo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gqtszbmgq.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/glhyobycd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gwtjkxxgr.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gfqmoleru.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gnuduagsa.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gptnefpiu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gxuvgxobd.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gbwkzntcg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gucpuhyfd.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gwvbnnydi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghcuxlwnb.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/glasjlllm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzynszciq.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gaozhrqrx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gpjyeqbyb.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gopqcratk.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjjasklnn.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/glngiqzwa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gjvsckppa.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gxyeadvef.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gmskqjaom.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gxheohssf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gfytxkrgr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gysumrxhq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gkflktjtz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxmbhaczo.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gbwdwtglc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/guyctfehi.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gcjqixflx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/giopigkma.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gebjwtxqp.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gxotzoqap.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxaqbmjon.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/glboxzjkm.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gjpfyehcu.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/grchsrnjx.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gmphgfcua.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/ggnchvctv.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gkidvezyf.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gjiplkkrd.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/ggxujemxr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gaoibweta.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gkudyrbzf.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/grhnazmhe.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gozvqwwqh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gogvqppge.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gcyvgdozk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gpawiezvh.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gucjldgor.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/ggfzdsngo.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gmfsdremu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gxfrzqfxa.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gahbrwbee.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gfkaaufmh.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gjixkfzsi.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gxejwduky.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/ghrrylqss.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gthftbdqh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gjrbewqeo.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gkrlduqia.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gmnhdrtsn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gnisotigx.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gzivgvwgc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gougqsmcd.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gpgnwjpwn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gwxqhvtuz.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gnvtlpbqk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gjhbzxweo.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gplqubzkw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gxiidfqpz.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/galapvgoi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gwxdvtkoo.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gicfevsvg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gzvqwzvye.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gtpxrnzqf.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/grxwjkupu.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/geftqodhh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gafveogjh.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/glkedhjkx.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gfpmgodbj.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gxnqwjkow.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gkbdpgrcy.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/grcitqbkv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gatifcvzp.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gnjxyaboa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/guqwtzeyo.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gfkjulnzw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gcsuqsrex.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gzxkfwvdb.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/genlhoqix.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gyjlqqxzb.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gvnrjqwgu.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/glhxwgvdp.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/glzfeoxgk.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gjhpicfqa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/ghkjfcewg.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/guniflbwm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gwjasgmjn.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gpiuwadfy.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gqisxzivi.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gfeqhlyxg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gpijqfayw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gkecccljn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gkpksmzdg.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gmnunawgy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gjwuatlfw.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/geduwzntw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gsebzhkhm.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gpmdglmsi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gqoesbqfz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gltzpktcp.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gwckhwura.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gplijbxnq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gvfltrgij.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/grxydpcpf.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gfmlnsize.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/ghoxugykb.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gglhsbcac.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gfegwcgzf.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gjuvbifpk.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/glujuldsl.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gyayxpmmv.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/glpkflpey.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/ggyeonace.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gayfeyxog.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gkqbnlnmq.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gwvzsszuv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/grxuytxfb.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gqpiqifvr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gbedgdvfh.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gagilgwed.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gxjsvliyq.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/grkccpxhk.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gjbemkcpq.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gqyhkfwio.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/golirhxur.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gprplapzf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmspqavxb.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gsvytavex.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gbaafueyy.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/grftgpoge.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gkdhomhbc.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gnuszsdjn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gsbnansfr.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gphcxdsiv.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/guuqktnvz.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gtaipyadu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gmvbzzmwm.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/guriihsfr.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gbiabbxur.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gworddxvd.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gptkrjngk.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/ghzaacdrv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gseclpkdi.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gpclikxlb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gntpyejhp.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gadzssjkd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gdzxbyvfp.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gxppuijmk.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/grtwhsecn.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gasgtzblz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gcvmmojdr.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gwiamsaka.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gubdtwrlc.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/ggaqlizva.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gbvnhvvqv.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gnwpxvoja.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gmwzhvprt.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gsquqlago.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gcyohbjid.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/geepxpyyz.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gkfngihgt.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gifnsbona.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gvladexpe.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gfvmklqbz.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gothphghz.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gnkijzjgr.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gtnxupezu.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gsgapwnfl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/guabkjegn.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gqdcqxphi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gjyacyzjb.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gtkoacouj.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gropbapkp.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gxjfhqlfz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gbrrjhwjs.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gvkgyzbua.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gthiwnkng.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gevencfxs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gbeijwcmd.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gewzriies.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gbynsmwrq.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gtjjpvoqc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gkwymgcnl.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gxegtmswj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gzhhodqrm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gkhylerqi.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gywlysjud.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggbpiiqtm.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gagujwqna.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxbocrttu.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gprzhkmjp.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gqxepescl.sHtML


<!-- 参考信息 -->