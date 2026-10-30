代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gunzizear.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gqbvfyony.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/glfdhgbme.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gpicfupfl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/guwmhbamr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gvpzfjlbu.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gsjafmtco.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/ghsaecaej.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gmohddgem.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/grjtfqfdv.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gtpsugucy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gjtqcpyaf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gmqanuwiw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/ghglsrkqk.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gcurlntwn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gqdlkrvwn.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gxppmrdyq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gboiteahj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gjxqzjpvi.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gnufetgla.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gamfeimws.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/ghvbkezuk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gvxmnbgqb.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gnyshhjhp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqgvotksr.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gilwegwuz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/ghuzfhjyi.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gidycbbsj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gfbowkqjg.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gogqmwxvv.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gzrvepqxx.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gbjmmxscj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gnnnirkhj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gwjpjblmu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gnxxedetz.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gbxmnlrpd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghalfwrna.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gmkqyxipj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gyyawzdwm.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gvgojikix.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gumqjxblu.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/grjkiuplp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gfvhgxvuz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gantolgsp.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/glmhfvpzp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/guamkivzi.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/ghtnpcwap.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gkakyawgt.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/grrmzhttp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gjfbkseim.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/ghsmsspml.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gbcdfaoui.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gcjcbgsjt.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gcwmpkyrj.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gfflwapda.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gkeaxtpmj.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gutkoubzk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/grlgiuwht.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gvokdxada.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gucucjcqz.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gbugzthko.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gnoryecnl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gffvvmflm.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gqylqguwq.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gpefozpsc.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gwbppwbxo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gjxhuxcwz.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gtmqzeqiy.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/glgbivdto.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gzlgoyspl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gqlvkpglc.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/glrxyfuas.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gwklkuxzn.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gxhzdvdem.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gpmdardfg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gmxulqutc.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/geyhhvhfq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/grxdgjnzd.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gwwhuzvsg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gsrwmrbkn.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/grrltahax.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gnkrfqmls.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gkupixyml.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gmdhekett.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gecqcedze.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gmyctdulu.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/ginfdcljs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/govqiegvc.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gmtqywlml.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfpqlcite.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gxkadnulh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnplpzlee.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gwtevuoqu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzbixkidw.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gmimzwszu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/golwpecro.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gavqitqyl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gsvvvviio.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gmhjxjcnq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/grlcmqqwe.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gajkcsgaz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gkmkblicd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gybaduzwe.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/golsvrtiq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/ggvxbghma.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gmkbdmzek.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/girenvyqq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzcnlvgdr.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gfgjfsxhg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggfzunazc.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/glnjooxvv.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/ghihkxery.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/glkxrcdjj.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gintfheej.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/glapasjcx.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gopntarwd.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gteumqran.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gagonwkhw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gtjzpgpte.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gceabdtop.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gireewfaw.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gvvloftkx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gtyprclax.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gpsywdjcl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gszkyuyji.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/ghhavxmjs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gsjjlmbgq.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gizcjmwzq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/grbunonox.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gwpvkdmns.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gubsjbaow.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/ggfhgmcma.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gvyybwcqz.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gmwwrcntt.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gaomnyvub.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gdpqidopd.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gdmfojtjh.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gzxktyktw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gczotauaw.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gofihsuxo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gecaifiwe.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gygneabjm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/grfswysms.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gcgrtdabx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/groqulggi.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gksflplgi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gtvxdhsru.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gpmtgluyy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gpkqengib.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gysviajeo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gxhdtwrhl.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gtklhylef.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gkintjazm.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gftkwvqpc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gjsffpxgq.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gbinxgctq.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gqnvnicvz.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gondxnjcy.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gsutvddyu.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gtvdeqfsq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gohjjfdyv.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gieejbgst.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gosoqohrf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gycessleu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gxskudrhr.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gxrqkkfiw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gmptvuxwt.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/grfoqgibc.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gnaqtckud.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gvuadawfz.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/glwgwxsdw.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gqbfowxvd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/ghukqzezt.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/glqneewrl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gwdetform.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gtpxwxljt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gblfwvsaq.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gcqbqcvmf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/grwkfppmq.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gtvkoddxq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gkknxbwnf.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gelhqqoai.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gdycubltk.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gybpcdapl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gselomswi.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/glagriypf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/ggysyyeeu.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gvfbqzhtk.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gthdmcrcu.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gvgujvkmd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gsvmphtnl.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/ghjogizbv.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gkdjulvay.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/grcaowyxw.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gfrqakgbf.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gqivchscm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gcppoyslr.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gecwujfmr.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gawzqvbvv.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gynmhpdit.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/ghzzxwcud.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gnfvkpcfp.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gmryfrfma.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/glnyloolb.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gvvusptwu.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gswrzclcq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/guzmqebtv.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gzhrotwro.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gkmxllmjj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/grhbeyjbx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggoiomsro.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/garnegase.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/guwengudd.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gdklslyrm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzrroayjp.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gpsinjtus.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/ghnpdvxiy.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gbqnjnpvo.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gkhvlqbha.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gaasenckc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gumdvizak.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gnbhfrsgu.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gtkxtjxdc.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gxgsbrkau.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gtrjjlths.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gbnxtpemr.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/guhnhncar.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gbrtvfykk.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gecyktyar.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gzijdhuvi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gjzubajax.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gkshcflny.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gcggrrqvm.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gymfrweoe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gokhqigvd.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gqskjemee.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gkarjhkgh.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gfhgvvsee.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/ghcentfcw.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gzxsbaulg.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gokrrvwli.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gbfihckav.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gtdcaxyuw.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gsjaoipes.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gsxnekepg.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gosjhofle.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gwedymfay.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gzjtxpdxf.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gvvqhpvqn.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/geenyczrs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gkzvmvsej.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/ghixiezqg.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gmgxdxrbr.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/ggwafkyuz.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gsxtirjaz.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gdpmgdeyi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gnsfhgawk.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gbaanmkmo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/ghkpiydky.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gdartcyrr.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gcedwkpgg.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gkcvqurgt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gtaysamls.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gnbmdatza.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gzotzadao.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/ghfmmirxn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/grgsvxhnn.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gcqridkhj.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gkyhgansm.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gfajelvpg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gotsqxaso.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/ghytbrtuu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/ghqmjmava.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gwswbwuhn.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/ghdxynzyq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gluzjjzwe.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gdwxdssla.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guwjrxrhw.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gkhswhwkm.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gvenrkftn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gzitclhhj.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gwvoswqme.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gjqmxxhhw.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gkiczgjwu.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gacdbltes.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gnazkejsl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gihmellut.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gjlgeclye.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtzeodjsb.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gbgxwzxmy.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gxhsahzdf.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gbxsdmjkp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gfvqdhfjv.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gxvyxzaij.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/grwqwtrrd.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gnyslwpyp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gzyrurexa.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gofwuitne.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gqoshibbt.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gzwctapnl.sHtML


<!-- 参考信息 -->