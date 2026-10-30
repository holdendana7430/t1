代发 wailian999

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrsnjfyk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqhycmdj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gcljphhpc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxixdkxa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabecsgqj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gjnryhnoh.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdgvincz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqulilcsb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gawmylnlz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbyyavjt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjchgtzk.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/grlztcvea.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gxogpmocz.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvnrypsm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtvyeqxd.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/guawnoboi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvaqrhqt.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gshnupcqm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfginlfg.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/ghhysisiw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/goasrxgln.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gwziwzscp.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/galumokmx.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsdrzari.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyriwfal.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gvfvfppdi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gyolfppnl.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwckhdde.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggphjtmmb.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/grpnwjwjg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gdvfrojey.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzmpeppi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gusrswxhu.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gcixpcleb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gckglpzdg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsttejrtc.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlfrsqnz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gcdpttqaa.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkayvpbd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/ggeiufkko.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrrtkaxg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gjeqarhrc.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzloctefm.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgvlbdzg.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gmfklnbeq.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzdiojhq.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gwpumolje.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupywaqhr.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gogynbnyu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiptmoim.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihkafyqw.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gptgjcemr.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gontlpcza.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gxphejkyp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gvlbvzzfl.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gyeivcvsn.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjuzsxcd.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmxwuqiq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnffurin.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gxlrkmpsj.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjneqvzeu.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gzsvpwfcg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxovcdgpj.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzktbqtnw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/grrogjiiw.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/guexgacpn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gvpdmrxrh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/garpwhgwz.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gtlipurom.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvpnljbf.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gwofstofz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/goqthrkca.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gdrugxyyk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gvslifmyw.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/getaxlbkc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gchtlmjcl.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/glgppgoaf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzqhoxttw.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpereaxoj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gytuicyui.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybhdffub.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzzrgngof.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkfbxqvj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfclqnjgn.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/glhjkylks.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghmjckbqc.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcgupzbj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gznadzdno.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gtueekjmh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gohonhccb.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gipqkirjs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpjjgaup.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfkylupb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gqednqfah.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqdjklqs.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxrrrpvn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/garorubmn.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtsevqik.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmhhuzfu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gomlkryct.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/grmtdgkux.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmapoglke.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgjthadl.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsapyoozw.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/ghckvaawx.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gtiupxynb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/glgzihsrj.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkucyhnot.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gyputwobb.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gadbqxjnc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwytrlyqu.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gvywhjfxg.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhhiwrxm.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gaqbzqmcl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gihlfxdpx.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwobmkww.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gwidawwsh.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gcamkytuq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gswrxjtqk.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrikvjky.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ghexdfkre.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzoxdmzc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoqatksu.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeuzlznh.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjxpnlyt.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gggtxqqpq.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gckhbyees.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gayzgjawe.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcppfyqtv.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmscfwowo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiuzcklq.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gciwlzeoh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyxekblip.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gfdfqtztx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glgetlwvb.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfwprmyn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjmjgbcm.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwojzhgdb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwukxlsz.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekwdzmci.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdxshpff.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghavrimsb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjogrpyk.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gauycupsw.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gonkburqn.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbkxicpy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsndqlau.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/geexvouqa.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzxghnnu.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwxooktx.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbfmnrpu.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/grgjjcxmv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyrdfksl.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gvqpeqnbo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gngjfmhyb.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gecnolkae.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkruedtpw.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gkckcvnzo.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gilvdruxl.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwshupdx.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmcwibym.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gbykxohko.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmlpniuv.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gervpqhyj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjzvmkrd.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gvjwmnlsq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gowvkchky.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjjctjdvs.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbnfoorqi.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gsqkujgsj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giowhcgxu.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gusoexqdw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoeclupy.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyttdwaul.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/geakwpjet.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gkirfxvzh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gdhvwjjld.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gbhrnhdmi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gwugebkzt.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggswzuvrm.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gyeogpobf.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gerloabik.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvdxqwrl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcgyjxxx.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvjwtahn.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gjfavcmbu.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gvloynsmj.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gpswlrbyt.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqozicis.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedbivphb.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/guhcutlnh.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glxnschag.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvlhgsnh.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkrdeurg.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/ghchvewzn.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gldhxqifw.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwcsdelu.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gevddhjsj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gkspjxmna.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gndbttucs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gscaqdgzd.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gadfmmkuu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvwdhpjy.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzggifcgg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gqzbfoudh.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gbbjjgdqt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gujwbvkmx.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gfygcyqoi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gctonylbc.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdncbvwsx.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/giumfmqkq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gavglthfd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gnhbxpqvt.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuwkssry.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glaqfenzj.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gzncptwve.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycewikuy.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjrzrlqk.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gokazfhmk.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/guxygnsir.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdjqqoke.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmdjzlcxg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/grvzyyizq.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdfcigwq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gxwsyyigq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcephijxh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/ghdbzqigs.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/grsoadrqe.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gxufeuzua.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeucbhng.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gcerdhfou.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxgtdcps.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gmiptbyps.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzliiltx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhskqozr.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwrnlkrl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/geiyrifwu.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrneyskf.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrdwoosi.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsdregiz.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gfhctdowj.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gztwdtxfu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcwglfpu.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdcofvju.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gvdljmhip.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjuuqcqz.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlbipjxh.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gprrketyj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gaatstixo.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gmtiixuch.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnuwhoukc.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjzjxuxy.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gxgmoivhu.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gruekyydy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpkjshum.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzavlkpuo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gjtgiutik.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlmwyeob.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoirgpxz.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfpoavze.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepstdxlx.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gxgcgznsi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoqikazz.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxjibwzh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmfworlvx.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gqnwhinae.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geszpmatx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmscmafan.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gvwyndwch.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtvrqnshp.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbbglfxw.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gumtyhswe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaggtpgoj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggexkmwpq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnjihepf.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gmfyjpjel.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdycuvgn.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gybahnxvb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gxjaovzjf.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ghdyakjfq.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gsacyupji.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/glnzuktzf.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gazsihkma.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqxifvtx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfefodps.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gwauxenuk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gpcigjytn.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gymruhukc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gsiphacxi.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxpnbsrr.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfttyefju.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gaemwpzoi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmgnorat.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvexvfpwr.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gigwoxqgs.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxvzxhyyy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjodmbuw.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gbwaxqvzz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gllyhehgb.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/grlbiphin.sHtML


<!-- 参考信息 -->