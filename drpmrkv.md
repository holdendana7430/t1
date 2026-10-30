代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdctedhti.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpntzpbp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmscnuzi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwqmzlav.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxviiotc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gwxtworhy.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gqqxujhkg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gicpetzos.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gtoumejit.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/glfufbxrn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjkmbhat.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gdmwgftyp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxrlkedz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/guqnqfucu.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdbvzige.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmccffhr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggootgbfj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqncmkzv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gusbcqybm.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjsjrcdz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gihgrxjpa.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmfzfemv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitdyujaa.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gspjvnlua.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjdcbvjx.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gnibailjf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gigutyrlz.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gnyczvhqp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gnclfsehz.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/getojttcw.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/girnfrycq.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gapoftgld.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gupelakgx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gpxlujxrn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gwvhgtrnm.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfpsydej.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/geoqzemng.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gotubcdzt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxnpxnen.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/giyeiipds.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvszeliqv.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gqlcxyyae.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfrpamoz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gogwxseak.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/ghmfvytaa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ghvilbsry.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlxttkem.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpebufabk.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/glgzdjefb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gvicbzyzf.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdndkgyds.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gcekcbvln.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmjcbwid.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/glgoxjnjy.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gawozdgbc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/grdikiimv.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxrpvnid.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsffblmu.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gjbsczpxn.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoeydbhs.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvkttduo.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbekhsml.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gshglbnme.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqzgntky.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gldiesbqa.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqtnagbn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gmpyucmdi.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gdfqkeqlv.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhbnnoua.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/geapzyzai.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/grhddevxh.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gtxovubws.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/grpowepnd.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcugewxm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gfvoxjznq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/ggbnlcmye.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/grnhcsstw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gylyatowt.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gjnqphlzt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxgejmqd.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gqndmibwz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gfscowumd.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhasnekq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvdzxrjy.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgevprkr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gteknatfz.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gylcrbcle.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkhjcdyv.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gippewspm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gidshlnol.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbszmxfk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grxtensmv.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/glyuukjrq.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpetkcxnw.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrctxjqt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gursibenq.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzrcttmy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvewykse.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjxgibwp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/grqjqanih.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbkqjaby.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxrmsufe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjhubpzy.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/govnxqwag.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gfdpmulvr.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/ghdxpzbva.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/ghnvjrqcr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfmpirwj.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuhkiffa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkvtbprp.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gkmiepghu.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysevetmt.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gnulsaavl.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gylvfhqyk.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gnmzfcsvs.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmgybbtp.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gddssrmif.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyvdodej.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosdtpanh.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gucdxkfax.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glirjszzv.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegqhrlsu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjtxcalg.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrrecnne.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkhepkep.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gfkmivluf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyntdjtsh.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/ghlraccrz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gwzkkespk.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwkjfyqx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/godvsyyvd.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaulxsta.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcxldmxw.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gaswahowq.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiaxzmrx.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giptmjtwb.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbhuiksp.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswtsxoer.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpirfnget.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/glhhpwjem.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gsofefems.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gtkupkbpf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmnxwelx.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqaqtadaw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gigtxgltg.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gcdkpgaxe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggruxfvgc.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/ggtyxffhq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjszeonsq.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcqmrweb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghmaysryc.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gfresjwll.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggmartukk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsxcynjq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdyiqdlmm.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfdjtamp.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqtozvcty.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbwrquhv.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjnqeukz.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxzbxurb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gouvksdsx.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpxcmprg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrokzgqs.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gqilfrxdn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsvmugqoz.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqjqfbwq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwohxkka.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gyerzejod.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhzhoryj.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gqfytexor.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvdgwxmw.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzlucsvcg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gngyplmam.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlkyxiyw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gopoycovr.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfeamqaa.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaeljbage.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoqlxkwo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptsmgnns.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gqtgzkfrv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gdbgqohab.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gibvgsepl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gwzskjtmv.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpuxxgsc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijaqmwte.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdihkjrl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfcxoqgv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzxzrzgu.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gsabavnqg.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjqtojfn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/ggenlsanq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjmghqrf.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltmhevvl.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/guwgyjxip.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquzroxzp.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gvohlbbrf.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gkzjphipl.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gsuvzvhlj.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gluzupgnl.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gywbbcelw.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gajfkradd.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gjvqonjeb.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ggirrwity.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gpeibywrd.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gojywgtma.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/guzrjuqrh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkhugpni.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpbyqarb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjztljwpy.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/ggukqzsqw.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/getmjaknw.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxgnlsrg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcgmhote.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gnqolruib.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvhfmwhz.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpqjpsfp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gbhrhcoby.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgbkglho.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsyluswor.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuvyzppq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcirgyfd.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaqozlqx.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gekoqxbzc.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gmslxdlll.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzygcakuf.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gsvllcowt.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzbefzbo.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gbvjglldj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glifiyvdo.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/geevvxqiw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gargzncdi.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gxgswfbgr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gutbgycvk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/giffzxpwc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gihovezxl.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gvkyptzkr.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gmjbuntar.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkgnawzj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gqrdefteq.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxfaprdz.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gjctyaphg.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gfgdsmiwh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gscvftvip.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxiaalvn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfhjojjo.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gjynrpooh.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfxgqhnj.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gaisnembs.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzjdlfbi.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrbegeox.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjwftlxru.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxkvuzdc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxmtpnnr.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gngxmeqld.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gdhmhvgpg.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/grhmtfirg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gluqfguta.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoalsozl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcwfhivn.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gzoncaqaw.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gslayiixd.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gdzibxzvx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdymotugm.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvsgyvufy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gafcjbroc.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyedcbzxy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gktqtwymd.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/goaligesh.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gimvrlomy.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gbgbqvuan.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnujlnnzd.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gfifptvzr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/giclrhvvz.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaxmocoj.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gasgesakv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gezltnlzg.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gxobrrkbw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goorypqvb.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grksghodq.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gccrcbpkb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gempxilmb.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/guidhpgnm.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gydttqqvc.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gawaohqtl.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gebftmqjc.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcnferxa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjkjgdkq.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqgwmnak.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsvqafmc.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/giohgpdxy.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gycsrpmbi.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpimljjm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/glhpndfbg.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gufjzzuru.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gldbdstfl.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmpnnlzt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaksytcm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvrgkcbl.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgxyvjaf.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbytygqhq.sHtML


<!-- 参考信息 -->