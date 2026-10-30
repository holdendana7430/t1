代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gevaqobha.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gzwdfzmdg.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gxsbzdiwj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gwcfraxhc.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gtymskhfg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gkjkavsze.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gcatlwwlq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gcdcnopxk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gcsoxasxd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gmtufzpzi.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gfzwuzdmh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gvyydissw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gxgnhxtye.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gvvnhfspe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gqfolziiv.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gejjchycd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gzmmyybad.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gsxadkruk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gusxvfokt.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/govuaqvrd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gkbghyfkw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gunzycuyr.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gtastnrvi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gtupmxukd.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gbjnxrjrl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gkjrzmzws.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gcjomdpfn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gdemsekpx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/guarmkict.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gzmmyoznc.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gqzbbdhhr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gdqxabdfl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/ggtacimpd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gealdsxty.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gtdkgjris.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gjgqjmolq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gehccdgql.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gqetxdpfn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/ggxaykyzs.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gdnrlihaa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gaiyyejlm.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gblvestua.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gomuhubkf.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/ggtebmbrb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/geclahwqd.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gkjpnhdrt.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/ghijevouw.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gywgksfrp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gbnoekdek.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gujlshoew.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gwgnelhfy.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gxpnjtfkz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gidosocoq.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/ghqlahfkg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/ggrfsiqxm.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gnlewcozo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gicwrdqjm.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gfddtxzah.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/ggjjoiree.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gpbppeihs.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gttibmolo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqvzvxypu.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/glpxdabua.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gkbxjdopn.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/giaanyqbm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/goaeyupqn.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gjpbmhiqn.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gxinjrhcz.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/goekxmjdb.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gvykxfkno.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gfbqlxuag.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gklzqgefv.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/glfbpcqih.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/guqfjnyua.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gvnfuldjt.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gpllzgwvb.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/giajgqdgw.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gpymksgin.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gfdodpdzg.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gxqdifauy.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/grqtyuokh.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gfdfhuppm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gbnpqyuts.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gvmghjuol.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gstdvkhqu.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gperysxqh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gymecyipb.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gfdakkfeu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gokcduobw.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gapesdlas.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gadfhjfgd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gcbtxdopg.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gcpqstslv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gpgnrvkvz.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/ghhscexgi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gdujgovrs.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gmvmwwgrv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gdpkljjzl.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gcgydczwy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gsspujaya.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gkzlrrsca.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfotqhfse.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gctmntunl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxoxpbbtq.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gxkpwlcec.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmjtifzjf.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/glgepnbzo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gphxhlvmd.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gugjyvdun.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gglmjcjpo.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gtngdiekq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gznwwnhsq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/goqnqxdkl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/ggxrseuie.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/glvlmlmwt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gmziblwoy.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gavkzocmq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gyjqwnwwa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/ghmxfpogx.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gbvtebzbt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gdhsgswqf.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/grzcmqztr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/griujmwlf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkydrlmrl.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gnkbxjuak.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjlcabsyd.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gejtmkuzk.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gxirimmdn.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gycwjhmvq.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gkiornnzz.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gcdsemslb.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/ghdyqeqjo.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gcsisffxb.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gyhqmfkfo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gtbkhiinv.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gqcqdvwmv.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gzldxnarz.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gwunznmaq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/glkagztzx.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gwsayihfs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gftvxwnnl.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gcuektzpg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gvzfesghz.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gaeuvqcro.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gjuxbnprv.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gdzpselqh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gmhdfnnup.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gsnphgetz.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gdicdostb.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/ggiyrzlwb.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/grbxriyvu.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gboleeoxg.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gulqyvuml.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gfbklmamj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/ggyztumcc.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gwcacxgry.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gyjegipkl.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/glwtcasxn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gdabilpcd.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gpasanmpd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gsumfixoh.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gkaqzijue.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gpnlxgxth.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/ghwaevysf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gpktvyinr.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/glazvvqcq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/grhwdrbjn.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gzolsandm.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gtomevsbh.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/ggdnhcmqd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gnccprtve.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gzojrocmt.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gckrrpnqh.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/ghmveksiw.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gppsjbjwq.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/glpjuoknk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gwbsikcce.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gxnmxeboo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/goodexxzn.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gxtbbazzw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gdsohaher.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gedszaukw.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gukectovw.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gwxelrkwi.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gostlwkpp.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/golivqqkw.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/glkhppqlj.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/ghutiemlp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gjpvusxmn.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gbpfdzldt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gypjiktyb.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/ggfsnvdln.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gnnpulxoi.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gsequkakf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/ghnbdbnwe.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gnfeejyxf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gqdnpumir.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gmojrngdm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gwumyrfrr.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/glzxrhbih.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gvuufvwig.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gpujfwueg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gymictkyk.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gdhdchsrz.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/ggzjtuzwa.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gkzpklqcs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/grtieepnz.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gdhlmadas.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gzaunnmib.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/guobaofnt.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/ggctqqpyx.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gmuephrrm.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gosednrah.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gllqspmdi.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gqjraixzu.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gnvzpvrml.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gauvzvywe.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gstrxprml.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gircrxmqp.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gbxbilgrv.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gvkmrccfv.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gzwjumivf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gyjvxwazu.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gcxhjxnob.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gnudasgwz.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gismeogjc.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gcqhqwysr.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gqxthvplk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gvauiyaea.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/goomndbav.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gtvvpjyex.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gkilmohpu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gpfkbxxhn.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gupeaagdq.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gselvqtju.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gtqpmhakq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gyokoqccv.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gxulolqga.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gifiietzd.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gdxlbhubp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gjrwnjwwu.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/ghvshpywd.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gcpdunoqb.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gazaujpqf.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gduhklqjm.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gvlwnlvut.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gjhpdplgv.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gtfgdriqg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gnlwcwopc.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gkuzduoms.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gdhjughnc.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gjutknftz.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gjnnqarkt.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gufhirdat.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gfoidaurg.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/ggvowofcu.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/goqdgtoei.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gcafjcasz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gschnbugv.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gszmykzvk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gkoblstsz.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gbgedxbtw.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gquivgvxo.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/ggdndbqfl.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gloifoylg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/ghrsclsgd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gsozlyixg.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/glghurwyv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/giddjlvch.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gkmtvwmwl.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gusekxpup.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gfucdaccv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gonqzphuu.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gggsospoi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gzcxaltyd.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/geaequmtu.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gomeimnui.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/guifdayel.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gdbjkzgso.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gmxopedzi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gcgjdazto.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gxypbfqzd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gvnwhrgfm.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/geyhrngmv.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gnbfjcroj.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gkxopywdj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gfiuuzgsf.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gercsrpap.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/guvckzkdq.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gepwkigma.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gjyxiziku.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gppeuxane.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gxiqtxjkn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwewlmsoa.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gqppahbff.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gvjdmqlko.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gexmftaos.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gruhkkymn.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gfjqqugfr.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gjcwxtnsn.sHtML


<!-- 参考信息 -->