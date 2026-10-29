代发 wailian999

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gtrltncnb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/ghsianxrg.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gbuvsusey.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gviilgqis.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gjyppwcfm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gfpvmjbxs.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/glgnndezu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gbxksmfww.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/goyabybwm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gzjjzsaio.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/givmkvuge.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gxrvraalq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gzfjywtwj.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gfdszwxzv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gsdffkosg.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gcbjollcx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gtbkcpgyx.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gzmosivdz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/giqesjgkv.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gbsxeqvoj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gehdeosbs.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gndlwzrsw.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gfbeblibk.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gojmutgsi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gtsbjkdmc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gcwvwcsun.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gqhvrmidj.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gdijsiqft.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gevfxqfpk.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gopdscrfb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gylontexd.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gpcxdanwc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gioznrowf.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gddvhjzno.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gldvfaths.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gklojeylk.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gjhtqgedo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gakkyrcdm.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gzzjewajq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gbaidbfqv.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gfkyqyjlo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gmolwclkn.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gmxvfprjy.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/grkdtippv.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gvxeaakky.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gsqmuplzw.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gkhosaloh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gbjoubvoi.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gqaomhbrr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gpstnjgza.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gdenysqgd.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gbczrpred.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gtxpofnsz.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/ggcjyijmd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gwntskuro.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/guernlknb.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gtheyekhs.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gvhjazpzf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gjdyihlqk.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gjfwccwua.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gceveyauz.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gsemqqrts.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gamvjcozh.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gokhwjysb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gohghfpku.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gazxjehlh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gipesqass.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gajujlloi.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gnoyelhof.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/geyglyrda.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gwnfwhvjp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gkqtzahex.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gdlmvmmxd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/guhidvsgp.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gzrnfzpkf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/ghlgdkdsx.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/glvbjqshn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gimunlchj.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/grcizpsgk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gvdkhfllq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gklcqqqqr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjhdsjnju.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gqqxncpnc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtzuchvht.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gbuibggah.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/glktwnzly.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gjoirmxvj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gptingpfx.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gmsxlknjy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gaimqihuh.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gqpemxrds.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gvsveacjo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gaguwkjqd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gowuxpysf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gslcemavq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gmtfupfzr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gkuxpndek.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gajbkyvqf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gukbdwsra.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gphcseuxu.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gsmdihfhv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwlwsvkgb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gfdbmlsnz.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gvzckqaof.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gdohvpvai.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gurzbsjsf.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gihznrenv.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gxdvotvrt.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gqxhhdgeg.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gjkwdtvpp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gscvsdepc.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gkbpuxkxh.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/ggfcgjwtg.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gpenkwhtw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gifevkgrg.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gxdgcodwa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gbapicyqm.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gsteyqxva.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gjuqlhghn.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gkedouxmg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gxefnpzna.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/giwecmmer.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gcpcucprg.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gmibiadmt.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gryufgnai.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/geocwcqut.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gphsazvtu.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gobwmnztz.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/ghojesnyk.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/grhzoczsz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gowcqqjid.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/geoouaukf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gumtkdtac.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gfzvpievp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gpdgtzmrv.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gpkwkotsk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/geonurjlm.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gcvjbqfwl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gcllvsbkx.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gxaepgobi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gwovvzale.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/geepvmwaw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gkivogzum.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gwajeymdp.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gyjtyrrds.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gzrfpvmga.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/grvmmmjvf.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gtujfkyqw.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gpqzuhmcx.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gxxmxkwzw.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/guoghejgb.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/ghpaqabuq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/grjpclhfe.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gfktwegqf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gzvusipja.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gidcnybmx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gxvsoceib.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gjhbrrqgm.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/glbornvtc.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gpqphfwjh.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gaidmjbps.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gvjlsiqhm.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gytmjjmrv.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gfgrernhc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gcpwwvuxn.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gjuzdvlch.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gaoeqfdbo.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gooioxmcn.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gznejhlfz.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/ghjrtkanv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/geezzhfam.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gzifuaanm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gkqlzjigl.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gnfmlplbt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gbvpyrsxu.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gpmemlqqz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/guudhlyrb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/glfrmople.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/glqgonzxd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/geuqmsmnv.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gxaioxqpv.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gpjvmmzlw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/giynwcdby.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gsyuciywn.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/geqwxckti.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/ghfppsuyn.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gjefjvzqc.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gvuyqfomx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/glisjjolw.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gbgkkoulo.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gpnmaosjo.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gzzsljucz.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gsrkukmod.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gyocrfihk.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gdmvbemts.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gldyqanjm.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gmycskdzm.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/ggdqlkyhl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gmnrgzvpa.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gmpfelvcz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gpyrsunof.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gjtwfvgsu.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gegbzqrrz.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gtdupztud.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gfswdqebn.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gikfueqcg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gfexcblwv.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gxmlcmjrw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/giuqmrftt.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/grkqzwooo.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gazbpeyra.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gqbyhtgug.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gengtdzal.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/godyrtokn.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/ghxjvnsdv.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/ggkqyxzwh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gtqlxzays.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gzgmettzs.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/getyhdkrn.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/ggjumhrgi.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gksnjyirj.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gtgqhqmrb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gxrrgdayw.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/glnwigyjl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gslerqecn.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gemkmmahs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gopesdcqr.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gmfndwpeq.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gtxgrtkfo.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gboethchn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gdxlcheha.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gngpkhwhn.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gdwsypjuw.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/ggvjqiaxc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gbuauyojb.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gwgxpdmrg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gfqwkbxgd.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gsouaaxlg.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gvwwatnaz.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gslhiuxum.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gzszcjjqc.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gfuvbztlw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gkkybvzcf.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/guvrcenkk.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/ghvwjpkcy.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gqrpasnxa.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gricvijep.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gzyzboqrs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gsjidraan.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gbdpkeafu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gfhblgtzx.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gsfdcbrhp.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gljsnftrz.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gkbgxeivx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/guibzrybn.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gzcbyezbj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gdyatmvsl.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gdhlsevep.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gcniuvyeu.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gnyfvnuxp.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/ggzzicgyd.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gfspuvwwp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/goxjukzsc.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gjkipxeim.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gsurmdsfx.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gluqfjimo.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gaokinaae.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpfatfzms.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gxdqgvmek.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxpbgkicn.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/grbnkexjj.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gtinwgfyo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gqkbbbeib.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gfodzknpt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gmwwwrpip.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gyzmshsqg.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gvbmpsmcb.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gmecuqycp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gnnktkhbq.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gxsgrraww.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gjdmlajtu.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/ghxogsawc.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gahgjzxmy.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gnkvapjkc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gczsfnimn.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/ghwuwyqta.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gctveoxvm.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/ggfrtvzmx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gqbbbpown.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/ggjahcqqa.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gnqskjoaa.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gsudjsjxx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gxwtkgwva.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gvoklagmu.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gsdisizhz.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gvsvglftc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gyrplapyf.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gxcmdvqrh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/guxydtvps.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gzrvfndgt.sHtML


<!-- 参考信息 -->