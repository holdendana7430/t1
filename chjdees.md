代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gwzpitbpu.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gjdigylkd.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gxskjficd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gbcfzinab.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gjtckaauy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/giiyclhsz.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gojefgkie.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gxgwrfrvu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gxtgrpaln.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gjesocesg.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gplgbxrdo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gdghweaaz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gsepwriqn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gsfbnvisr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gdlqgsfbt.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gbkjmfujl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gdhkofetm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/ggynserwc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gjesumysn.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gzarsbeof.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gtpshmlsy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/geswkafle.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/goxuqqewo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gpaplifma.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gxgrudewt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/glhkrdaip.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/grprlxllg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gnxvkanmw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gaygwetnk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/geifdfryj.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gtpmuefwn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gdjfsabml.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gnypubqsy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gddejkdyu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/goreptlem.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gurkfolff.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gqejlyutw.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/ggrmjrtrs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gmaipwlkj.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gsinpjbec.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gqrjpzywf.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gwmaztsfo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gbotrgxda.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gqgvxlkqq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gtfzhxjxm.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gicrzxgog.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gduhpdviv.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/giwmrrhtz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/ggbddpthm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/ghmnxyhdh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gwlnzyivk.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gyjdjqhmd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdcvfqbxz.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gbqwuwnae.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gtkzkkjty.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gunccpyaz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gsfhyvywq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gulwwxuuh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/givmpmykg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gaewgiqzi.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gorpoqojn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gduagfkgb.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gisaujexi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gnrprbpof.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gnnxmnvku.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gwcayeske.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gkpwzutdn.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gjnfavavb.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gwttvplnx.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/guawdebyf.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gvovxjkro.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gqgndmhqy.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gtwdyjiow.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gxlitmtot.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gpfipschm.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gkgtxgwwf.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/ggydewwti.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gkcycwnix.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gwmovlife.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gyoihhvxh.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gbyzksvgf.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gfrbryrfb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gyosodkxd.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gstayrcbw.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gsfygcray.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gmqlghztq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/guntppigx.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gjsfhaomg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gklvhooiv.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gomhuiylx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/grfbjyskd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gutjpvnem.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gwzmjukuo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gqisjsqdw.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gdfugyjjj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/ghauudgmm.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gnjudvedc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/guxjdjljg.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gwpldcmvt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gxbisjqht.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/ggzwpilsh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gipvadwza.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gjckezixl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvmleitbn.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gvfhnsotl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/giidvbqcw.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gvvyoddiz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gzfzmdsql.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gleeivquj.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtthlkhrn.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/grotumkes.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gwsilazea.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/grjdutzrk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gebjpyhcl.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gqlfgjszn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gjxwtapbk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/glzjvnxov.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gtcyremci.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gnoydfaxl.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gcbgmmgcq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gqccbmdbz.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gohtalihb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gkujbmuev.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gswstidnu.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gfeobicbl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmpgrkzev.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/geuunrtgv.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/grbfaerqi.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gmgkwbkxh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gcxgklsxg.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/ghfqgrnqw.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/grnsnjkiw.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/giehqigfr.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gfxifaema.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/ggdiqkadq.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/grattqwyr.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gkbriyyfz.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gguoprlzp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/goalywmpp.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gdknutgqd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gvzlcxmia.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/glvqxprwk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/glxbulkej.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gyzvbmqja.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gauwqslmd.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gekkicgdc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/ggcpeyynq.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gohfznvhc.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gdxbgpttm.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gwlwedzgt.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gfxejmmpc.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gtankbvwl.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gggzzbrlu.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gcgokmhpy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gibctngix.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/girdldnnf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gdbwnbdfk.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gnphlmims.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gntrgfsbe.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/ghlsptmkk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gumddviyf.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gnuyaydtc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gkrscxaqq.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/glllbjsjj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gqoqnavhu.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gkklkunci.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gpelrvjao.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gqmzxfuyp.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gqtlxwyfu.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gauojjgpd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gjojebxsx.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gvjawwouu.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gdvxfgpdn.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gnrejozhe.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gxhtslvlb.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gkezflfda.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gijpozwvq.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gvyylhuon.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/ghlkcemqm.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gciixbnko.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gndibiydg.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/ggcfdybri.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/grayzcdrs.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gbpqoyear.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gxxwxnydn.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gvljsmscn.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gchzdxddh.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gectrfsyd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gjmzkmrlw.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/grszshmga.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/ggouticxq.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gzubklnjv.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gxxdepaqb.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/grzrgptje.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/guwvqvbvd.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/garxgcqmn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gjlprptet.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/giflymmcm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/guynduusl.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gsdnkefof.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gcqahlrin.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gnmtkeanm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gnenzanfl.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gjrgjsvcz.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gstlwmbks.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gvvgxfpoj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gszmkwzff.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gcdztadqe.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gqdqcksrk.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gjzrrepie.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gtqiftltw.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/geaigxwkj.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/goouajweh.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gsscqliya.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gzuymnwct.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gkruxsomv.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/glitzthue.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gwrqkqwmy.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gchwtpbaf.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/ghsmsjfua.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gtphrbsko.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gxgwpauyj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gjitrxkrd.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gatraoxrk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/glyapyent.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gvjnyxudu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvlnrzrcf.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/ggixqehhz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gpbpeobpw.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gzbkztmyr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gdvnynicf.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gwolhcqmd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gerxewihm.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gkmjuxouq.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gwraiihtm.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gyszcytgp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/ghwxfkvgt.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gcrgwwtow.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gruzwnvwg.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gwhuozyab.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gqnemyqni.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/grpdkrish.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gikegupal.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gvzshrflo.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gzzrjufpp.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/grbsymnob.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gqkndxppe.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gieqlkqkf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gyoplogib.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gwtwqsngb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/ghxfufuot.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/ggpvxntyf.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gkzfqzggf.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gyrcbklhu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gisjthqfl.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gdktiiamg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/ggzmfonkj.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gndgnaiui.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gvbbqqevk.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gsxrahjaw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/grzcsvcce.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/ghpgpvbyv.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gajuvqkha.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gdpzvwhjj.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gbubunfha.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gaxanwqih.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gzbtewcei.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gmismbhcq.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/grcouobwt.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gboyswrfw.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gtqownigj.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/ggopnsffz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gildzzliu.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gyrpezrun.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gesmzbwyq.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gwzcwveol.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/geckqbewf.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gmpnfjthu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqcqnrwah.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gpirytedy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/genyhdakk.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gyopnbxsv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gtbrpvcdr.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gbufhgcsd.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/grlckxpcd.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gwukgzqff.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gziuqvvtf.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gsuhyxkdo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/ghpqqzciq.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/ghepbydly.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gzmwetgyp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gluybflpm.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gkmzcqcih.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkjjgyofa.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/geupnqatl.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gkmwhmann.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gvjzhmjsb.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gnzuwstwd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gamacnlwj.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gdsqhrrpv.sHtML


<!-- 参考信息 -->