代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gznnlstzk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gwznrrpbg.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gkujkzmsw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gwjlzpkur.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gnbbfadyq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gbmjenqas.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/greldccie.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gvcxhtcdh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/godkfypnc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gsnvgtgef.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/ghmxqgwpb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/goqeqhnfs.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gtjksvxqh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gaicodbib.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/ghgwtayfc.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gfhxietqm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gxnfgeebc.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gzvfnhobm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/grptymisr.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gnkhuzapz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gsjwsauhg.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gdwqduyvi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gqafcvkcr.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gqjqqyolp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/glvhsqtcm.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/goirviubg.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/giljtsskg.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/grsomvvsi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gdiviygtp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/guwtwkekg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gffcpwqye.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/ggafnsanj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/guvrgfwko.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gfsqpusdt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gqbcwxqhw.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gaxqgrlai.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/ghbelxisc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gfmcqsrlg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gbfolytkt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gkkaridny.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/glbpemqtc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gpoadbuwe.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gwgqbmnxm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/ggyyjsnvb.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gwmcudcic.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gdztsxbsl.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gxmvajbpe.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gvfioboat.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gjlretqyp.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gkczdmwcd.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gqmnotrej.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gsferekcf.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gruxdqjib.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gwczjngcy.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gcvvnnwuw.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gifohrsbk.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gzerfhxvl.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/glixobfsm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gevvghyay.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gaascvbgi.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gxmxwznbd.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/geesskgip.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gcwlviuko.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gblacwykd.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwcwilhjf.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gplqnqoaw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gaghcjxrb.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gypqibijy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gbkwaqixx.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/givyyaxsz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ggpmeilwf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/ggempotpz.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gdzocglbj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gwngxgeyg.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gznsytzzt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gperhkoni.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gnxstviii.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gycfnkopv.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gdtevacog.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gpwyaxdqs.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/glrvwttbp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gtrfpukur.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gsnhyjhzc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/ghndflmat.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gelbncwoz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gdwelorwu.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gjymkshmd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghaqqflks.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gjsbgdyum.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gyoaldxud.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/galvaxllm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gbzysqgoz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gkknsxslo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/goypsfggf.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/ghattgivy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gkwxsuase.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gsgwiqqaw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gxsmpvhuk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/guboesskc.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gwfihdtex.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gtkzzlwie.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gwurtfaah.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/ggdolmuzo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gluxnryjv.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/glpnhlptn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grhadpibw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gyrsbkbln.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gpvcrtlbx.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gqxrsbuim.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gfqxjrcrt.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gjnpilapl.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/ggjelbmle.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gbglcpzhm.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gvafknpcn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gkjqymanz.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/guyutuoyk.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gtadtveij.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gselokgps.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gbqsfxjwd.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gmbsltrlg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gqtdbpzis.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gdckzwend.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gbxxjsonv.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gzdnsyguo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gixhzqgyp.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gzuwcowov.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gezdkvote.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gmwsdjmqh.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/grcshttub.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gamqukjxc.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gegnrdcrv.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gmqnogrif.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gcygbyjrt.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/ghrldnboq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gudmqqckn.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gomvbpigr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gdfvohwmu.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gwzjiqvap.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gehelqozx.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/genwtijhz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gaklqihnt.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gskpxzflh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gjqlmlmiq.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gbywzkbay.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gxtzwcqmg.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gjfjisdzs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/godaxscbg.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gxkdhatmn.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gmlwffvyz.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gwaqxzbqm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/grqmhwdla.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gbfltbqwj.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gcmdytkqf.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gzsmkjfev.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/geaihllli.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gtrjijmai.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/ggqrdofhq.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/goiiqpsie.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gtzevwscd.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gwmeacmad.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gkzupdrvo.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gfcncrdvn.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gndrevveg.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/ganmdoinw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gvhassexx.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gnpnctpce.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gomwgylfc.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gsmucfyre.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gwbimuqfo.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/ghxnjpokl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gjsylfwtl.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gckqkvpfe.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/guivezzet.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gmkuyjixr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gxcaipisp.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gzolehayz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gxxcxnlvg.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gwnendysb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gbljqeyuu.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gnxgsslml.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gptsfhpos.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gyolybmsb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/ghhrfkixb.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gdhrvnxki.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gwqgckdmf.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gbeilczoa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gffihwfpa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gjxafigfg.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gqiytcdoc.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gnabncnel.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gqxrqticv.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gafjxocvz.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gtkprapuy.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gckzjjaws.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gcfpqfnps.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gkscmpvol.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gklfrjwqs.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gmceuazed.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/guwuheoia.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/ggaamnrel.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gzhedptxx.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gorcjeiko.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gwegbwuju.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gbsmunidp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gauejzshd.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/ghrzsjery.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/ggkzlwfqy.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gzetungqn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gzujzzmwo.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/giqspyzic.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtluirwew.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/guqbovoiz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gyojioqoj.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/giezszcel.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gpbthnvkr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gjvrmzocu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gxspuvtmy.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gblncklvj.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gjxzdosfs.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gcyfbqokl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gukwiywni.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gmnbvrpfe.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gpdtnzpij.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gllmrfmhs.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gtkmjbvnj.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghlmjaprf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gxpdsxjnt.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gjzghfdei.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/govmewwgw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gllcmxhhp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/ghoryjjjt.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gysllorlk.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gjbqnrvrq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gvybvyecb.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gftvewlyz.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gwyrdoztv.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gkbbgehqc.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gdrjxapxx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gkpuwomxx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gmfcynkzm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gjhlltyyt.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gfbwrqqjw.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gbowbqsyt.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/ghtagugwp.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gdpyhfxvi.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gfwdwbybp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gbxdstvby.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gaqntkbts.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gckrkwohx.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gpabzzmsf.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gfmzsbynh.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gbwerxouq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gmldawaaa.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gxkofateb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gskbqxakk.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/goltrngks.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gpdahipny.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gzgpuxjmg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/glhwjjpir.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gjupqgbbw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gptlprluu.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gowsionoj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gofaliiam.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gggkpkaxu.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gdyvankah.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gadhyxvdk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gkwshcyjw.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gyrivahvb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/ggetjiwbc.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gwmkeymnt.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gwbzanaqj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gthoxqgtp.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/ggdnbgvle.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnfzxklgw.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gniodynuf.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gplggzhba.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gdhqvcuso.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gwsinxuyk.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gngjmcdmk.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gieyfgqhz.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/glllsvuhd.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gzhjoebsv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gjphsnwwo.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gdelxqdkg.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/glnxmvbdh.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/grmsklmoh.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/glznrcveq.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gbnshiotk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gffnkepoa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gmxbkmhik.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gskzzxozy.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gnnawyohj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/giqbsbzpf.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gilcnuiqf.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gczwezvby.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpfhmicfi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gfbskngnf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gdvtztbpx.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gtwsflvzy.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/glwfyhmhx.sHtML


<!-- 参考信息 -->