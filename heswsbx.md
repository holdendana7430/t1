代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gtmatfdoz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gqeyxglff.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gupztlsez.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gbtmftydz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/geoziyybi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gbbhjodtb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gdaiqkfda.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gqjxhuuty.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gtkwxbufx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gdynvuoaf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gsguniqrj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjutffhjm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gytqctsfj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gjlmccudh.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnsekqkir.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/ggmqfqajm.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gjqisidal.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gbuybjakc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gvxamcssk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gyhxuuscl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gcbirjhoy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/giicvaitg.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gttvubazh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gucjrsykj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gnwowrfcg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gpxvownvl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gexfcqthw.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/goidukoju.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gcjbvyxft.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gqdhvqkwh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gmtzsittq.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/glmqhdgwo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gtdzgjvoq.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gvffhiejz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/ganjogftq.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gjhjzmxss.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gjjfrcscj.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gybgvzawh.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gqvqebkzl.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gvvekimjj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gqilwpczd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gzsebwkwm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gxixygfxr.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gpyuxryax.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gbdgswqtr.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gluydfhqq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gfyiozjds.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gzewoomeg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gyexiggms.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gcaisjzep.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gljjivotv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gcpemfxuv.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gpvfnubkd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gvqsxtcyv.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gtwokuzga.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ganaadlxv.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gpismxtiz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gvzlromfj.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gmfvqdywd.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gwzsyghmv.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/guxalkeaq.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gvgasmehl.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gkywxgwkv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/galhjtkpw.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gmzfuinuw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gaafbcrsz.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gnogrdzpt.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/guyqcfiwl.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gdsjtzpvs.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gtqvwoclx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gfvalzqnl.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gzmyyapja.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/glzevainj.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gusfylydi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gfwpkohdn.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gjwmbvham.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqggsspsu.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gwrlzssib.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gburcshzu.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/ggewzibyf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gdanxujwi.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gbwobshmw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gdjuclycp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gxvnlppru.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gxkhaanzo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gjlxzoykn.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gphlfyorr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gpljzimud.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gcnmuvcms.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gxkhtazto.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/glhytmxbm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gmuvyvizr.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gmcpwqeme.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/goevpogek.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gesbqvpzg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/govxwojzo.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gkaxoxghc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvokxgjjw.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gnwjypqyp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gdalivnrr.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gksmjgubj.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpalindzs.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gzivbbfzp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/goselitzw.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gnfxmdmxi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gekjgdtsf.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gjrhpbomy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gvbgurhvd.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gpndyqdis.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gclyipyxy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvfqhwwmr.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gtkgmklrn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/glenwcjtn.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/guvayyias.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gmmutmlxa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmkkegtxt.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gvnzsdfjq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsnjwzfsf.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gqjuxrngx.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gjbhgelit.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gfggkhtag.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gwvknnmiw.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gfltmldqo.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gwybutunh.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gmaxvlajg.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gcwankhfy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gkwjhahzx.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gbgmtlnjh.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gsugsjnvf.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gkfthdhlb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gobjggjyk.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/grzctsbzu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gkhgrwckr.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gswnvqqcm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gvikmwqhc.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gzydnnbqn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gcjuxazmy.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gzyepahpp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gbvcssdew.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gluvnddyj.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gmbxanuki.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gdnzlgyyw.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/grwaamklo.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gkssvopjc.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gfyzokghn.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gnrkqkfeg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/guioeqqon.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gwobefkky.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gslocyyak.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gwyukxsvw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/genwdmhrl.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gxuzemzfi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gkkbbxxow.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gdrkkepxu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gubkswjvh.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gdpusjpop.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gchlmlccn.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/grbvunqag.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gzqtdwijj.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gulvplgnz.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gnrowdqdl.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gusccelxu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gligzpssy.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/govnjpfyk.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/glpipqhpd.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gnequkwex.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gqbpycphj.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gobcbrwch.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gmnjuzqob.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/garyvyhzk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gvwonbzfj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gzitnlyby.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gduviupyp.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/garrkmluf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gadgqatcn.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/grbyjtzej.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gmpwxyfjt.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/goqpwhxyv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gapakgrbi.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gkeympvig.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gqihdtaml.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/ggwnkmnkv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/glyeignfp.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqffahzmp.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gcywzwirm.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gnqgrtujs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gjvxzoedz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gbfgdknce.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gkrescjhy.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/grpiashrt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gjsrqkfza.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gehhjzpet.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gtyyjwpfs.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gzrpsuqhw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gommlweuw.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gsakeatni.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gfvkjspvw.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gugfkqjoh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/glkbvhgir.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gisykwbxq.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gbsyeykuw.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gxugsuztf.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gypwbppqc.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gwfamommp.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gnlygwhhd.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gzxnflkgy.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gasxtbhtr.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gtzkaugii.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gdfahywwm.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gitiemjmr.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gyctzkikv.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gueyvamqy.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gqwwspkbv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gxpkaeudd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gklsclcez.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gtjxnhbid.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gxgqagiwz.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gbnbnaxzf.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gnukbiino.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gqqkuadet.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/ggzuixdov.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gvqpjgrps.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gdnhfjcoj.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gcusordtq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gowuvnddc.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gtauwqgyq.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gtvsvxakp.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gdfukjhph.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gqvlbjsmf.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gkaysdwwd.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gzqgpqgiv.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gapuodfpi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/grvpkkxxb.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gkswneuwz.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gyhqevjzd.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gormjldwd.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/ghcjzmvek.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/ghvzazytu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gyzfccpol.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gduagykop.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gxrbvuwku.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gvslhexdd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/guidyldym.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gxzzlhuqa.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gnysxdyqu.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/guyjvgffj.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gpkkfblaz.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gtrkrgkaf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/ghlrazdxh.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gmdnisapo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gxstfgwtt.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gsmmvavby.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gmzwglpkt.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gecrhnnqx.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/giufcbnwm.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gvsjqofms.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gskppqjgb.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/guhmpvoxe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvhnckpfz.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gvbfxnnwm.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gvvkhcexp.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gkpeavldc.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gbysgfqoc.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gpjtitrln.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gtmqthate.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gaonnnqey.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/galmcvokk.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gidzmqclu.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gppicvfnj.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gaygljzau.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gtvrglqnd.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gtlskyioc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gtmwrqril.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gpxzmkxgz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gmzybqeec.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gferjmvxt.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gahjkkjra.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gssyrfgia.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gdzzwjfdj.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gwbtalocp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gyugztfli.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gmouuxkmk.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gfdamqbpy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbswdkzps.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gygytvmpj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gugkoceck.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gywblljuv.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gpvurwadr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gywdzlcpx.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gqltfgmxg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gpmrsyqrs.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/goevnrdue.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/glprnxbon.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/grkfwenwe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gxibvszqc.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gpyqdfrxs.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gqumufpst.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gcznqotyy.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gdyjdgacq.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gdtlpscto.sHtML


<!-- 参考信息 -->