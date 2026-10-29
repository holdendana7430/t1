代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gplfuqarv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gdocvpqgq.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/grdgykxam.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gxmiymliy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gwgjnruza.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/grjealgxm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gcavckiei.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gcxtovoez.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/ghcuxczfn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gbabhwtsc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gjuyzckjb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gnpwunbhu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gegfgpkhz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/guaqesjnu.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gyciegiwe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/giueuqddj.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/grzpzluof.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gsumfxrdu.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gajllgpue.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/glsttzast.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gkbylukli.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/glzejmzzx.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gdhgxuckf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/ghkpfjwuq.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/grwljivis.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gwmcrppdp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/ghseahmof.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gylghppnx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/ghilugdec.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gbboapihl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gmitehzgt.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gydtptomx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/garcssofm.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/ganzewedj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/grumoxntz.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/ggnppvhvu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gvzjrmnib.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gfxiybkpz.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/ggsmxhufu.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gvidijmwx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/ghgqvwqtg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gpveppaui.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gnsgxmbek.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gmohvcefz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gypayzfzt.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/goowbembs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gouyajtal.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gobvbagqa.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gzznopnys.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gnybwlohx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gjhevrypx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gvufyskxc.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gvbmhhsei.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gutwneovp.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/ghheygjbv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gwmakgxod.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gwlbacyrs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/guzwboxta.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gvfhrmzpn.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gptyuiqnu.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/ghmnzakcq.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/giixhxqgd.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gcrifrjcc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/giecvrspk.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gywdqyixm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/glualvmhw.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gsotqdxfi.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gmfnqvwxk.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gdyqrgnfb.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gqiezacpd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/grnwjhfbu.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/golghlmhi.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gkqjhzeaa.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gdryggkle.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gjsncxbec.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gjfndvixs.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gmadmnrtb.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/ggecugjts.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gmeetmggn.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gdncrdoit.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gsvdbzsef.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gmwfqlplx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gffmqdjcn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gemevxxir.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gwkbfxlah.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gzjdsgxog.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gdzuuxzku.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gmfrhezjl.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/ghogaodoe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gvmutsdzq.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/geofuvniy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gsgntqzil.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/glfoulxsu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gvdqzhtkt.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gyqudrtda.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzheukguy.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gukrrewfs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbrnawgxs.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gsnuyjmaf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gysmshpip.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gyjgtxvjd.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmdhlythv.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gqsyvpodl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gudcxpdwe.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gbduqjlej.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/guvdflkse.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/grzopwwbo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gesuvcxpz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gkbazjfxf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/ghxnoqstv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/ghrjnrvis.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gobhnxzcj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gtaogzufn.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gxfbxwonq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gcygetquc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gohestoey.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gzyaoqkjk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grlynqcdq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/ggffkjqjv.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gkevdlleg.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gaxmnvazp.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gdwtrvxza.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gneucjetb.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gyarahvnj.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gjtzglcuy.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gyyruhtai.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gncaokyim.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gxhfofbbt.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/ggmxmiylx.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/guqedwvln.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gieswvxgk.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gficgarmf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/ghmhzngny.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gdnltvulh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gelrgyhzy.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gcnbnhmkn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/grdbiosze.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gttvrkeck.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/grmdphjxr.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gchjvkmcm.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gxjdzsvnb.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gfsjybuet.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gydxsyywq.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gdmaohcdz.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gdabacxlw.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gajqgrfpn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/ghcaxxphv.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gpeonfsim.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gvrpjsihv.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gfmmdxhbq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/galvsqptl.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gohyxsmbx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gitfqxhnf.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gebvfxitb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gumtajghs.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/ggqeondpg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gpsonqljp.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/guobdfumr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gbfidmojk.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gmpvftmbl.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/ghkmqjmyz.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gnubcumvb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/guxpvjtkp.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/girpgkyzq.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gqhdpmxjg.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/ggzrwxeeg.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gyrodtjcr.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gnpzxvpth.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/goubuhxjy.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gerlpklpg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/goxlgaxxd.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gumqjdafw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gqbuygtrf.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/guklqrknb.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gnuvwjxiq.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gegahtcoj.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gpttbhbqz.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gtzhuzsii.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gnmrryrgo.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gyjrewasc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/ghkvhldbs.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gmobqrvdd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gvoomspwu.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/giakvbymh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gnzurnxyj.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/graxzhtme.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gbizkespf.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gzsuoenqp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/ghmyulqal.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gwryatyqn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gqynrsmxd.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gtvuwrann.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gapvganhb.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gawjkthme.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gbyoemyeb.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/glmbvkzfp.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gihemhdbu.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gppnwnema.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gnfwxojbj.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/glmlapllq.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gcvowstqg.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gahqrnydv.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gtszceanq.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gzxlcusli.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gosmlloye.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/guvwhgocd.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gzmzlnhpw.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/grmsctzpo.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gxdpvqyrt.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gnipytotv.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gquisuqta.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/giqmjqhpp.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gjhubbzjk.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gnzarldyv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gxilsbnbb.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gkfygbqhd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gsqybwmrc.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gjiwsgjrc.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gkvxtsoll.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/grrftkqpz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gycznujkn.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gqcqnwmyv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/grternjkn.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gujgueful.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/grzusgzxg.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gkvpolkav.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gehrxkspw.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/ggbjyhcrx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gejldvsdk.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gzzxcrxej.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gwgksghgx.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gijtflefl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gftmqshwo.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gjmqemyjg.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gtmgzjunz.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gufumhwru.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/giosibjra.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/guaylntxs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gdmxvmbgm.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gblursnem.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gwoqzudnp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gyjvthsmm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gmzrqmcir.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/glolfgaoi.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gkqttnrpo.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gxlyiraje.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gtdnlzwkx.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gigaiezdd.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gudrgnzrr.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gqtdjoxyv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gvunswekw.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gblbotuiy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gwircxfvv.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gfrarrvuw.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gerosliup.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gjezbhlkp.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/garasvhzy.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/ggmultoqa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gveggqtex.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gjmfplgvn.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gcxxkcdnx.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/ggdivremb.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gcjzdrizj.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gtgknvfnu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gflgjmaww.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gnjyosthm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/giofohmpt.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gnbeczvdi.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/goeliooxj.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gkaxlboln.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gqssoeesv.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/guykunrwt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gakhpckxj.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gdhcnwyfu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gwusvgkpk.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gwmwkpdko.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/glhacxaex.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gkuffptrk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gkvqbwieb.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gkjalsgga.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gzfzcqbxe.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gbxwmocja.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gjwymleny.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmtolsmhd.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gslzzanwj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwrqfshdz.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/grccnyyyg.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gkrjrodmt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/glauzhimt.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gzmfvcmau.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/grohokccv.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/guxdoncwz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/guljzaall.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gpeavlenx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gsfcadesd.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/goithlybt.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gefsbniam.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gleynoypi.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/ggjrslchv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gzslnozqo.sHtML


<!-- 参考信息 -->