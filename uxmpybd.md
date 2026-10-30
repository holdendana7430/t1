代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gfxdksuja.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gxrzsmurr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxswgtdp.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gccloiqgl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflbddery.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiiqsbcq.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklfpbwpb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gulhbzytf.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gjevvvqll.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkbloxus.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gbqqfmzhb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gyyfbzeka.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gtxqaxfnp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gsxzenksg.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqsfqbqz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gwrbgnebk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gvtjesiij.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/godxhjdgs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gnbroqjtm.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwlhrhhs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gzcawezdx.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhgbyarj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gcyeqgxzj.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gojfemzvm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghivdhgov.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gumrcfnde.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/giocnhfqi.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gpicntaaq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gxhgabqzu.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gunicujep.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gyftwimcf.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcibivits.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/goomdlwry.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gkyouunpr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gubfkefjn.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gzyatjuqt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfzzkfvop.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklzzblrt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/grcpmnvvt.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gjmjyxrsa.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbavcxgr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gadvvpujv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gucorioxy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfnyechc.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbbvogba.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gnbeumzoj.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowfzlwet.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgcbuzwl.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gedbcsubj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gatuznxgd.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gcugafwps.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gsoygnusz.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gshsuzyze.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxihpasnv.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmojzvfu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxdmnfbn.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxcksgch.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gzfbsssul.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzbbbgtq.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gumtaxxhb.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwymueuyr.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxngoimb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gfnezzlxn.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gisrlkvuo.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnkvbckws.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gwjbsvfrx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqotmoiv.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/guppfovxq.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsgdqzoe.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gecqdekea.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gdkrnrhel.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/grymjxare.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxevtbscm.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzsrqrzm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqdfjubq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeojnest.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gfovdsijt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsjwciys.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gjtqwjbze.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/grzhrxudc.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gsegihirq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/ghnaehpwm.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gizpgtvtf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gbmrdtzea.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gncfohbhr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbuigybe.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gybovgvrt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjgyiwetc.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gwjuzubgr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbeplqwht.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gafroxhey.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjpswjkzb.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvtphwvz.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlapgobf.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gbddkbnfd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtddxxyj.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gvrhkgwba.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/guplvibtf.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzolczgi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnrlndnf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyswbbfpt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gykirxwpa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gffwodfxn.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gtqgzfaho.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceiilxml.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gdjldxfbw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcztmdszt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glfexojru.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltvwlodi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grnyllboj.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdddiynz.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/ggzojkpge.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/glexgrums.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmgbvwmn.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrnszesj.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtfvsifo.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gnjnucnrb.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gpyhhlvwq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gahnfspag.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxrgoqda.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdssnmvxr.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gkboixwbc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gokbqfkdh.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcfcbmyly.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/glsbppozh.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghuwolsgt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnxovvit.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/grysjlzkc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/givxsfwqa.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyshulaq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gmbgzabca.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gkocdadvi.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmysddbr.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbygqcib.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtuimzvt.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gxioufsmz.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gawjckyst.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gilpbbvzg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gezvgfupe.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfjsiyte.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/geqslocer.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gujmgtjmc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixbxqpyw.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/govtxfoyx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjpmkkbi.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmlknbnq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/golmrdryj.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaozjhnv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzooapqyk.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gblsvsuae.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgxayaja.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gziqgbwmw.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gylvibtbw.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gjvqpjyfs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjmpxnuta.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/guxjpxrmq.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gujdivchp.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gatyrjmqr.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkjxrulk.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grvxdjork.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmrdepcg.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gjrkrbnne.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrobsepn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjikbsruf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geskegmrz.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfbavrvib.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbxznzhd.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gokzwrqxi.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/goqehbbas.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gqwjwfrik.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gxymclgyr.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaebmxddl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvmkwfhcn.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gmbnzehof.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeuzxtdf.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gagtkybzo.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gshqkyvjj.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxxhobuy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqxdyjxyg.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gzbofjrea.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/guesmvkza.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfplbymy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/graugclle.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtjjerei.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcsixokz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/glbjfghqe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/geeqkzgyw.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gznloksiy.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibxuzuaa.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/goardliby.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyeblkyt.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gulaqqbvk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpzksqnn.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gnjfaqxgf.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gcdgvyyjp.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/grcwxgmvt.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gqrtgziit.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjunyqby.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gharuwzfk.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxsbmoxfj.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxfwzjbp.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyicmekb.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkqbxcqh.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gqgqhebhp.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gotaylvuw.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gjizlnlkn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/glrbkyesi.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjffragt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvjmgkkbp.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgyzgrhj.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjekfvhas.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbhjjuim.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gybtguomh.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdabqihmb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcniinwof.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsorgyei.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gunvocygv.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gytzyxfdg.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtaovdtft.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gjviunzpi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gijxllsjn.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmmsyfce.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxynlqfsj.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gffnveyia.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/ggpewjqvk.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnsmteis.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjgaiyxv.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gaozlefhx.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gftkvdxxy.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geontpedk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gyxebqmej.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/ggzgwbxqm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gundspabu.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gdlsjzggf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gfdvrfuru.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkkoawne.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbwqwvtt.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxalgffc.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfqyjjrb.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gatfphort.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gfvnpdwpy.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqoghduz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcvqzzrt.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmowpwyo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gnutjluxh.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/goxgomiaf.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gkvucyxke.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/goykwtwjb.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdilqtpr.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlxvrvel.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/glfehgnlf.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzuhsyuc.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gzqzukmao.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gzhtjypge.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gidcizjjs.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gltzxultg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcllojiae.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gmfxxmhvm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfmqxuleo.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/glpkylzwe.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeqxtrhe.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgbtkrwx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjowaqdfc.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmfcgkbo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtgqucbi.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmimbfqpa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gkkzjvlsh.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gcatjimru.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaxzrzep.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gwraughaq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gemfwwore.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gzslyrpeg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccdosryb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjdsvzjo.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gfpyuigey.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxkdqeicg.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyqhvnhg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvcxutaar.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gegtgknqc.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtqptpcf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gckmmurwy.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasuhxrdu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkasphohu.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiwzyqkn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmromtpyp.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeiffcvy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gymkdecjh.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjmugevp.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gfctbrrva.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gewaolevz.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/glxefrxwn.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiuxwfan.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlsiwsgl.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gxqpcpgev.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwwvlxlz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyokufaf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gwuqmkmtu.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givyuomun.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrrhenlx.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gymjcqzxd.sHtML


<!-- 参考信息 -->