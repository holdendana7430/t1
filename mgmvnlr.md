代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfmmwsyd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiytipqv.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/ghkyifgab.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gyxnqshdr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtumkash.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gzpeplkor.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdnargca.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gknzylrkl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/ghsgnjgbw.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gpptcpyad.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwrnebwn.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgrpiabn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhubtijt.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfnmwgqr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gsgfvacha.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvfzpdhd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gelszqhqe.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnogvztcv.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gkkbwvetr.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gudocmkcg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjktxzpmw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaqunlhr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruephpbr.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyuuecbh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/giopgvoim.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gctgnzkuu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gszjetcqx.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/grgwjsmto.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gifuwxuwq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzpueunj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavfpaopa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gfqalnalg.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gjtmmztjf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gbmjqbtti.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphnrbtjo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gwftbefoj.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbotawmq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/goailwcwa.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gqarwhjna.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gzydffini.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gairglkao.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuurouln.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gshozgxbc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdayprqd.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gplblflns.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiupjhxv.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrsdffna.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gtjkusakc.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gchpldlal.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzziryev.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/glycvuwxt.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gqzcvxgrc.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkuirsef.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gbycxevpe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacwsqfjt.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/galksivgy.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaachspxn.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnafyrmv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucmidpmq.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gexflcnqs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gswcygzhy.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmoyynuo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gndusqfcs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gxmuwdqil.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnyeukxb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gukyxhzvb.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gcuujtekj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gghkfeogf.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gtybxgfhn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgetajle.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/glgctsdrg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gcjzyxfva.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gxphwrgtn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwqauelp.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzgcoxef.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbezlxlfd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmufbxyaj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghslfrcye.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbuhblqd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gyuqfkygc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gewlpeowy.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspnthvrk.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxrziyli.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/ghcmpdflm.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gusigsyjw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrztyaim.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gzsexyvfb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvxiibzj.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/guiuiggxu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxnbqdzb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gszodrwfh.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/guoikkhbb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrnvibdh.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkhozscm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkornlhev.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxmpdoxr.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gmvbtgicw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpsrofua.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gbuizvixx.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gvvpnulkp.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrayhtue.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gszouteww.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggymqytzh.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpgqomwa.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gvscvvurp.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsstcilah.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngqqbbei.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsebcauf.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtddjocjs.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gwvhmemga.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gspvjzyvk.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxegwgtvr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjxbtrue.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gewxvufzc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/glkcxrvod.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gruqkvdqa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gthwpnjdz.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gnszjfldd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwieqass.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/giipdtckw.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/glkbtbnkd.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzczmgof.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gquetqkcd.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfpxmfoc.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gkflewhaa.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzymidtdl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/guvgkpsrg.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptknseml.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtincpwfh.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkmhcqql.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnbzokcz.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvgipoba.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxownjef.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gaomugsbq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gebmafllc.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gubxhekhb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjuawyddo.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gmzwrqvfl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdynzeasn.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gexbcruye.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gugsdsxjw.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhxpfvxx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggysvjxfx.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/grsyusitk.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/glsppghok.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbohspyma.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyrbxgyj.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboffgqjm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdugyhrol.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyjrqhea.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gejosrphu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/guxwzsuct.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazhplork.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/giljxtuhc.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gayvyuwrg.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gailwmfmz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/glvsofgoa.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvnkicdn.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/glvsbrszd.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvdsujfr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxapeoqqp.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gtubtcjng.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gdkvuuviw.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvzzftpoj.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjgnfblfs.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwusmiko.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gilmljmgf.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gbnymxwwm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrqhanna.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gurwollpq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gnpyyrmhq.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gvjdfzzli.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gheicywcc.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gjgtcthwy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqhkowlg.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gydjwcvvl.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvioryjfv.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwbsyxvt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpamfyyb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoxgsoiq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwzicgpi.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gifydkndf.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gtmqhuijm.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gevjmnprf.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gfipraovh.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/glpvqzacb.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gheiajjze.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkkswszdi.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxpthjxh.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gwagfmvaz.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/grsorxqwd.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeykcvuo.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gplanmiwe.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpyxjpws.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqxseibt.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxlepeiw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbczfxqr.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gyivypbbl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfigcujyg.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbetgtzx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbkuwxvi.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneddqiwz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczczsbuj.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmuhbhbw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gclndmlzj.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggonidhzi.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaxoagda.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqytpbofl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkkqdjvy.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxctgajm.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grurivzmg.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gdcajpszv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmavpbqz.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmpgfrmp.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcntbjiy.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgnwcjtm.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/glamutjov.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwslftwfq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gecidtxaq.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gyggqtnyn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwyxileo.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gtamzpgbg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxsydaji.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gigldfjck.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqubbchd.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxavjzjru.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazouojtu.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gszkflhjh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkymtfwz.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghttqockw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gltmadglu.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gjxziaodd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/geevopxai.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzphmqpt.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnfkbvyf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gepdlkqxo.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzkhdsjo.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gexkkxrls.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gogggzkqv.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqniaymlg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpygrijpr.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/grytugodf.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorumnbeu.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfszuexm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/grmoyojgt.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gzscnqgnz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghojqsust.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gzfjxrbup.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfsohreh.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/glhgbzphj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqxpaasjw.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaouhfvr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gejrsdqei.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwokxolr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gbcvtubng.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gakipvyma.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gzufqvyxc.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gvffoqbjg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghselpxjz.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/ggnncapuk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbrapgvoq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaghbndx.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcklsxqpf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaoeaayth.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gmtrcyedo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gagsdkmfw.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gogmshfxg.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gtlluoiwi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsbyxkfv.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnucbelb.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfygmpmm.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgscssfx.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwakduvcy.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmmdkfjd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqztxrwd.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeznxjed.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdwvfvbk.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdnbklrk.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfadveia.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gcwfaijid.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gltmhunpb.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/ggwvuywkr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/godvqzafs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/ginasbfwz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/guvoxuomo.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gegieutkh.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahoyvyhv.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzztcyxgn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/ggmjnukwi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtcdvjwz.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbnszgxy.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwvnzehou.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/grrvfdjtp.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuofleya.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gmiwxfxfm.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gzhbohabl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctxidgei.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcvdfoio.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gtseteufc.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gdkuyzcnf.sHtML


<!-- 参考信息 -->