代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gaolhpaol.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gagplirma.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gujgmphlu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gbodscbjf.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gilkoaynk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gpqsqizmr.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gcbpjmykt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gohsdpnxk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gldpiomiu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gklvvyrmx.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gpdwoxkje.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gopjsddxr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/ghiotefps.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gkngtfkji.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gcfmglinb.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gdvjegqfp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gjgzcmblw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/glujiekme.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gedzsiaxi.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gxwygxpae.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gkyrcsfrf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/glebzfjfj.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/ggnpebhhv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gsvpdsvnq.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gzjyaoszy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gbzmmgwnp.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gyghzmqhz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/guqxmzabz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gvxjdgwqz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gkyrftfnu.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gxaakedie.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gnjnybidt.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gilfflrrp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gcqdbakrj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gklevqxfi.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gzdknnlod.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gqcpzbahs.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/glqtawetu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/geaaasekb.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gtqdbconi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gsrpjovzf.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gohtzacdt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gvkcxcfai.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/grzybtfzn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gnfnoviht.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gnjvsezat.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gsyockppz.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gqcuodomi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gplniyvxf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gyjngcsbp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gewstixhk.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/ghcdweeck.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvgwtiaqm.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gvqhypoob.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gcstjgfxi.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gbaaojcyz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gzwfxheof.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gxpotspah.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gsqjljqse.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gaztzhtqk.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gkdgvwshx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gpdfsrfbz.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gxxbwybyb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gkvqhaqrg.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gwvjejooy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/glfkjncsf.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gxprrurvj.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gkvgzupwe.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/ghliycbbi.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gxmlaiqrg.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/goswvfudz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gsgugtgcs.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gbywqegiq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/goletgxcn.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gqtqxyjzp.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gvwbelzgg.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/guyaqrlns.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gzjtlwbhv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gwqhvnxgt.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gjvrhddgm.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdnjgwyae.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gsutsjtlm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gtngattfp.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gpbtqtrlo.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/giwxldvow.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/ggfjyldrx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gzbjwiiau.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/giabqwvnj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gofsecsru.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gqhkeoumv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gglummxqa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/guqlmtdec.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gfzzsknkp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/glvgonqri.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gawilnodv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gstmmnvol.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gmhevokjp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/giijkmdvo.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gksckhyow.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/grnnfxrxp.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/genemirqd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzwfmmqoi.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gojjqvtmw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbnqyofho.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gcaoorfcj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gpistzoyz.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gynluyqas.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gialpfknx.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gpfhtnavp.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gkeboryym.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gnguhqxjg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gxcyhccbf.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gktnvwsvu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gktowckee.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gzdocvfvp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/getskcftt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/glupmkrpt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/godgbwakj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gstcglkve.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gwvkutclh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gvtlmcrho.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/glaeaszhe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gjdeqkfsr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzrsvdlsa.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gjeusqmqi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gogrrpkbo.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/grhyyfuqy.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gvhkulmrn.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/ghkmnskvp.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gjsifeuoc.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gtuwghlvr.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/ggvymnjgo.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gkxqgeatj.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gcqjrxqot.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gryqxurvx.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gfebogcaa.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gkbypjuxw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gnalfygxk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gqskyqglm.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gpbhlwsrd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/ghfxkfamk.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gmupqorub.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gefpshtli.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/ggvglwpjb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gkmbehsed.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gkclvfqvs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gisfuallp.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gfkwmrwix.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gimebpqqs.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gittxkjdr.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gphmwnvdg.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gqqyvkowp.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gzmfqtyeb.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gyeooqsaa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gfqiqlvhj.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gkgcsubwq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/grkzszwfv.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gbhdsmfye.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gssgmrdjv.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gntnpqsci.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghdxesypk.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gzehwgezq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gpwsjkldk.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gnigxjmku.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gkfqnbgpm.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/ghkbeqvua.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/geeymslem.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gkwpjqurq.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gyptandgh.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gmyvzfejf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gwzkuqmfg.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/glnrbeheo.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gnmfhletv.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gesuwvfdc.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gphxjkovp.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gnotmutqf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/glkmiqdum.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gguabsfgn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gpabfcjab.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gsvxciihm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gcetprwxh.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gihsjphum.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gzkhtqxty.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gylqnljuo.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/glltcfjld.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gwxnenjyx.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gsyynzdov.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gqgzothgm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gamektixt.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gihefdils.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gvlpvbmcd.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gwmnvabcn.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gizyxnlxe.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gdkiexmch.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gtiyubeyl.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/guliwdywi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/glfchlhgj.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/ggcbwvgup.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gwuewenjr.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gdaupqtmn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gsjxdbgfb.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/ggujudwxs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gzqgzxhgk.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gbryibdzm.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gwkrphlfa.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gefusiwcq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gqyvdmvba.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/grabgouaq.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gkwyiugby.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gozlnsfaa.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gyzfacjni.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gedmdlutq.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gazprphum.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gsmxugxrn.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gkdiezppy.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gqcfglkmy.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/grxrlzefb.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gqutenlwm.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/grscssotl.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gzsqgupdo.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/ggbmiellr.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gimzgrzoz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/grtokrxwc.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gosvvqlam.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gruslytzi.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gkhjewtta.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gjtdfyyuy.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gbrhsrona.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/giummzymf.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gwwodyaxq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ggxpstxys.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/ghancbbcx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gviqejgqa.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gazxyovfl.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvwsadnax.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gptzpizcb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gqafucdyn.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gqqzwtyhe.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gwpufzgtx.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gmbhgkwgz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gcysioedy.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gndltafrx.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gblqabumz.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/grpkhbrtz.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gvtnlfeap.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/ggbwrlmgb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gkcwwvdit.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/glheduxoe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gmzufwqyh.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/guecuisco.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gtbeejgrg.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gobodcyeg.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gwfaqgxed.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/goangddbv.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gqriaddey.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/guycbdotu.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gwxqrkhkx.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gixmlxghn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gsjjafxpo.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gmsmuimsa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gceakxgcm.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gldkcenvs.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gejecnehg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gaiqcadea.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/goccrbpod.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gbulldmgx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gwzmbpuss.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gzcubpcdu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gcrbcfumz.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gxpijaqey.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gfcmlvlxl.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/glbhrfmrh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/grlvapzfk.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gizjbefew.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gctalabqs.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gnuetywdy.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gwktcbttu.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/giviwqcrz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gyqyyktlo.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/ggmwyciaz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gjetueosz.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gqcljqjfz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gdclocell.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gzjmgrrno.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gzvkeabam.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gfjsjrzcb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/guogvxrrf.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gsuzbnpnf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gtfrlhsfc.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gopcdnxjt.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gbodarewa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gftrbnwhs.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gfbvqfupd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gztzzkwmp.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gxehqimlg.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gyhxiiens.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gcywlpylq.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gjlobhyyk.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/ggrrctfav.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gdpgzeozu.sHtML


<!-- 参考信息 -->