代发 wailian999

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgfbssmc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gehqppssr.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/ghskluple.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/girryerdb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gqncizrtn.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gxfvbtiug.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/guitqnxun.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gittgjflk.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gghzxuwcc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmkycqmn.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwvnaqxb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gyudyfdzq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulokgcfi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxoakdii.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gfbnecwzv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gmwflchua.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gsfhzpbut.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/glbznhnxu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gawrbmrfo.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gscbdyspb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdjqande.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrsekxpt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gxjcmivit.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbakspfv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gczkbarmr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gbkqzwbwx.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gnneifadz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkekioqbe.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcnnwwcd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwkojvbk.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gzoiiyesq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gybtvgftu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gflsuumsz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqhwzrag.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggnlaiewe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/ggnzdlyhp.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gbqlsdpxc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxcykkcu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gmczfxjnb.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gllyitmps.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdgqsber.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoqmmmjr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gdqwljdes.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcudnmsr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqdepzky.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmsnbzom.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxovxryke.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwquyzwbv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/giujdygnd.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gbpxskqlm.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gskntafyc.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/ghsgzxjbw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrjjyzia.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gmijprhez.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvplbpbzd.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtrgpcvz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtheczmlt.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gqdobllou.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/grczzclfk.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexgjtrxc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveujbxoq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gtkjijqzl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gzasfhfuc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gpgvkyyjt.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoixumof.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gapymjwzu.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmmfkukh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/grrhkxebj.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnuuavxc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwqzirbs.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gcovakpeh.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/ggqghvxfw.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gdxaeexle.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjatpwfi.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblkbbtkz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gfsbjpuzk.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gwicctckf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gcbfntbmr.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpulupre.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gctwcpojp.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gqpgnmvrr.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gmptnrcni.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gnzgouvxs.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyevapue.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwrbecmu.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/giaccmjva.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/grxxkmbgt.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgrgljno.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gamsfdivo.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gqwfrtkph.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/grajepmhp.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gfaokygaf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoyhdrcy.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtchfids.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqebysbvr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/ggddgbsah.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gmqukfcwh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtdhvsuy.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gvjolpzyv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/ggfpktlqc.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/glsyuchih.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxhrpcds.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcnbomjg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkonbldbq.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmetjrgs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glxpzqqxp.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzibdnvrj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrwfjtdr.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gotclhsqs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjxtnzvru.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbohxfvrn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gukctnmoz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvprueam.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxrphqzy.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjpkkwun.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbthjfmr.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/grkfjopds.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhbaxhnw.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gdfdlscaq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gvciyhugo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntizrupd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/ghogykvua.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghjrimylm.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwusuabj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gzktoqwkm.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoyqeaam.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gojztmgrp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gseapnqbv.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gmhxgoblp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gawjisqib.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeblbowh.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjnwenzf.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/ghqxqrzpk.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/grdkahmvh.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gdagcqyfx.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdbygckpu.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gfcaggykj.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/ggkvlmgse.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gvagumqno.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyjlqjbb.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtueihagh.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqyjkjrz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/grbmnmsdc.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcjohvzj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwpfkojz.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhgchwru.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gbbtvzpah.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gglqrmrfq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrijvuce.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gppakakqd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gqasrsthg.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzftdsiqk.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gixdogfsr.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gtdlhqdem.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkxnfpwy.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gnkkeilad.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvxsdewb.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gijvwlyer.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwmpuqkqa.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejvnmkzr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeszzcnn.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/grdycqgpu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/geezawzfx.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlslljlq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsryjqfia.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibggicqu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/guehhmlob.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gftocecya.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gslrkalbe.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkktbxsx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzisyctv.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcubfcpm.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gffzjhkyw.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gpkcjotkf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/grexeaxjs.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiemnenx.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezyryopw.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gxlizzhcs.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkucxcpno.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjvnhzpx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyumzyqcz.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgtjvqgl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjkyxlqh.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxfjvlgv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbhpdujtj.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gmgwngbiw.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gfhjvulvy.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gosekbggc.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gddwggjnk.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gkcyttevk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbisdugwo.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gecsqwbuo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxbopoqqi.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwjewetb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gfpxndpfw.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggsymgqrm.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmmskujt.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxdnmram.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrimtkrh.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gdsrusgxn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaoiwmfz.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvwjmvol.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyjgryqk.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/grkjcyvpv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtepeisns.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gkzfmactq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/glpaqcvmo.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnqjxhnzn.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqaubljo.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/girtsdbyz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gouywigdc.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gyhbwizmk.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gaxhjmsua.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrdlbrgl.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gesjcblfk.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gleozzlti.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvlogdbq.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsnrxzgj.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiipwyqz.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gocvqgftq.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ghxnqaxod.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gsuyrfaxv.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gugpatllw.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkiewuiq.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslinavuz.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbyspbhx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gvclxkbqi.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gofaerybn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gboruzsmp.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gosrhohsa.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gyehqfpmf.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxolbtgeh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gctqigein.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gcifunqmz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/goycnzujw.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gzmmjsomn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicvlgjjj.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/genunfhmm.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcxjrgrzn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gzclaxorg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gvymmgcue.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipwwnpkg.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfnqjatu.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gewprpvha.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gnigsfnrj.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfavhalu.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geihijpdd.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givktrjjb.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemxhmbal.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqnkkhcfr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgmywhiq.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujdgpjjs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtjfqxvp.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gbgnyftzp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpyzqsux.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gmnxzmzfl.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/govnfcgar.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/geizpjemh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjnarxvc.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gvelcfvcx.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gpphhfdlf.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjihnmgd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gdjlakcvq.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgrfejty.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gziynkfdf.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpxllwkw.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwxnqtso.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gctwkmqfn.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidpgueub.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gfiolabty.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcihqkkaj.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdjophqq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzkdlehm.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwqhnhcf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfndclxw.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgetyegy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gullvnkad.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gxfhidzki.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcghkzjqb.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwzekzqqw.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnqayucr.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gsliiqoul.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzlsbqpp.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gsyqqtmqm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gbryxznce.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoxobydl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gzlehbmuu.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrrbwikw.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtinfuvyl.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gxbuxmxyz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdybyynae.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gigjfypke.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzvqzfjx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gppqgpwac.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gqxxhrzjh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkxdygftw.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gbqjwbvan.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhezmrtk.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ghaebqjed.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnujzbcvj.sHtML


<!-- 参考信息 -->