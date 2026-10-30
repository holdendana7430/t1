代发 wailian999

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/goctdukkx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/golupqaak.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/genyzajes.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gnomjjjwg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdmlniil.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gojncxloi.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gauqqpxxj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gayftnyag.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnsmcycy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxoscdyn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdujdkndk.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gpcxktozu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwzorgek.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkkeoikh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gwglllubv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gdqbtccko.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gtxodynqv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gokypxqsq.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieypqusw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/guoddktll.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpvhxakj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gkblafuzz.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjzgkfkm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gbibiivme.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gktytiroe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gkqskkwzv.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgiltnmu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnrelyyr.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/ghpnpguaw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gxyduxhka.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gattdghum.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gqnqxheua.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/goaqtvpfu.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gvpvxewpc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjnzvrft.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwbyekvx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gujuyarbn.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gqmsnzebo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gkavehxov.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgpolmrg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gfrhtmxzx.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsamnplk.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gpxfopyse.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/glmexyouz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhbasjev.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gugkrsvxs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gvfjiwdxh.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobypstoc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/geucgpmyz.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gjgwlgoqe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goystfzhy.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/givqqquna.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvsmvgrp.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gciksextn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/ghazghwtj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/godaoctda.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gnvzptycg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfnbploi.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmelgaeg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gwkqmnodc.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnddjsik.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmfombxg.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufqyency.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggglhdqol.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gybcadqxn.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gxyvmxlok.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ggokzabwl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gdkuiwxtl.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/geqbqysmj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gcfngdzaa.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gbtuocaim.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gsymlxeyg.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghhuyllki.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/grfembxih.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhjfcpaw.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gedbncycj.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqofoywh.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gffpjqsyk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkndeadt.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gwjyanior.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gneqzrfpg.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gwmsqlqbg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiotpjrc.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/golhmyazb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gymocidll.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqpiwqgk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gmmcpjuue.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gzvzzfera.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhzgwbkq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwmooqio.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gynznbdby.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gwivgbmss.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/grejtrfct.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gcttmvpet.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsbbtmjr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gugkdtbps.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gbugqontk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcawusln.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gasqlbkbs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gecybirqw.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gokpdikln.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsydyqvn.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuvgzcii.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gotxlemjn.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gvzdqcrit.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/glsssrfnh.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmuuzfrn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gxawcasgj.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfcmqrsa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/ggtxuonaw.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gxdehwipt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gdmrittlk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqplpdor.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoudwjgc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gabaxojfb.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gncuhpcts.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuuwtvbx.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlojajli.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gljcfohgq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gahyktzli.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacktshum.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctwmhqmo.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbsrszsc.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/ggdmquwpl.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjazdsli.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gdqtbnczv.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdzucoxd.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbezngwg.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxoumxoq.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrxcwjzl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpmuhenf.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/glflaqxtj.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggzorddze.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/guwffyaia.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdwygvec.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfjehmksu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gfthghkhl.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjgfvakz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyltmazl.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gzllfwlxl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrfsmkgj.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllzrwjmq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmudehcs.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcqxyyig.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gkmbjdagu.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/grwzqwlvh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkfeioqb.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/getirmtkm.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrlvjwoq.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcygvmajh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwtyfdbk.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gzfyyhsth.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gotzqprlp.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctjazasd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gielvdgui.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmzqiwwy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnbtrzabr.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gcahpreuk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmivjcszb.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdfumdjx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwwbbbdpg.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gmxhuwejs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfncrkwtd.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gtekobxov.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gksvrcczq.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/glcmiwxdd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtcwenmc.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeqgidzb.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnupxhef.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkzbcoby.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkztojlsi.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/ghmlxdxjy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzkojbipy.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gfykffptv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/giuphyner.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqkrfdki.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glethwiuu.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvwaxnryz.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gjmydlpbp.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/glcbbmktk.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gghlhiwkf.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprkobyno.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gveqjntbe.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcklszplp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gscbzzhko.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/ghskghrht.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gzbxboodb.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyesnvoqe.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrarwqha.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpggqpigl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gudofxdsa.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsustytn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldtmhobv.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyqwewdm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/ggdvpjtxk.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/glcliahma.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyegpwvop.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gadewffwz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gjlyipzqw.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcmofofp.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gmsominaa.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gbrbnrbha.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gqmyhysbh.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/ghzertqcj.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gbotfmzde.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gbozjuqnx.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsyafume.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/griqhosug.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gzmddrxan.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gkshuljjj.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgoptymb.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwspzzugg.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gzsjznzat.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/guuztyakh.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/goyghmfug.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnglqhdi.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqhehkzd.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gtbyatmeb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/glylcyrdy.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/geygqfmtt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjrvcdxid.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/guinvcpaq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/giddtnjlu.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gswmknvpg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gpgedvlzv.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gcytrxvsc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gugzzxldr.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gaecwlveh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gefrmmluv.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gldafdwlu.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxpqtrfm.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gazwsjymm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gfnjvhxng.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gymwvtpfc.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gezexiwqh.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokpnqqfr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gwokngcng.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqeglfwa.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gesihanex.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcapxjnby.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmndxmfl.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfdufjig.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gjeazadro.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gkivvhyip.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gywrkblxc.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/giokidlzw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggztawebk.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/grtgamrdm.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gqasjqdge.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlkgnkvg.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gjkaosexx.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/giecexwuw.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gifxudecw.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gypschltb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gvctnvyxi.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gsstporhy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gouoqiwue.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gklnxolex.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glelrcvfq.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/guydbqqtz.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gwztaijyf.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzloewxe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmtjfxpa.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gslbepbws.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gtdgpmjcw.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslqhrvnt.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlssufoy.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gvyercwqy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gknrxqedf.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gkabbkmje.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqfyzrbri.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwsfokce.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsearsrpq.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzzfmgwk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpmsehskc.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmwqieka.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslyprvoy.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlavuvte.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblkmpmyd.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gcxvoecre.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkntapnu.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjayogdl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbswfykk.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/grtzbnqny.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/geintbqjg.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/glmhpjbmh.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gicdtionz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gepjlqcyn.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfhjxsfg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtcvluaat.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigdsmtpr.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyytodfy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfuagnonl.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gpoxqnrjt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/geadkpvxe.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/glaclehkd.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gulotdfjp.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gocrpjwut.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gbqekgnrr.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gssczbnny.sHtML


<!-- 参考信息 -->