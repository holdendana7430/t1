代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/geyalugbw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gantonfpa.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/golshsuzu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzullmyy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gxhppscgo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbtwadgz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltzspsrk.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/ghgefctyo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwmyrmqo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gngjudnhb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwtmenej.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gdwdckwgd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gmbzgxuve.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gabsjlnza.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/guhktzvpt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gycmdqeos.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gqzfqkxqb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjezrzmed.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/giavakyiq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gduylfuyj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcbwuzab.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gqdpcevvn.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gffcolpuj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwonwvyq.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gdhrofxgz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbamzdngh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gozhdybuy.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfzzfzrn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gchexaste.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrqitvfe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/giaaxleea.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/ggdblpdwu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gfxxttokl.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gzmsgqxih.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gcekhxgbx.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/guheibjxv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gzepkizce.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/ghjvjutta.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbxcfddp.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/glhtenkir.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnpqfimm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbzkyckc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtjeppaf.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqzmdnzn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpkxyyys.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gmunkzpev.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxqdyndi.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/glpyfwunf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqspsysw.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/garxsbhxd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhjnghbx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gzksivylo.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/grhazhftr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/glpygozhv.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/grnubnjvx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/geizagwlo.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsfdmoou.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gifgzqkgd.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gzradlzbk.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbexocbwi.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gbitdofiz.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gkviibcnm.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfgbnqoh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/glylnexio.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpyglots.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gkeslzveu.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/guxhxspsj.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gmydmmtiw.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gzzcmozdt.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnybhzxk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmwsuprl.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdlxylfn.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzhqcshvk.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gieojauwr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnwovcod.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnozrnkbe.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfczowwhz.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqrkvhaf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gwfaqdiyn.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gajenuozn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/ggovejawr.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsnglsap.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gifatomdf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gpsnlpkev.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwtranom.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqknzzexv.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gmucowdhz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/guixjkqbk.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzgstfxy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvatxytx.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/glwfynzzn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtrarpwa.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/grremzaij.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwtxphbs.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gljwiciun.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/godbokcaq.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gerjkzacq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbtxxjwiu.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfhqlcuj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbktwhjea.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gevlfrium.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnzxpfprm.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbapzutc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduezipbp.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxnzsjqk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gejdkbxyv.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/glofrmemw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbugyqbsl.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gunsqmefa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyonbagr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyxcwput.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gniynprzq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gncguhssn.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gcorhdjuq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdgaqydh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwbizjpy.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdhyukwg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/geiphqnny.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gitpufywe.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfaameqp.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gowcnqojg.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gjpfmhbyq.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gthzzfeue.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gttwwqeuh.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gplddkoiq.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhuojxpq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatqrdcil.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/giwniwjhh.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyvpixxh.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gynuhgrtb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvewcroua.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gumkifxoz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/geyxgvjek.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gsvyfxtda.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/grudtqgaw.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gudspjjrf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjpvgaqu.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbufwfvh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyrqqanf.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guatopopx.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gcdksioji.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmvuhoxt.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gsadcaabt.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gaybvqpcc.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gifolvwju.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gicognjfr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtcmpcjkw.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gfwedxkeh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gybmgpauv.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/glurqpbab.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtmkkmraz.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjbayzvc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybuqmjzp.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqysteye.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscjsvrzh.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gpknxsebc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvgtsstg.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibbmixbd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqsrxrjhg.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfzreftn.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquyfckga.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziwboizu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwrnrtat.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnsboazg.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzglcyzuq.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gymyghptu.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/ginsvlybd.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/guncviooc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gijuicaeu.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gytwyxuyl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gybquxyiu.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gogjvhdmp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyfawlzi.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glbccdcvs.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrwrpgfk.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gvwdtwjcz.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtchmujsb.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gbdscxoyk.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gisvqkfel.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaybwnwo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmwgqbhf.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjflpirxk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvkikvgu.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwefzbiia.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/glorafrvb.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiwagkrp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvpudxic.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/grandrrha.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcvadzmh.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/giajoseqc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/ggtjbiunq.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/glqzquewp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/grpklyyww.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuwqyofz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gbayrwuoa.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmsyhtpbs.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/grcwunvdv.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimowygwb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/grgxzlhoo.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlualylt.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gnicfkytm.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gqohfgkir.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gvfyxivsa.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gnpkamayv.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gzpscyzae.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedqyexcx.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsxagjhir.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/geycepwca.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gdunxmvcs.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszqtznso.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gdkipdccb.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzzgmgou.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gitnmtswq.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gucurveux.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtjnvyyg.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/guothtlnl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gulafxdvw.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbhfxwob.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxawkgsg.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofqwjelc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gosqnmvts.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/guwmjxcyb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmaobyxvv.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdvawcsg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gysvpzgsu.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsntqklw.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqjwxoega.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsajoiau.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoibozux.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gidtqsnwj.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grubhvloh.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/goazpdidm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcoigwxp.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gjmukcbyn.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuderrzo.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gippfxkuq.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuhdweat.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeifiupw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gozuzljjt.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gcesuziwo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gaelfharq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccmqsgsy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowigwczn.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gdomjxras.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gnonkqmai.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gigkxjbuq.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gyhjymhcw.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblqzlzxu.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsncbvlx.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwsdowhg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvysdvsjf.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyrgqkta.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdkfqpxt.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/golouynsu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzajzkmcq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmpquzdt.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhoqmnhr.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gohhokhbx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gugqwtpcd.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmasdrqty.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbrnnuds.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmvciglp.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaceytqc.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gtchdrzqe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsywmtbla.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcbmiaaw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghvcoixcd.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfkjyigx.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnpywizz.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzgdwdgm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfwqqkzy.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkryvzfic.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gzxznajbb.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvygczrtb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gtghdyyrq.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/glwjbacud.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowwnbbcg.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gzwsqxdhj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjovvddel.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtjtmlhu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqseslhj.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gqgjylvbb.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gctxkwzdm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gckxeljqx.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gyuoodsuk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsydxhqlz.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/grocjugzq.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gfntcqfdo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gghhyadvi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gedbpqjyw.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvahisqx.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/ghzueevqx.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gpwygpfyq.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gdtsgzicb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryzqtzyo.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgsmotfp.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfteowicg.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvhspvab.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwntsqvx.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtztvibrg.sHtML


<!-- 参考信息 -->