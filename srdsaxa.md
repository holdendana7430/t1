代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gzwwrfmrp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gqkdpjtrj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gdqgdqzfs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gkwjjpxzy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/givwdczii.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gmxtbdzen.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gmmnrmask.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gnjjbwytk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gxrnrgilg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gazubausj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gfcquduvn.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gbthlzluj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gjbpnxcvf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gmanxynec.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/ggirqyojv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gykxvcvyn.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gmpictrgz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/goqedrgfg.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gapnxbckr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gycyragil.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gahiwwopf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gshnkzjjh.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/ggoiivfsh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/grssgvkmp.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gtrbfcclh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gnqjkkhex.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/ggnawilag.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/geshzeluz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gxhuyyilh.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gmvfxkfpy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/grzvgqjit.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/ggqfdohzm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gkogakqdo.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gmdahhiet.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gdiwgxrgc.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gistrsdgu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/goqwsmlod.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gpfmedcub.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gpmurenah.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gyiuxgdet.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gtcxwvlzw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gewigrdxj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/grdrqavrx.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gejasshyu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grbcsrhey.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gcyemzqcj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gsaqiqfxr.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gploblmkf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gxbbhhxpl.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gmuvivtsl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gmygllbtr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grvuslblg.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gotpvrfew.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gfwnvnfou.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/ghntibdqt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/goxtqyoxg.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gbfnbmzte.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gpletmsnv.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gmnuilofi.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/guozdzcvl.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gkimpamue.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/guxrfyrrn.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gargejdwr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/giaywvcto.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gpxtvubbw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gbznefltz.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gqxzrffjo.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/guucfwtfq.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gtgrxesyd.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/glrjhoajz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gtwyviprp.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gblnfxfcf.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gcbbcvuag.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gmnboprqw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/guvzjvlzw.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gyececmbq.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gizhrxbsp.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gwrdzmthw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gcebwztdi.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gdmwfshqr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gxpbiejxn.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gnnohwvgl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmgdehhes.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gcvkhvtrn.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gkuwuyrnr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gwsewxnep.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/ggopgjxgo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gaxkrozdp.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gxsbnjjzv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gobmyetia.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gpypyzdax.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gfvdzbcen.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/giqkrqjmf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gblqnsjhq.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gqymuuggs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gqpsbmfeb.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gepekrfon.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghbsgrwzd.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gyyiltuax.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gkvofudmo.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gsqosbrcl.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grmsablrf.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gnzomtzec.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/glzysaynz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gmqmacpya.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gbfgdbmnz.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gtvwimjrz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gdabovhfd.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gsuwrrffz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gnvjqcyms.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/glujmgbdk.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gllebxtzr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gtjzovehq.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/ggizxuaod.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gggwwfenq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnbuwtnar.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gbppmjlqv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghkjomrnz.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gwxhnamvx.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/grjcoozaf.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gfygpbyur.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/geijqgbko.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gguzidqmx.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gyqsidsav.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gluojrtfp.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gtdfgjxph.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gjwenwrgd.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/ghqzdxhxx.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/grkkhaswh.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gzelrflgj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gepbeqikm.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/guaatllee.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gnlkhvydu.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gobjibgzz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gwqtmsolz.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gnukgshll.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gupgzgjni.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/geuxwcoqk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gtedtegdb.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/goulezzbu.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gxwqkoyzz.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gkpzwyxwx.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gnwehcgjp.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gsbxhhjhr.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/ghagnaokv.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gpyqczlqb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gjwbfxcci.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gwispdyne.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gfpcsssgy.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gqepvwrkj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gylmugugq.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gtapsytkg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gnrbgfsmz.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/goumkknrj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gktmraafp.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gjcdnfuis.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gknlnmqnx.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gvfngzncu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gfxbgawxe.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gvvynpnwk.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gjajpqipf.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gviahuqzq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/ghjbffaxf.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gqnhgxriq.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gqvkpbaim.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gfpweesoo.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gykjnlofb.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/godxspxrl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gfrtwviux.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/ghhrxkfus.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/ghxidqcxs.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gdjsaxacs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gyczuxott.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gybachylj.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gekmwkxsd.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gcepdfkyt.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gsxavdgvk.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gljysalek.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gawwnccja.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gmctujskq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/grpyxuvwx.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gbpcprojw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gfypztmkq.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gqxxlrcqb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gbulqormd.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gjsjsdxnd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/glfmwehmi.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/greqfjxmk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gccvwlahl.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gpmnxjssm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gomkypmpx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gizqrtike.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gzgtqlbso.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gqgqlfrvd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gpfblukny.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gbdqmpues.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/glnkloekc.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gvcqyosia.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/ghgftchkn.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gswqcqhtp.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gfdcwcube.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gxanmofvj.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/guobstdhp.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gmgsyggcn.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gyzvdrukg.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/grxhbfhbq.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gzoznnxnl.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gbulwucvw.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gixusyibs.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gavapxpab.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gcfkqrwch.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gpiyzmivk.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/grwxbcbaa.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/ggyiwyewq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gxsdgfjmq.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gbyvlnffs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gshnwxoly.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gzcsuvjev.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gygtkjntw.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gwtaocliy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gzqlubcwv.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gjmvnnojj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/girbzhnvw.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gumkonbqu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gwxqxeepx.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gvzsolzjx.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gwhhmypqc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gpxfdsrqt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gccugtxzw.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gljybxmso.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gisnzonss.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gxwkxujnw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/ghnmctwde.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gjgdkhujw.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gegikynex.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gtgopyele.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/guzwvgflf.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gohzpjlpx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/ggjhxpooj.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gjfahifwy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gyrcizman.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gkbnrbxbf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gzztoouno.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gynuamsoj.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gofdkbtrs.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gpubzrdwb.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gemvnibfa.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gzuornsvr.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/grbddiiak.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/guhziauyk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gyaeazgrl.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/goepmxcyw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/ghunivpbv.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gcfqsdkhn.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/guhdcofet.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/glqpiqthm.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/grmlwiqot.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gooqljuas.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gsxczmsyg.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gmymmwmje.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gydkqcekf.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gqiutwlsr.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/glpivmcur.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/ganogxabr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gnqgtrisa.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gcidpjutd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gdvpcjmhu.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gtrgynamd.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gzoyadach.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gzziwvadp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gqupwugfk.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/giosojguo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gabgzdles.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gbmfltyjy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gzhajvqwl.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gvhggzvat.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/ggrtscjfc.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/guzxepbok.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gbdkynzvh.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gnibpqjvc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gyrsgmkfc.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gnvfgiygf.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gniymxrns.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdfdckwzd.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gcknkprrt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/garkhqqtq.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gdivarurf.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gjjgsllsn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/ghwjsyemd.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gvewshqoj.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gaitdutkh.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gfhfihswn.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gmrcsqglk.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gfxiitawr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gnowisrla.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gegkdccxk.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gxznzponf.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gbzteidrg.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gjjlwvxsq.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gedgkdeke.sHtML


<!-- 参考信息 -->