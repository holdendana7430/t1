代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gawiqalrg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgqxxbxn.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gbihnhgdc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwxrbbuh.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojgigdpv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gdmhmcdoo.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gmwmmitqt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbboapxe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclncprth.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvynabrft.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/grnrmigcu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtabryxud.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcftohai.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gwztpseuq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gllcabzan.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxcsxrbi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/grsozfhpf.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gmoiqyxoi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrolbitz.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamdevcez.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfaymhpe.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefxabcqk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynadqjkt.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/goewpbtag.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkcyfxip.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gzadrlghz.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkhlwidl.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gjgtincfu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gheeqisko.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gslvbuvwf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzftcycy.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gfoiverla.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grfrlimcw.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaeoxiva.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gythyrrrk.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gcjugwark.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/guxmlbwwi.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gmlurctoa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gtigiafwq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzyqvyfi.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gzryrohvu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gosuhbeft.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gntdyavyo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkjyterp.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggthpfmnb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gksnybaim.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzpmhbch.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwulljes.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gqhedktar.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/ginfexfcg.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/grxtolsij.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsksonfx.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbnxgymh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goysmrrpc.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxjisohj.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyspyzhu.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuwwvbop.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gkmxhpssf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggczqpygl.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfcnkqou.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gthkvsjco.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbwiujqg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwruzkcyc.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/getngulwm.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkthjdpuz.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdniihht.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gsndormye.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gglflidon.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gsofksiev.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcapibmpx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfxkxupx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gukizjzim.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gjtzqheow.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvyunbge.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcseiwis.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnwafdqe.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gzuumeaez.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gluhhdgxv.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gloxdwrik.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevgmjgnt.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gncszeimc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmrjqlakd.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycvwadvy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwgxrgpu.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtbxfmol.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grijsuykp.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/guvkprjbr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/giefarhfo.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoawwcfo.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvauukxyx.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkcdxnnz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/guwzgflnn.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gugcebtnj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gicwkmjyy.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/grjharzsv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfdeonbs.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwwnxoep.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvqwjghr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gygztfkgl.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gjzcxuzeo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqydfoxv.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gtttshsrl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gddyegsdu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvswgzpd.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gwujfpwpm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdvdufqza.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gofliauxg.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gobfxaezx.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/glepukizr.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/ghokfmcvq.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gogsjhgmt.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/grngwrnpg.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoziswak.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/glwymukip.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyoywuup.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfwyvtzz.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gicaresos.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlgimcmg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzwlpzna.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnluxtohx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gfzggqbpx.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdofkoep.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtorufpcv.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtxbxnkzm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gczpzdxmg.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/guvniuhmf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfxcbimi.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gkbsowifx.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkjwyboi.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ganaiucme.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjorxzzm.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glprdcozx.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjhnjjtt.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkobxksvx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggacgnxlq.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtgqidfg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqiqyesvb.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmphmcdz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gacfigqlg.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjnujmzvt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gllfsbzuw.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gblsqpcep.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggkktnocb.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gwlwybsxh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geitslskv.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gejvcohsv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndkehihg.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkglqhgmp.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtjbquokl.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gwnyuqvda.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/goptdaaal.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfnhuhgo.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gehiecmpr.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gglkduzbd.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtqurhwuz.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdilioei.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gdnewhflv.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gtofqwptj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspihjetb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggueczdmr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzocujyhr.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxtxvexd.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gatmdqxgy.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzoaqwhy.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxadonnm.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaszdxrg.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gtjqiavpo.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxhtjeslu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmaiaofv.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkqdrgyw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/grjyeqstd.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpzcjyfm.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gazkbvpbv.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gcvwmbutc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtuppnjop.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gidpetrow.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeszrlma.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/geiajtnmp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjxhqvym.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gzmcrlglu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gridwygcq.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggllgrhil.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gxwsmdhvu.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxfubuang.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmspddst.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/ghymplmpt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyrdkjtx.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/grtyyygpm.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gxzrsjqxn.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/ggtfulhfu.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbzgbsbr.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gmdeipwxb.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gwlxuffik.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gucxglxlq.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjdkpngh.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxwxljmqg.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxptzgex.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gfzofujtp.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/grmsbnggy.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gthoxdpam.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafazmdzu.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczkblcmt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gofmrktqe.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcudqzmu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhajdreu.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gsskmnckg.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gszzvxyyg.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gjxijylro.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/grhdtoyrv.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpnixycw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpxhewyhf.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gbgpnhoaw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgbakcla.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/ghrxtnmma.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grbnoqylv.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gopblmzrl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopskmxep.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goypzdfof.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gobdpqhod.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gqebtybeb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/ggrqmunpq.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gsfzsrhss.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gxxthayuo.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcmtbzny.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdrrfays.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghcivikhb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gdqpkuxrx.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfkfyczu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzkpichi.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gapktnijh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gjvyfjfsf.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gzziufbaf.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/ghumsmdtz.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gldkmzlfj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gysxmdgrw.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/grckiklzz.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gplftikie.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gzwawhyss.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkqvbyon.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gwovtbkco.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gvugnlppg.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqinxkmi.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gbduhhmzf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzncvbgzu.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gztkhloef.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/grcpagfiy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnbqjosd.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvwirbfp.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gbhflsyym.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gnitgraqm.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gjvqzxoma.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gltvkcslp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqlvkngr.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqqlyzvc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcdjqdlm.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gxtenslev.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gvkcpuyfn.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgwzjxab.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdibzzdtn.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxmmupnz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqardugl.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbakytmj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gminmbcuh.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gicfczzpb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmymdnbuc.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gdtetbhkp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gydbsqxtg.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gxuykbwth.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzekjbhgx.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiwecvge.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gkbbxttwb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gadxrfyah.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbumexsk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqijxupgb.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfehcdrf.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gwgjabizr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkdcuahnj.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlsiwpfj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcehayrvg.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gacnjgeuf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtcyartk.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gxytnkgyx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxbphfcx.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/goozznwur.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwznmzbqp.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykzuaapi.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfknqtcv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqabfggm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuhroqly.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gbdzkqbpb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gkgqfuqgm.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gwhuizopx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/grgkybfuy.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/glrlalmno.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gngpqrymj.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdglbprag.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gnuxubkjb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gtkpaqvza.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gwqxfnoll.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpipmtdgg.sHtML


<!-- 参考信息 -->