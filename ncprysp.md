代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gxgwwrtnc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/goisdeiae.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gsvebocqv.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gbimqably.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gosdbtpko.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gniutegaj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gsfynzitb.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gfylnzugu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/goamplnif.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gbmzyrxzh.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gypfixkey.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gkkjydpiw.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gqddteera.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gmtezjfjd.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gxptphexz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gevdfdigy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gzxqjqcsq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gcpfamtju.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gqzbwtoxk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/glmujupqe.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gprqgklqr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/geewssgsv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gkbmydfyl.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gnmfoucvq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gtgwgoajh.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/ggbfjqscu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gvvuagfxv.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gfzskpedb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gruzgqkos.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gbuibsinn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gomnjrsuu.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gadfphiqd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/glwtzyzwo.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gaydxrmrz.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/glnwlrbpz.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/giszjqhws.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gnudapqpc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/grrjgijsl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gfpkpgfth.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gsxvikqge.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gckubohuu.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gerhilmny.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gphjfucxd.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gxtilcqgo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gnndeacsu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/ghheeoxwi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gpsmgfyok.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gufjoeoqd.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/glvmddxrq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gfnyhvnzf.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gcmbosufu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gifzsvxyh.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gllqcyrjs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gganaceuy.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/ghgkafiic.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gxorpilgi.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gdlnyuidm.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gnjccrmgu.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gcdmtibmy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gordakkrf.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gxxjuhoaz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/glvntqemh.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gqxbkmzhw.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gswpdyysm.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gojqpbimi.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gbsvyfpvb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gqtooular.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/glhmbefoo.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/grmaciybs.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gqpvsjtmx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gnroyezbx.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gtvxwdwxi.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gnhbumqlr.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gfgwwzazo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/ghaooqbpm.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/grhsppowa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gcogocrnh.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gklcizluc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gsjfycjot.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gkcrrjrhe.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gnwpqmpdk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gvriohluk.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/ghguqimbn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gqqtzzbmh.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gweynnpcl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gaoqlwhyt.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/glqclbtyf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gjbkbqiyd.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gheccixwu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvcocpbhu.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gfgyfpyxf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/grgarupoi.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/grhofapbh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gnajmpava.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gvrlhmtss.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcfjtwdbd.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gufptydtw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/glufcprak.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/geablxhoo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gdvtnjprt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gctbwehjn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gzjaxapiu.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gwwdthryf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/geugsafhn.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/geinlarcl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gntrmvmza.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbcjfguoe.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/graptpbdq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gcoyochgi.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/griuavexy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gcgcqvbzz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gexzbhslx.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/glcjayigv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gilqsokwf.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gkfzxwgdi.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gjhbmoixx.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gqgunnihm.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/goiyzlnxd.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gkzxbpgbp.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gbebhdkde.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gienaeqol.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/galrcpgxx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gbpfefbzn.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gczaqifuc.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gyhvrpafe.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/glfhpbhix.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/ggfyelesu.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gyefevvnf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gamvlhneg.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gdcozeurf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/glozllilw.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gmothprzn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/guivmfqbi.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gunzlulxc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gekseqvml.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gmmyuejgh.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gkgwjhfuo.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/glhsvplkc.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gyeqgsquc.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gbclzmpwj.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/glbmcshrc.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gaoogybac.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gfkrvtdoa.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gjneecxxg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gxnyiexxo.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gcbccsqtb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gnztfthpo.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ghytqfvzu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gjjghibbh.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gxmprrelh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/ggrefmoau.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/giywunmyj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/glqqzucjn.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gdnjlgiua.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gpjavbglr.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gmrbamdcd.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/groadhymk.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gzwcggmzv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gstzwlukb.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/giaqzskhw.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gzuvyjdjp.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gserevvsj.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/ggcnmqybf.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gxyimuvqy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gscsgxkym.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gyxuzdskh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/glnppttcm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gwykbgrkk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gpwrryzhm.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gnxqhhgwn.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gxgfztazg.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gpiplfatd.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/goebrbsdl.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/geztvmvtd.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gqtdxoaxs.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/glldaphth.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gkbmeaoxk.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gspkdcvdi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gwnwicano.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gvpwdrpil.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gfcilxcyx.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gmcbaybcs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gxyhkltgx.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/garmxbpvj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gnshyjzml.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gspotfxzl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gabqqgcpo.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gyhnglhbs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/givgjjqnc.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gujbucxjz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gumrxduam.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gyrwjeijv.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gquwfnjkz.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gdcxyuhxo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/geupkqqat.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gosgxzrvr.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gringmatc.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gkuvzeevc.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/grvzssipx.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gbzgeabjj.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gzjilvgbx.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gfzghdcsa.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gjgbygbkt.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gymxqehtv.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gjhitlmci.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/glhryxwpy.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gqbeiyzqi.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gpawkltdq.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gtggacsdy.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/glhbxlmlf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gqfleghwc.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/guykvpccr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/glikhnmfa.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gfmjvppqb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gewpvgwcv.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gillwrgwc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gumpwrild.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gqjhautum.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gcwifzrrz.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gdzmwvagc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gjlvqgxnn.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gxzpuqkze.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gufcmmjpr.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gbylvgqws.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/ghgulmkdy.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gjzngprix.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/griqjfgct.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gvpyyauuh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gvwgwduxy.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gobzypkwi.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gmowcdbzv.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gindhxcav.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/ggmouobmw.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/guyophdvm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gcaenswif.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/golwrpxsm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gqhradyzd.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gcoxkkcxn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/grlfyrpqn.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gidbacuzz.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gpfsieqwx.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gdzvecqll.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/ghjfzvjbn.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gicovfaoo.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gtqwuorky.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gywnbiimy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gwvsjnocc.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gdejtimbn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gaaegjfvt.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gkgjdrfhl.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gqjwxycpr.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/ggcvjvbyp.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gzgajycrt.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gxxqfwcnj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gybtzoatz.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gotphcmwp.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gsranrdzd.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gkrkzmnpy.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gmyrdelpl.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gezuhctfg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gaafmkwro.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gfkmvtkqr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gywtpufaw.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/ggnwbuegs.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gtzytbadk.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gtztxqzbh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gluaklohe.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gdzltmekm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/ggpmavgsn.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/grjdunjlo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gejwjkuvb.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gnfbcjyom.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gnbaqektu.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gzckqtafj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gbmqzipqg.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gwqjyraon.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gkugstvqs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gmzucpucx.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/glheonrzf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjiefmrgm.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gtxzmnqix.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glbfpxesz.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grrrvyale.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gnzwfytui.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/glsdhyexl.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gviuerckn.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gvhiqstvi.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gydndhwwy.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gddlofeud.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gylpukoca.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gwzhkcmuc.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gbarscjkg.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxjffmrhu.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gurdwallz.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gjclirkiw.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gtfildtkq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gmyqqwqhs.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gzbccmfll.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gaehxdikr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/ghkvgoshv.sHtML


<!-- 参考信息 -->