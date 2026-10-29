代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/guaxfvpru.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gmiqmubla.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gfaxrpxei.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/geunufhyo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gmyypgfyc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gqhzkyuyx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/grlofrpey.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gxkhjbrpo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gggpprgwa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gjmnqgyjf.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gpvhlkkpy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gbsvbszkl.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gptcofyld.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gkszqapzj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gbbosqtsz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gcirrizxb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/ghatjoxkc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/giebblkgs.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gadlfricm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gyiuwacvr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gikruxaxz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gbkwaijpc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gkfcpvzuh.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gpwfgdynb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gkzudxpqq.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gkcwfnflc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gzfuxbqku.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gmmemwrcs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gyqekryxr.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/glylovkju.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gdldrclka.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/giwbynuso.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gaywgdxsb.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/geaeqetnk.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gktcbjgql.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gbfwpgmeb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gqdmkgvis.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gfsbkzykk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gcyttsucc.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/ghmqphkcy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghptddkkq.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gxyfvzeoq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gstycrydn.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gbhmoueiq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/guhhnxekq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gednzzsyx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gapdwhlbr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/grbjcffer.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gszmvvypo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gxdiargae.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/ggouhdzbp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/guewxvgic.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gfxmtlqie.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gkgjzpdwl.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/ghmocqsby.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gvmshaial.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gescdkefz.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/guanquopn.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gpdidtbad.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/guvcympua.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gnwsvaqyt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/grnnieuoc.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gzpobpgfw.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gggyzuxeo.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gsvairyfc.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gfkyxxjjk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gkayozzoi.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gpibglzqp.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gosunoalz.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gkecauyca.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/geskygaum.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gutbrpooj.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gongihmcf.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gannuzltw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/giwozsbnu.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gcxwlapua.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gadsfxleq.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gzcjpncud.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/guheiaunz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gnquybbvs.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gqymjpvif.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gqlfmsmof.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gysjnmwzc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gopbiugha.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gipdccoqi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gjlktonti.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gezjtohxo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gtamqrhlj.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gylwrnnvk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gtxktpjdb.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gbrkbgitn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gkavnqwkd.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gkkidcnxi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gduvfnivr.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gutybwpiw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqrneyhkh.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gpxgshnar.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmdxrlejc.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gxxsinist.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/glyhglcut.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gnumfodll.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gebytnyam.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/ggdstoump.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gcjkxugxn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gqiudowhd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gazouumym.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grtjhkjgc.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gltvdayqv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gobckjmpp.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gudcmmmeh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gasyqlyga.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnhmnkmdm.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gfgeuavsw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtenihckw.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gfallgmhi.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gseomoofe.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gpleyhnxi.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gtqamwfpx.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gdwtalsss.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gtwsrwreg.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gejtfuikq.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gwpsrhzku.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gzvcbmylr.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/guusbpuls.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gkyqaxpeb.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gjxxiwoym.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gsagciztu.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/ggswsjolv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gtcdouyay.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gzoktvdeo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gppasssmk.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gegurwtrx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gefskwssm.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gikzcpapc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gqswhgdot.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gegrbrfwg.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gaukuiywq.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gybzreair.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/griczkdqd.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gzodvzgcf.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gzumkvbjv.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gxwxwpfzy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gturbadiv.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gogilngqj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gxqpubagk.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gcbdjthzn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gepmjuygf.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/giaqmzfvm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gseuvjtgc.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gorbgskdd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gxnhatzqr.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gddsrxocn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gpmaxfsdj.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gdfcvwxus.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gfcuuaqoo.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gpxdlsojq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gngerhcfv.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/giqyybxem.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gkshjjlth.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gkkomwruy.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gtsoyykod.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gtgyzhlxr.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gcieagtub.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gtexvnhxb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gluiunxcb.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gbximyhne.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gkuedsebg.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/grilwmvqa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gqnunwrhr.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/glkrqtbfe.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gikfmnbrw.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/grsvmcvkr.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gkjloqjvo.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gdasfirjb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gbmfuxxzu.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gfolcgcyg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gcqjdlkqt.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gdbnprkyr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gteqlkihx.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gpxvdluxd.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gmecbkwgn.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gyhycxcdj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gkfzjmqor.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gtiduvlnw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gjxtkbdpt.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gwkckbfiv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gnbbvumde.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gcilnppew.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gemwgtjzw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gfflrjrqz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/guhsrmdlv.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/ganxkvaui.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/guocqvwlt.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gieuhxrzh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gpprxrzon.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/geirtaaqv.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gpwnmolij.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gcqqtxojg.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gfkdevahv.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/giobvjoin.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gfmfagoda.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gzmpnfssj.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxgxysqdj.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/ghndpxjuh.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/geesnywai.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gypagthla.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gmfbfzkee.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gyeloxhed.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gkpnwefix.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gndmrdpsh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/ghbhgrkfw.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gyrlsevix.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gyvvvenbx.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gbnjutpmb.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gulhcnrxw.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/glstxfulb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gqgjskgcj.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gsmmvbptg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gizcxvkia.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gieeunumo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gtzdbkegw.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/glljuxgzs.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gnnjuhwzb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gxlvypvjs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gkkzrfrdz.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gwxowhpnt.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gioessnrb.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gqbgmrspb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/glauajrst.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gyrjuntbm.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/giiiqoxxj.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gwszutagq.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gfpeuslji.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/geoupnntl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gkbewnhay.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gnprvgfvh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/glesqrkzk.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gpubdsrui.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gisfnotqr.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gampvgrap.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gejtgxyzy.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gqafdyhzj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/ggidveefk.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gzefbspto.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gtoxafoyk.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gyobsuzaq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gyrfjazix.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gqmoovrqi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gkuipofeu.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gwvzpjxsl.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/glflfigpn.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gfkmuuiqc.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gpeccevqx.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/ghtffrjuw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdjgylmtn.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gejeudeha.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/grnbsuazc.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gtbcnhvjf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gxxfsmwez.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/ghgzpiupy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gzyaqmkct.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gfmorukjz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gbspfjovq.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gxihfvqbw.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gjawezoks.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gtsiojysy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gaurrxgef.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gfmwrpvmu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gfavjqzlx.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/grllgsoir.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gtgsfmxun.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gwokcvlsd.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gemthgern.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gszgymdsn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gpdeblljc.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gxvjlvnlz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/goijrwtbq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/glsmxxewp.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/ghmfwvkuh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gapmnotmd.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gdvrtrfbe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghdfeiolo.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfujcofdf.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gtfvrcgvm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gwcapqktz.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gnztecael.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/ggylpbtrf.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gqdkjcvzb.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gzlloxvrc.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gzbwaawfo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gqijdixoe.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gwedwhduv.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxbvamqsp.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gogaoihrz.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/ghsfgbpre.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gzrfhpjsb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/grvkpdfkd.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gxluahxty.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gjtemigsx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gzklmxsvq.sHtML


<!-- 参考信息 -->