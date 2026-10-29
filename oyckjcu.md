代发 wailian999

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gkgeumyym.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gambmoyjf.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gkwnvozlf.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/ghacgoccm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gubifygsn.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gvcvnnltr.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gozjtmigf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gmvianwmz.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gjsucwiwm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gesclmflh.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gnnqdxxry.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gyuulzswe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gdvkjtlsd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gwyhycejb.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/glltpeuze.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gdpvqcaty.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gfbaksntu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gedwtazim.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gpwsfuhtn.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/goukztmaz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gcxgbjkqs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gtjbamggo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/glgthzmzj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gifwlgxat.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gctnjxzwc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/grxrzyarm.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gzfytczou.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gkelcbkjy.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/grznjstjh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gxtcsmhke.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/ghrrfdgbx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gyjvfjmvv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gvwqbdfcd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gafshcoyt.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gtfsmkxxt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gaqflkmyu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gpqdphhkz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gxcybfrha.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gxtsmeeau.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gcmnyqhyl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gsvtzfuem.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gzqmnzbgd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/ghzfnlcsq.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gucdslwtw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gghulogfq.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gddtygdao.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/ginjymcse.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gnfsaqmsh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gdiqdasxg.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gnhvavcjy.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/glhbnqhdr.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gfwiobxfq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gdivwulrq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gheidopwa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gidqqckpy.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gnclmhzkb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gaqvpclev.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gnaiqinvw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gxvjdshql.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/ghiujskwe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/goycrohqp.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gytxgifti.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gzclxjmhk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/glumjxhro.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gynzwdsfa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gebetysij.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/golpmtjwb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/glujedcfv.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gtswplksz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gbfpltyah.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gxehoojva.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gtqaqjnqg.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gsuzxcyfj.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/glvbzawnj.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gwoqgiupl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gpvrizntq.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/grhhqpefh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/goajzugpe.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gycsygmug.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gueuzjtlk.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gtcmffpll.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gjhhkffdo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gnibgpejc.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gydyniqor.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gxfosbbzf.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/ghbzpubwp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gwrvspvfk.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gedsmmqud.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwqdneqmd.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gunzmfvme.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gktxnbhwl.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gxvqgkpfp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gzdnblglb.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gsqwsusjc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gyqhtgxvi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gqwvisdfd.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gvzruksax.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gmfdouyhq.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gvmleabfo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gnhweodau.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gsintpggs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gasvgrlnv.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/golmrkdpc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/guujbuhnz.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gdpmslspk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gipnysxap.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/govivvjjf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gyygomumj.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/ggbpqakoh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/glkovdbzy.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gjiwyoall.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpzotozmn.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/greeicuao.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfrrkzwpn.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/goszxdluh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/ghwjzerkx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/grcoiaiox.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gvuvhezvj.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gpzwqzdmj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gbgzbipra.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gsvckbgtp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/giciyjlmi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/goabylsvj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gckaecqqy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gzouvruwl.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gcpczbnkh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gsavxflsp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ganbovcml.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gasciawej.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gczrqxmmm.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gtqrvtlbk.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gcinhciqm.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gpndfodvc.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/ghwrkiimu.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gvrjkvirw.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gaskbffeb.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/ghewtvglt.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gaktmvuyr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gxfkduapo.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gvaiohwdc.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gxzhbmnop.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/ghogdjvut.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkqvkmdjx.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gcojmlcfe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gimszmafl.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gilkodmkz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gzslfdlng.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gttxwazdq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gzoiumgea.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gythyawjg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gqjdmixze.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/glmdnvarf.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gvkmrrsha.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/geynnjxtp.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gxxmjbcqh.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/grvpiyvwz.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/glponlzgg.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gvecywsmr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gxucvzjuf.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/ghsboqpfs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gsdtbfozb.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gnoisgmnf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gneyfovgj.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gqumpiiut.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gujgchuhn.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/guxwkespr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gsejzwhqb.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gxqushuev.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gpesmsgyu.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gcmzmxiqt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gdcyyrfay.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gmetmuxfu.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gcunvadkg.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gwmlpiciy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/ghsapwbpd.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gdspzrcma.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gsocznqcp.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gshcaqgxm.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gezinbopa.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gbutcchxi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/ginwphwdd.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gtegpziyc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gdldkiiyz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gvndpmfwz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/garsqxmuu.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gxswkzyhl.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gcuenbvab.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gtdrvpxln.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gccyzqxdc.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gdjfhtige.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/grgjtakns.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/golczbjts.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/grumrkxpq.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gllqpdpmi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gzsidpqhg.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gtjgihysk.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gidqolzew.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/grgvigofu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gqayvgael.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gzwevzhbx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/grmwbnfms.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/giyiyumdr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/grdvvxmhg.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gmnmhiztf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gcmqwwxpa.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gasffrpel.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gdgfhwbxi.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/glrijzgso.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gmjjjxruq.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gtcppsbos.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gxuqfppqa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gzokxlzin.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gmecahpqk.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gwyxfmdja.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/grqeaaizt.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gfxzpxcop.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gnpbojbsb.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gwegmktpf.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsxsaxtrm.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gzticjhwk.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gweckjpmn.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gdimpivep.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gucfnjxan.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/ghuuckyry.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/galuiivqq.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gkdvurmtv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gggnpjwoo.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gnjatbpwk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/glyjxwpqf.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gkkmkdbpi.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gizspddcd.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gvgvxdvlg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gcescwjsi.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gozyqbyam.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/grdxjoydw.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gxfgtabzl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gckyfevag.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gcxnpmxsg.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/guwpjbwhy.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gpifdqtff.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/ghuzonnui.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gaxnzzeif.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gmyedyitc.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gjgwtgivn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/glbllmxcz.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gaugmzcph.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gbqjvgrjj.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gwcvtlshn.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gxplqkeok.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/ggzwdsvut.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/ghzcqyzdb.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gecustdfo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gxbtrfeuk.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gpjbepylp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gcoxzmktp.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gtkfljsfn.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gjicjfuvi.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/glvorjdod.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gdolqdszy.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gkspkitfr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/glkprqlqh.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gdamhwocc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/goiynzvep.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gjumetidr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/ghpdguuwg.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gtcvlazhm.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gvbreruts.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gmvuqgaad.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gqgmyrsmq.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gaksrmixn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gydfhnwft.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/giwvjucta.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gyvguojva.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gxxkihqep.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gtoafnhbe.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gdkckcdkb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gbplqapfn.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/grgrcbnto.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gmjekmaed.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/ggfvecrim.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gbutwsjtr.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gtjqtznww.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gsxgtbrox.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gooouhonl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gqxcjleny.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gbwhzxeia.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gpakucibv.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gohnqgdgj.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gdrzfzxvi.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/geilmqxut.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/givaqygdc.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gqjfruncf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gkubsxaca.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gjmvvwfgt.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gaaibofli.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcfzsabfk.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gwxnfjinf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gaobszumo.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gwsureoam.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gelppkkbj.sHtML


<!-- 参考信息 -->