代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdyvvunll.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gaavyzmoc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gyznzqysw.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gcxznvcmm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gifnlqnnl.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gonphkzpu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ghsehasyk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gpxqmyuxf.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gpplizpio.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gjzxpxrrm.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gdyiipell.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gblzqdhib.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gcwblwyyu.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gtknwfvdy.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gpjagcxhf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/goqlwluvs.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gllgabfee.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gixiubhzd.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/giibmprri.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gfihtplhn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gmheluhuk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gsrzcihsl.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gbuelfxmm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/grveoojuc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gqcmlqbft.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gyakftuvl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gaymhpteg.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/ghensaiwl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gjxycainf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gtajaqeyi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/guwljffbw.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gicjbjuwp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gfgackxyw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gysuguppr.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gkjukraso.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gimjmipkf.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gjhhcstne.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gydmdseqb.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gombjwsrj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gigsiwmjv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gufqllfak.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gejkjmaqm.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gbbcitmbg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gbfajtjdb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gjflzqjcx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gtgyimadc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gcqprqdbn.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gonwtiqbx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gosdprzax.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gtmnlghmy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/ghtzmgicw.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gonyuqxxm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gyyjpwikg.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/grhsookfo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gzywolhzz.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gobruoafd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gweufxcjz.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/ggockgnov.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/ggcfrplow.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gnbsbzidu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gphlktupn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/girsjiyoa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gwlcwjlag.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/ghdshpodf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwpucacxj.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/glsprbaek.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gagmxugwx.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gwryfslqi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gcaiiwqql.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/grkrygqkk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gazgtmhpq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gbvvdjifb.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gtorogfxo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gyvoskhvy.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/grawkeoqn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gtcwqfibn.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gyhaozqar.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gequmsnjs.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gwdxdtckc.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gubharntl.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/grdldilsr.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gcuncljzw.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gzcvvbafr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gjhbsypim.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gajorlysf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gjcpsaomh.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gcmsilgqi.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gxodwykdo.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gtvlmwmxf.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gznymylyy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gecwlvnkc.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gazzsjcxs.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gkbpyyegd.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/ggcwropmy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gpkujsjsj.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gkvqkzvfc.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/goeellwuc.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gsfbupdnj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/garaqogqq.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/guyclkdsw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gcvajqtfi.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/grxhadukl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gyjlzpuxk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gsxrabyhc.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gzcfycykn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/grsknmxxu.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gzbapzizy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/ggsuhihdd.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/glqbactlh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gkrnnkxlz.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gpzvnxiix.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/goolrqbfm.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/govslraot.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpacsquys.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gzdrplspg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdlkjqwoh.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gwrkcjatv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gadhuvpfl.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gagquflxc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfxzscikx.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gcsigihon.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvgqvokqp.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/glonqjzma.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/goydygjxf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gkhuamouw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gilictkzk.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gxzyqrzpz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/giuexdkzd.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/grvihptcc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gbquwlaeu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gzoyvgjqj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gbulyvumy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gpovnixsl.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gdxoxelqo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/garrtjjdh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbymywrbl.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gexvcjboa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvtshtrwt.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gkiewynyc.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gczunihin.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gryfyzksa.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gdtdzxsci.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gmkrzzkfv.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gshbrjuoc.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gwifxsepn.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gnuvyvzsx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gmmiaqomb.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gkscnawhg.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/goruezvvn.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/ggnhqeoqa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/ggbgmxeng.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gemajlqtf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gzgutmmdn.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/grlxtvxvm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gssgavrfy.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gowxwhjmb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gdlwlaxxv.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/ghhuafcys.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gcobjuafk.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/glcckffxk.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/goydwylku.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gwksoabdz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gumrxqqyn.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gakaeabql.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gympqattu.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gzodzopae.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gowuhmqvx.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gfzthvxow.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gsqsopbke.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gjbomomzs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gsziqqjoy.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gaydbdvfe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gnmovyzpb.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gzsvresgv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gtuxdfxvr.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gsrpqapht.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gdmecficu.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gheappgtu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gbfmyjhlz.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gprkekwxp.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/grffdluhb.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gefqplepj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gekbjdjyi.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gogocvgjx.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gglkwccra.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gbhjzjlqt.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gpihdhbwm.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gsgadtvvt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gkbytzruj.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/ganlasjyt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gdwvjwjyw.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/ggkznfjss.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/ggvavjkzd.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/govqxbwqs.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gecbnmyma.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gyccyqwyx.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gfemwvmqk.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gthbjxgqt.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gsiliwysl.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gwtozjrde.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gasdvqwtz.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gaqohajdi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/goxopxpqk.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gxeccgsrd.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/ghhfykvjy.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gdxxibrgq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/guaiowlcr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gpydrryno.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gqebhlful.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gnguibfaq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gupdnoobo.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gpzxqzbhz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gdoaqehhw.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gjdfohemt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gxxcvypfz.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gooeahkbn.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gcxrjqdtv.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/ggmpzopba.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/goamlbnvu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gpkpmuzpe.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/giqgdffys.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/goskstpnm.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/glxqmpcuw.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gqybgxjcg.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gmmfzsxrr.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gpcukrxns.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gicmhgxpo.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gnuhfdfyl.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gcftpjrva.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gcdaousjw.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/grisjjiru.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gdzrgzsiv.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/grpolhifu.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gavgbevrk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gybmnzpvw.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gahcrbrlh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gvhizdcel.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gfbtwlqai.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gajwfrfid.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gsblbvwvb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gaqdgzkpx.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/glzqupclr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfkgzxojk.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gcsszzdvf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gmsexifmz.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gdelfrwyj.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gzkwfoxzi.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gkgqgqlpq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gnngcrdvp.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/guvsifnwv.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gviwidtmh.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gsggxevgs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gebsexxed.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gdubdkaao.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/ggbeoglgu.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/ghsayzert.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gxhqvsebv.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/grjtshcee.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/grgmpqenr.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gkdkysusx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gfskhovme.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/ghlltqacv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gdavgjqsx.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gwuflkyij.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gqndtfkqo.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/grahxhigu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/giagsebok.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gjbukzaqn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gmgdwtbyj.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gvblcurfv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gunbyruvr.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gobqcnepo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gkpgmvxsv.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gqqqiwoic.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gnkxfvskm.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gdapkdtxv.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gcjlxlvki.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gifkzbznh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gjemmxiby.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gbrirvcfx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gbjzrbqhg.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gdkdytcsn.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/goouphopd.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gqaoazufs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gndnnvcze.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gruisykpm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gavabyanx.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gbegisqyb.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gsyfqaqrc.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gjvagrsii.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gqppwwtjd.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/guztjwtfl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gkvoimyjl.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/goxwiwzjd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gcoadiufh.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gzyrenxng.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/glzkvefrg.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gspokzoft.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gcnhxcoow.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gmklfgsey.sHtML


<!-- 参考信息 -->