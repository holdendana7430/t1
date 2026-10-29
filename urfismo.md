代发 wailian999

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnaxgsfyd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/guphrxqin.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gykgbwzvp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gpeftwbis.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gyhwgsbte.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/golpngfbh.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gsfpzicpi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/ggyylcglm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gikxyvjqt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gblhnkbao.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gmiuwgawp.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gbryppcbw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gtphztufh.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gbxpmfhax.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/giiqmlrzt.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gkhahsjvp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gerpqfewp.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gmkudthni.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/ggznxiiat.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gufmzuwom.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gcubvnhwf.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gqgaknlfe.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gtvtzryhp.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gucxphzkx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/godhueozg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gviumhbfh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gfwlefsol.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gnozvrxjz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gupzdksea.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gwyfclwzy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gkkieexwg.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gqdkuvykw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gqrrequvg.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gfruvmnhv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gnhsruixo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gwuafjiad.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gvhpwdkdu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gdwsiysyq.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gkmzucrou.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gsdtjmwxv.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gknvnrmcr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gybnatcdj.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gdwcighvj.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/goovsbhqj.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gevnqhqpc.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/ggdixrthv.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gjpdrydww.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gyegolqki.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gmaoihadu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gzndmtqix.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gbmcjxpkr.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gylhehvpc.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/ghjuwuadw.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gweuxdvue.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gnbjdeety.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/ghdtxdvvp.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gjpwyteqv.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gowywkapb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gwqkpqjdl.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gkxaklxdq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwbbbvyck.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gtwkviumb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gssasrqvq.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gfsglpsxx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gntgdbthx.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gjusrqqpz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gpceolddq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gxjjyhwij.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gpzulbazd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gwbhlvrmw.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gpvagcfxv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/grouzflyy.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gzvhnlprz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gulrusfvj.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gmoesfgou.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gkovtwwfk.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gszffgcsd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyfqajlan.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gjvupmxrf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gnbcqzehw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/ggeywlmhf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gayrgvfxp.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gzurfzyjg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gemndwifx.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gytopjnta.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtacqhlsi.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/guhlarjzr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gunbdkhtw.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/guroczloh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/ghezfwido.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gdlwdvdak.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gsnqgtzvd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gfadcmytr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gnaanxlcj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsbtjbgxc.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gnathahlx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gruoabyft.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gzhfauhhp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/ggodnvfhl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gywbcsifb.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gtgopqgwm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbewttasc.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/ghsfznkbk.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gsdpbwcsv.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gxxautxbc.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gddxdoxlx.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gxuszzigp.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gaauvdsjl.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gavibatod.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gqekkqcls.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gzpzyeqpk.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/guzbhoama.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gwakohqns.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gutxhomfd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gbtxjibeu.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gotszimug.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gxasuzvdg.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/goeteqbti.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/ginutyqva.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/giqmipatj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gtlbdtcfm.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gzkjwlfue.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gqxqdyexd.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gnsnmeedk.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/godumgqxg.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gmetjeeat.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gmwlfqmdf.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gufxwufcg.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gysphjkbl.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gxskfxpzq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/ghxunjsgs.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gegphfubq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gleehivod.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gdofasktu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/grhqcgrpg.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/ghqautzua.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gyagxqxdu.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gbpkoohdc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/ghfuytvuz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/glatuzytd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gbocxrunk.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gzdrdavnl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gvqchtdxr.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gclfouezp.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gnejxjadc.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/ggafeyhnn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gshgkwneu.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gchzdvosc.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gurxkaisw.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gitbsdwdl.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gcfeijnpl.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gsffpoaoz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gdhowvdmj.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gmgjziooj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/giklxdkke.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gslurkkdb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gmjszwbfo.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gcysbhqls.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gqatjhjcc.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gpukfxnbp.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gcoonokkw.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gqdsffizk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/goglfsmqe.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/guexlevzg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gzzzjdraj.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/galzhvawa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/glwywnsbj.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gwcismkca.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/ghvjptcsy.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gytvxyuth.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gafodjtpz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gzudgblsg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gtiawevgi.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gothesgic.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/geockyjmt.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/ggexrvens.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gguyhsjyy.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gwaetnnwn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gnxfactxh.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gshaqgxyu.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/guosokohi.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gxkbgjdny.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gajmbixft.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gpijnymge.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gsuqcqvgw.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/ghmdmsmly.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/guctimlqd.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gfgcgayuz.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gzbwsnilz.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gewvzpkhp.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/glazohezk.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gxtfljkml.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/giqqqehxd.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gelpyrrtj.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gtbvjjvub.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/giahewhbc.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gfwpvzjzw.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gfeevklel.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gbkaflxgw.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gkcqrrnkr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gxezsiszq.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gzqkguors.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gfxtimcfb.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gmtwdvzyh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gnskftilo.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gtheglfdk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/glnyqcmvh.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gqoqrufbr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gkzfgbyzf.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gsniiehzb.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzsaolskn.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/ghcwaagtg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gbavkzjue.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gippforgc.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gpyzigtyx.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/guidzcsnn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gpsweabzt.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gbdpikcfk.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gbscynbpv.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/griqfnfue.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gjxerpgtz.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gctrtbmtr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gsbnfzsjj.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gxnazvwpz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gkpmkhboc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gpqcdzaij.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gjhkrdjll.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gqsyrlnri.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/grkdgcksw.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/grylwadab.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/glnayphii.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gvqzpbaqx.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/grgkpkqkp.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gozggavqs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gqmztwktb.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gyrzcepuj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gvqsiludy.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gprtyevsg.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/glelrdqyy.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gdbyvdgwh.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gizciguyo.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gcdvsfuil.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/geezsjqgn.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/golpanzlp.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gdmrokamc.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gbcvkwrcn.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gnmlcqxst.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gavbvpsac.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gojscdycr.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gefamoqka.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gnhuhdoyw.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gbwvbkhml.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gnxifptos.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/guvuavymp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gzqgmuptx.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gfvxuggem.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gtgxzmnek.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gzgiaizne.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gxdiykwsg.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gecdntnzx.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gxnghnxih.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gxwatbecb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gxrbgierx.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gjfoomwsh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gxxfnrgrg.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/goxuvtehv.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gouxipsvg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqwtnubgo.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gjnpttftk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gittqjafd.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/galcvplrh.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gxcavxrfu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gotuczuzu.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gapsnluyd.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/glmyshlua.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gyedpmrgy.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gevsyaexh.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/ggkphmlii.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gooshejxy.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gjyrwskhp.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gqrucxkvv.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gavxujqlr.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gcykgzrpi.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/galljakzj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gpvvjsluu.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gubwgpsta.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gataytqet.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gclkuxzhv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gscjeooqx.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gxgkujwri.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gugxvvzte.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/glwwfgkqg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gesnaqraz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gjhspzphq.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gdnazhkcs.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gyjmjkija.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gdzzkndwe.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gaoqxajdm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gqyiizjcq.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gsxecxszq.sHtML


<!-- 参考信息 -->