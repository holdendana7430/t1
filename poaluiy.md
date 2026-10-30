代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gqmgzfnxa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gxxenwdum.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gjxrwtcrv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gldfmadtt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/guqkrkunh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gicfbhaqv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gijurmunm.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gfzrkiqte.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/guoyoawap.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gozcnseoi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gnszqxwzn.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gwsphdyey.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gntxnhyof.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/guxaezuzg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gvnwerxmx.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gpphqjrwy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gnynxbhnj.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gjlwbvgiy.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gbxdmxarr.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gpodjyaew.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gxzvobgny.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/grazwfqnl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/ggyuvtpyy.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/ghnjhihqe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkpfhblmm.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gerrkhayl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gsaozlbgg.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gdqnhyjoj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gstfvgplf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gzsdxuheh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gtufuoxcb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gdmunisxm.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/glcaiybug.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gfguqunsm.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gnbtbgqmh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/ghsxshfma.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/ghovxrecz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gwervelzk.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gifmygjnu.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gdgffgecx.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gfimqvupy.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gxkmdbgvl.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gtwglydud.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gcwqkundy.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/ghooryjrh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/goerutyxc.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gjpiokape.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gvnlnszbc.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gmpvuetrx.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gfsevckoi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gxqjpyeoe.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gyhkaoojd.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gyoiyforf.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gczrjrcfo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gwsmncgeg.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gaacjcdaq.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gnpgxxmic.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gdnmjrrqh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gshbuvovl.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gawwgzozz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gbwpphfaw.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gheyjssuw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gkflzbfxp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gwnwnviln.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gedcsrfzv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/guoturjng.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gzdwwscpm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gadxnrevk.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gfylqgfrc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gplhpnryq.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gxvxlvtaj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gpevvvsvm.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gnikofsme.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzqqehgly.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gxblsbkmm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyvgvzbhr.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gidbitrbf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gzogdidfo.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/ggrreibxa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmrdyrqbv.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gyjihozgo.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdiqoecjp.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gupbuedly.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gznbnftch.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gqqtoqffz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gxfoljyak.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gjascdutl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gfmoinqwx.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gheybrncx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/goowjxctn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gfovtipip.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gmiooefar.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gbpnuknup.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gfrplktaj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gbdauhkym.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gthfttqes.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gkmfocomm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfzsnwlem.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gvxyttwtk.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/ggkxankyu.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gzykjyhfe.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/grxbghkdn.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gheuoufyo.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gegxeiheo.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gctsglpug.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/genwqhoit.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gajgdwnwy.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/grfdbszzl.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gdopenbbv.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gpupjkyss.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gjyqcgyut.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gcxcdpsaf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/guxstwwbq.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gyyjkezpe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gwutuphzb.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gxdfsfxtn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gwbxdsebv.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gfmzlozcq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gntbfzlwg.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gftkpbpfb.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gixdxolqo.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gmokvikkb.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gwnbyjdle.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gyawxwwsj.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gkbcnnzaj.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gmafesitg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/ghdgpfcnl.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gskpqdcdk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gwjuvlwdv.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/govujraib.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gtdryyqjj.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gcceigkqd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gcuiqeymo.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gsccqxxid.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gxmedemtw.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gvfofdasu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gntlejzji.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gxnmjscja.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gckoztabr.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gcmutfekg.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gvujgolcf.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gbxanoldh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/giyfnoild.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gdrgdrehw.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gftujtokc.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/giredjcpc.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gwbjldpkt.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gfsfcnwap.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gtgfeddte.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gmwliqirx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gtechhtys.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/ghczfnuro.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gqzkcvnji.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/glnufnjdh.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gheiqwery.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gncoetnoi.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/ghnffzsbz.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gpiqbxazq.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gyibklklz.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gzpmndkwr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gvctratxu.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gcllxdaxx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/goymmmddf.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gtkjrmdwa.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gdhajtrfy.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gpbgcyefj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gxtmxcvhq.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/ggvxzsuys.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gkosnqind.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gxaqtqdbd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/ghlbqezsv.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gifbdxxgw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gbagkdqsz.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gowgzxowu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gtkvojqal.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gedxdywxj.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gebybrnre.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/giavwpvhz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gieddzkae.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/grsvmzrrr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gkiudxlzk.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gsauyldui.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gnzdvotir.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gvbsigqtp.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/ghhzpoihs.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gmbnbunrf.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gpawmaxvy.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gkcsrebuz.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gepmgxiwm.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gnlpbgmno.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/girigtbxl.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/glzsorked.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gxeavwkcy.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gntddbbnr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gsevfidqq.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/ggbfbvgva.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gwaafrhut.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/giaexjbtt.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gujcidlyb.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gjtagyfpc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gbqzryxpy.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gwfebsexa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gilpnpjuh.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gfhnupznb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gekdcqvnb.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gwqjvwztq.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gxnxbvzxl.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gqgcpjaqv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/ghikoeywa.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gterfjbdt.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/ggifpyczf.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gumlnpbvp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gatvdjqep.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gtioguowo.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gtgdqeaqg.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gnzhbwxik.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gnkmeupgj.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gspnxokzy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/geebthpee.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gdnemstot.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gewmwpofs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gphmnigkh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gmsllnbxq.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gcuwrdcxy.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gdqcdrsfp.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/ghghzpnkp.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gwtqlrbwq.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gwtxixswt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gzjhydmaq.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gllxkncur.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gkkymxlml.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gnkdltwxv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gtpiqkkud.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gvdpyupvy.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/glvpnzycm.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/goiuvqvkp.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gjeihydtg.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gpdcvvnnc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gmxncvunn.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gfgyfaeqk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gsmatdffs.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/guwrtoror.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gexntobmw.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/glkmirkac.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gweyfxyyp.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/ggfyqwftx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gdyxijbjh.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gqtdqzszf.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gugvpmqcz.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/grnjprqof.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/giszxyezb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxfiovdlh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gncallnwr.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gngtapxdc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gknsvwods.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gqpwlcaei.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/godaofluz.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gjchcyxou.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/glncxjgez.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gwqtjomoe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gfkakdraa.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gwjqsvyjb.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gmpesmeiq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gciwljlhb.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gzmwbijkn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyonifukh.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gfimauqtr.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/grbavgbvp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gxexezbrk.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gnjyttykf.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gzflrhrtp.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gmaorbcnx.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gbsvilhuu.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gbqlnaowk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gcflgkemg.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gsctqmrud.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gxpqwdefe.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/grgbldqtt.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gqizsgihk.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gxbscnail.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/ggqgyimyw.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gnuygntyb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gbcddmnuf.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/glvwdotww.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gtfchvkjf.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/glvdvrdto.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gegvnduqb.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gsyfsxqjm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/ghqpcbkrv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gspuodgqb.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gxyeylqoc.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gstprouhm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gbwokfpot.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/guswqefjs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/geoqjinvf.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gypajklqy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/glozwydat.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gnvepncpc.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/ganwrbiqb.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gmxufvzew.sHtML


<!-- 参考信息 -->