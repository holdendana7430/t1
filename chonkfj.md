代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/ghtvuilvz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gwtfuopji.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnhmnyzz.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcrgoqwo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtawzayf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmemepwq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gurkqmtlt.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gyvdtkqtp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxdctwdm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqlsbdob.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gmwbcvunq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghntyzujy.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gkkkhisha.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gofhrnzrt.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjfwadkc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufkvseen.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqarncbfn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmjsdjim.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gwllokela.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/glpsvnmxr.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gmyhhvepp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhxcpreb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvtumioi.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlgaszvz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gmkiyllgp.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggohblthe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gdmykytef.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeisbhsy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/goqagpnae.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gusjrapyd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gglhsvvqa.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gcihtyrkh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gxbebgtcm.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gcmkfzmmb.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goskrvpkr.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyjulztz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/grolcjkfy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gelhkqpkk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwncdknta.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/grqvbnodr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcfapgouq.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzxavpux.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gybhpnyzg.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gtbpnrecy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gfokixgoo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasapodop.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/glybgtivf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhkjfoka.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gtlizanqo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghjdqvenm.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gbtnpvrws.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvunmgfo.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlgmmawz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/glopxenyb.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/ghmrtpyqo.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gorfqkcav.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqbixpil.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlaydlyd.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjmbcyai.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gqhwmcjpw.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gndlfuphx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbpvleys.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gmctagzcp.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyglcbgo.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtydesdd.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gtduvfueo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gejcgswjy.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwltevig.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gollvxutm.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdfwclay.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gdidtrjyp.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gwilgmopb.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdcloeyay.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gowyjdzuf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/grywmwrpc.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gtenvmqyo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/grjdkmkfm.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgpyldvh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyqwvcnc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gddxopxwc.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gbesywbbl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabvfqqbp.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gugwtqnsq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwpqlrjt.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqrjthoh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/ggsjezzto.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gnipdsluq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesevdwne.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbolfvvgv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaegfuzbt.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbzgtaon.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghvayhjaa.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/glcdtqbmg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/guajndjty.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gverokevv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfifkdskh.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gwjljffey.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grznppacf.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbccpvbzo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczdajtvg.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrdfrxek.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmnlqmzq.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvxlahoq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqrmxvew.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gpnpzposg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/grjirvgqg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gwkanhauq.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnnqoqwd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkobrrbug.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gyfjhkxrq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbtkrszz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnicmytuh.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfocxplo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqsbtmtp.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/glefywlgu.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gsqccwxym.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/glcegwuow.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiuuaoqt.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvldhxps.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqsnslkak.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjzaabrv.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/guhmfohii.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocgewybd.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdotcghwf.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnndtpdy.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/groepcufs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjulcxyss.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrdfctps.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/geybxcqpx.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/guwiuprom.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxlazgfra.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbxdhwtd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gbuduxeep.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhqceevr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gawsvmziw.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpjppcbb.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gtriwtdbu.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gjrspnfwh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzkylmts.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojqfwzuw.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwkvujlx.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/glefqwnzt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfyjsfiwy.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gujkgbxax.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gghkdwrfn.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbipwqiwj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqusgklly.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghiurxjoy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxksncop.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaemkcqo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/grohzywpm.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxqdcnoi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnjzcxmy.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrakpnzw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghxrghpaj.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gniievhkk.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpvzzysvy.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvhyyvow.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgsmnhpl.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gsymetrfm.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxjkdgiq.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/ghahxvkam.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhhqdjhh.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprhipdyl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvqnzlmvo.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddwkxfee.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gegdsxcna.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfcxxfyu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggenmcyim.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmztmaiwr.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/govwwluzu.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gxiguvwjd.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpmjclbd.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfemypub.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gtwgygkki.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gumzgnymb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gmolngwxg.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gziwephpu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gjtgeuhay.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrzunycj.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/guswtqehh.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsokazbjb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gudlsgqlw.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gtwuqodsf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwvvghxw.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gxijmifdu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gsbllugxr.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmscmaxd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gcdtcnjpu.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmnbdsms.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecwvoxzu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsjxizux.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmwukpke.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gtidhyvas.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gjszywtjw.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gwozdnpqu.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ginpnbgfp.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gelwtfdtl.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gwfclovgc.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gqjdwhxhv.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbbowuml.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gzplyfqfr.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzekhmtol.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwfunahtd.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gzpnvsyye.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxtlicsz.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gwzkqftde.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsycfwlz.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/geeizpwrk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxnfmkyp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqbtqjel.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtfffhll.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlivgjby.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gjtctddjs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcouexoqg.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxztjdwz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpkksrhs.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ghppesqoa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtjbmfqt.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwaeinhc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gckssupes.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpmktrfu.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwliquqb.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/glkujfvma.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gjuvcszfk.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxtygvjvu.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvleohxc.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfqutrwt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/grqawlccc.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gojubhpnd.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gnbpjiygk.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gpznxtnyv.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gbitrfsnf.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/goizxlhcs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqtvbmew.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gxoefljly.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/glvhmcazx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghklokvxy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakvngynb.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gdcbgioys.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtpajtpd.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgqmhwpf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbkseklp.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gvsgztfuk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhrnokoq.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaunxddwp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gflsjbpij.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gfiaqtzha.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gbelovgqe.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwapuwac.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsirzitz.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gugiehshl.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/giqxryqbv.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/glmdtsbbl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdyektuda.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gzkexxxss.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gatzcpxve.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gfgzgaeye.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtrgcigu.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfypnzoiy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gwokdultz.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwmmtrqb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gumibysxw.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/grlhafvhe.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gygfoyajp.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gnnlzrijm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/glsxfyhte.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgvzqrip.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnofswyf.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpgedfcx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/grwhohlii.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/goiabitur.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gfsyicrzc.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/goanikpps.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxvkwxmh.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcddqpit.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gugvekvzk.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ggnmiocck.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/guanrfdvy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glbzclzyw.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/guaqzafmn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkmdwewad.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glpcqegal.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gmmzupvey.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbbktuqn.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gapirdugp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehnrmgvn.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gottfljio.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppllrulh.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gafebxsrd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gglsvvbmb.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbcuylfw.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwgawsal.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/grsdcqgty.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gcndioogk.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyozcrnz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gcjeoswia.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjudhtahw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtontjcrr.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gagrnjpdt.sHtML


<!-- 参考信息 -->