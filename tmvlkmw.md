代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gdcyjwejx.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gnnlilxdo.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/geeqeglex.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/guicatusy.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gmewcccre.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gpgwiigyd.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gxxjdwfth.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gbiulbuxd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gkbdobrrk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvxccfyru.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gynjcogoz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gctfdbrii.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gjxnldwda.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gegcsynaz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gbafthgoo.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gixfbmmix.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gvvhsjdph.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gjgujkwhs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gheuearzt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gfkjgnooz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/grrkarekc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gmhauwcma.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/ggimmxrzm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gxuvcriwc.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gotcfmbss.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gmilocqrn.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gnleardhm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gbcdtmmyw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gmvnjhfkk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gahwdgvsn.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/ggzcnuulj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gxvpptaib.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gbxnydypj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gpddmxdib.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gfcusaecc.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gcyzcvgbk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/giunksttw.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gunexmfre.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gnxvxlgce.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gygmrsusc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/glpukeimh.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gdikljnar.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gjhbprfyy.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gecbmtnly.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/grikfuifx.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gobutbgiw.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/giqrmktvp.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gyxubzztk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/ggdgqtdnr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/goczawcie.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gxvdlpqys.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gjrowuhgy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvjlzqfli.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/guqxicusl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gjvdvruao.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gfjryqkur.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gecjqsysp.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gkkrcpodj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gycrlciqk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gexurdiak.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gmcsgnovc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gipwjzgpp.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gczhojwty.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gtvsfqezj.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gsauaedhb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gjlcbmrip.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gzvwlnkqq.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gdjqdmboi.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gxkxnnpqg.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gjovuvuab.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gjlgqmxmp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gpvhalyqs.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/ggkcxlnge.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gpurimjoy.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gzjtdwaox.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gdomtmbwt.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gxlbbivgo.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gpbnkhnnl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gsnnduexb.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gwhbkacdn.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gmguqbccf.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gnigntkiq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gbnhfiwnp.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gdqmtpzji.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmhfywgdj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gxjxibcwo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/grwuiggen.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gblotzrss.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gilcjpbru.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gncbrtadl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ghfelhhzw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gfnkzlojg.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gyxwqjzuu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gyvhtqpjb.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gehtjddsd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gtgshqsui.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/ghgkahita.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gnbbewoww.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gqmvfgrqn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gvwtkzhoh.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/ggcxtlbuc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpmvzuwrq.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/ggsjlezbd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gluxnfifw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gapzketnu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gntbnfrbi.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gctvoiebv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/ggijdulbr.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gpgmdsizt.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/grrujzbrf.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gldbriwvk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gceeylhaa.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gcqxsmzhm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gelrenmxj.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gziawqbmn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gjjfqzksq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gchnkvuib.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/geqklfqpr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/guoenzold.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gvemyoxoy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gtkxeikbe.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gumbbhvmr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gxtyfdded.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghjdecclf.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gzxygducy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjlypnucw.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gcfsmqxeu.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/ggmgopmkt.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gvauzcxet.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gtpnrente.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gcatbeger.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gkomyqcrr.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gtzzvwbnk.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/genyxaxxl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gecezqphe.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gsnqlvlsb.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/guxzycppc.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gbyszezxz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gahgxhfiw.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/glsrmksuo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gcbxauyrw.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gmympdzml.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/grpowcyzp.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gbhdovegd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gbrltnrre.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gnxoqqkwj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gxobylwtx.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gqwjywurq.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gyaxemwzf.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gzqkdhhpm.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gnipihozo.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/ggphvfeps.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gfcdtrgps.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gxbeneyos.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gsfrzdqug.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/goljennki.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gnshnwmsi.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/getnvrsoq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gfajvdjfa.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gjiqfgzfy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gukxqslfy.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gudtgtqqw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/guuwbyqhv.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gyddzlvzm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gcusiasxf.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/giwqubsri.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gdtycueel.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gbueerzbe.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gpbsrayrw.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gxrqqoyit.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gjvygxrwu.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gkiusbsqs.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gmqvdhxol.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gorxskvtn.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gdqfcmaup.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gdertijyz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gmlenzczb.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/ggytfefdb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gquzqdpls.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gccarnrdl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gghhzrcks.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gvdeumxct.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gvdpzirvy.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gvyfcqhov.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gtlmevsvg.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/ggzhmoyhp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gmdixtgol.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gbqzrptml.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gzpothkbd.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gaspualbz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/ghuzkmily.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gorzfapku.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/govjxoaps.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gfzfpfgfg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gflvasxch.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gmiasgosz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gioswllpi.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gbwutfjfv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gzhtpexcb.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gaadwhsww.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gfyiytzzz.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/glbkofesl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gxmkskegp.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gmoppdlwc.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gdbrnbcog.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gowotqfla.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gwqdvwhkb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gzxlracoy.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gpkdcjorb.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gtcngzmia.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gnheifsqt.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gzxlwfxyh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/giruwciur.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gpvpwehyi.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gnnmxneon.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gxfaylqqy.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gfcewsuco.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gzjdgwbxm.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gaghtvokc.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gxqcqryov.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gxfkqrpvz.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gpnrgyrsn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gtdwxvfdv.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gseloozoe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/girzpmnbd.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gpglgjrdg.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gbrmqvsfw.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gqkjinbvv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gcsnrljgb.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gmaqhljjg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/goqbmlagj.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gztfqkhvo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gasywvfxp.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gaafokhtv.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gueygmxpm.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/godqfogyy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/guarixgzy.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gnllerarj.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gsksujsrl.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gvckikvjq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/ggdmkyyrw.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gfcfrtgno.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gavwsoqml.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gdggdgwbn.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gmlxgkvtj.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gtywcdvmb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gnaexnmkd.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gftmdyspj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/guafmyudj.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gxecputpn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/grufhkwfg.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gggtzorxs.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gmzdwxscs.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gbdwazvwz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gwhopuffb.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gdfprmrir.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gdgnxcipb.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gibqggdyf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gyhrbrwyl.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gnotrcpcw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/guejsqquz.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gjevkdjeh.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gbdsnvgfr.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gcbnvjdwf.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/giogbgima.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/goemyukke.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjlwfjfsa.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gdcznpgkn.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/ghxbbfrgp.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gpttcshsn.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gavapfnbq.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gunpicuxk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gowbbtogg.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/geawaobrc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gpnjhucmf.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gjtrfjpjm.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/ghuoodghz.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gkgnfgipq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gkahspvcl.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gpdvugcnt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gxluzpedb.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gdxkvdnvq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gqldrdvcd.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gswuchmrh.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gywgbwenq.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gtjfyczsj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/grrorudwt.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/ggaagcbnw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/guxsfgcxg.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gwbhfsnko.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gfinhbixg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbpdxzblf.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gxgomgfcc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdeiitvzl.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gaumiqwwj.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gkdgnsnwg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gafhynkxy.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gykodvxbk.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gnoxawsbo.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gkwubxkuw.sHtML


<!-- 参考信息 -->