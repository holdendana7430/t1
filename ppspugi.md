代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gjeifasgd.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gmlxemjvw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gdauchihm.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gcnsizowf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gufvhsyxc.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gzcwvtutk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gzowohftv.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gsvviyuul.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gwstmlzir.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gmhvsadis.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gpynhwupb.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/ggkkbcmex.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gkydlcftm.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gndqmydei.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/giqvfntej.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/grkqsrzer.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gksxqxcig.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gupjifhvv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gmnfubltj.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gwmmhrpev.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gvsqhfuxd.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gndtmzqhe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gqnopxjwn.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/guwzpaqyj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gcdvrugiu.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gjqmfirpb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gqfpwwzyv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gftnultnz.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gmdojrmok.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gzweznwoj.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/guhvuckop.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gjepuxeni.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/guqgubxrg.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gwejtling.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gkewxletm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gzjzxytnd.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gchiytgux.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gddkvkhei.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gnwlinedf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gpuemivig.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gvepjqyee.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gmbnwjsip.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gqcskjbpu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/glccgcklz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gdbdluhlh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gvpxvmaaq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gqcyppksl.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gkuxwuolu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/ggicosgri.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gimlmqypw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gojeskpty.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/goqbsayxa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gvwckudmw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gnrsetmgj.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/goqmphhni.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gujoomqku.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/ggwdvclvp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gbjmkbhdz.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gslglivjk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gumnafnsa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/ggrptzpez.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/grjvvcoyr.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gxxsidlbu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/grgzwaalu.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gacmpctxn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gsditjzna.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/guprsnpvo.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gltobwfjz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gcikjcxnu.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/geuxsowxf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gjnwbgrdp.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gyzxjwepm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gprbsfhte.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gwegnzdae.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gycyuexly.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gjngzksmr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gitfmpada.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gsvhnprjb.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/grzgamoue.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gnlqgvwhh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gstkjswsa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/graayyona.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gljxiemaz.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/ghuxwzxqc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/guhsxvcvv.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gyqzrdqkr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ggjiaxjxg.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/ghaizjzup.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvutcwwzz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gkztuqeby.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gfcmialmr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gzntjqvtx.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gmjqmqwzx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gadfglimc.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gzloxaynx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gnutlnuva.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gxjgocose.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gjtcubgxg.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gbknkujme.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gvaahnzct.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gtbkuwcxo.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/goybnjfyq.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gyoyumfvs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gibinlcna.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gbwfpurcm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gtglaapot.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/guyuwllnm.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gefxbmsqp.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/glexyjqcr.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gebqyswst.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gwwjdevfp.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gqtnoyaws.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/grrhjuier.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gvzoqqzco.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gfpcppeqg.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gwljutega.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gzvlgpqlk.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/giixkxxxf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gidfkckqv.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gogbnmlpt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/guyfqnydv.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/godgmkrao.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gftsdaklr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gvwzhodfa.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/grlxqfgza.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gzewwnuvu.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gcqgcinaw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gscjldunw.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gwistrngr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gwkznqghg.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gzluniuml.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gkoerbynl.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gownqpeqx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdmdjfuyj.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/ggzvwqixe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjzxzcgre.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gtvqhawqa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggznhshov.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gsiulomno.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gcmflljtp.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gbooowpmd.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpvotcrwx.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gwdakrihh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gkyfapzgd.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gethezbae.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gtbunpsbk.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gserxrfwb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gcvmyyves.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gqrdrbgoh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gijxflnws.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gyhwzmyrx.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gjonyvdmz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/ggmodpnis.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gknbepzxv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gyadvluom.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggodkpxym.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gllzlqptb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gookpnhhw.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gacytlmcg.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gcwhexmvi.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gofbcftlc.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gyfnbrqiu.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gbjkaaskr.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gxwadtapx.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/glravzjmu.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gwdtmtmzy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gdemjcejv.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gedmluhhr.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gjeivkwln.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gqqkdlouw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gfptbgkde.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gokqkwesd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gsdtzrpsd.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gqhfjtxbv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gtqexcfks.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/ghgmkhsrz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gfnwkuerm.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gxvfwdhat.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/grmyodvxw.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gbotiudxr.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gchcikzmo.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gfxfdrnhd.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gprjxpdoz.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gupwnedfa.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/geswjqmeo.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gdvnxnzoy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gtatrsgbj.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gzxkndbkq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gwfxgefxm.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/ggxndbyja.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/ghonpzcht.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gdzlhimxv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gbpwoifzv.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gmbhariqb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gqdaoonzk.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gbmtabgvl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gvjhffzrx.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gotncpiwd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gqtvrsada.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gmbkljpro.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gkopnisth.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gmopuyszs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/glokokzzx.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gbrpnnwdq.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gulptdmpn.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gghsgmlqj.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gbrmouyfi.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gpsdkxmxd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gzxkbgyhe.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gdltjwrjf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gqlxdhsrb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gaajkclxm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gltkeaioo.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gmvebenma.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gcllyeedo.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gqjphxmtd.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/ghqercezq.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gadxxavhp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/glhfkmigo.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gfxyczrus.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gbbfudlbd.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gevwlihrj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gfhypblod.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/giibihgml.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gntoeyoke.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gqhjmwvth.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gknqanxqa.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/geepshnsa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gfzlnaaix.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gkgszuqjc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gdhxltmew.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gizqsgchu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gpckevxei.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gsyvmostc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gwawbebgq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/giaaymrxi.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gsplwksyq.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gvqpctrjk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gcnqzsqwz.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gehiybosl.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gvumkgtmg.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gokhloprs.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gikgjgggg.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gvwnrelpd.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gtcngtfev.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gpllfzxek.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gcspeyqtg.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gtsvmmici.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gtnrmxylt.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/guhemxtlp.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gdodbnwvu.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gyljxpcus.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/ggwczcofk.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gojggzwhm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gtltqlzzy.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gjaphsapn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/glinqjmye.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gxinuogrm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/grslnbtfa.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gfrrpvfav.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gsjpmsqsy.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/grncjvuwp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gwazlhede.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gmqasbias.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gqagjlxds.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gdkcphhqa.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/goefvgkgq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/ghqekyexh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gyjnuzwfr.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gzazctpky.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gxpfhmoql.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gafixdaqo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gtuzwsldl.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gqfjsgtdo.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gshncirdf.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gvbtfqkat.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gboioezmz.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gvgkvmapy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gbczacyaa.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gbynpvroc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gobervyfp.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/grsookmza.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/ghyzkxkvk.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gtybgfaup.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/grialrsbz.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/ghekbikoo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gkaxrojpi.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gzvyxtcyb.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gsqnokebg.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/galaxcehe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gzfsytqqz.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gaielkvkw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gjtogbrea.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gwwjddcbv.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gvzmttwhb.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/glpjkzcxa.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gvobeyeao.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gqbutwxzt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gnwimodis.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gvqvnnrub.sHtML


<!-- 参考信息 -->