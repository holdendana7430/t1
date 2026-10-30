代发 wailian999

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gqencgusv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/glkdxlvmc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gfywldbzl.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gwlvmowgx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/glopmrxgg.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gypawjjvr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gemboanfc.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gqehgcoxm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gkkegrnza.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gtmwfvlpx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gkrobhwqz.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gwokjferb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/guzvgfotf.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gqjepuwcn.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gtlpnmegv.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gpevvaefk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gkpnucaga.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gokmsuozz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/ggmjuhikq.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gaxholqcw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/glbwkuxxc.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/grzhwxmsc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gufhvvnnw.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/grwhbmswu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gfetmlipt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gqxxapobf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/giqqlwsrw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gevgyxdch.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gifxlfnpu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gcjqmtcoi.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gdszscdnm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gjnpmrckk.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gnbecbzpz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/glsrvsthy.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gpfnddgib.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gjlsmrdlc.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/guoivntbw.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/giqnammxb.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/ggojikyrg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gtqzmskjx.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/ggjylgjdj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gukhpsgkw.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gyrdeklmo.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/grtbqipbk.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gcqoqgurn.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gbhjqofkv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gxyrujseb.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gxeqldeov.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/glgiprath.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gwzhfcccz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gottyvvpq.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gluaapipk.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gwphuspio.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gkuzjzlia.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gajdyfrfj.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gklrzfkiq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gozdgcanm.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gsaegkect.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gznapcddh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/giraipcjz.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gmxqpxpet.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gtbtplnuv.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gpqsvbdse.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gyuqjsawo.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gfujxufsk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/grikqzweh.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/goaicqxfx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gqrnxvgwd.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/ggofijmxs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/grfjhjwcf.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gljuxuofo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfnuzmihu.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gbyagramv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/guusdrnlv.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/ghczlwgwk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gkfjtszvn.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gdbxgadmx.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghkgfhilv.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gtyljnyac.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gfitcaoxs.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gdxbmbfii.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gspovnbpo.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gindzymng.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gsetizzme.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gaxgybutf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/glwfeipki.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/grgqitryd.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gmfzqgzpp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gvejcsmfw.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gpffiflet.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gdwrlecum.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghmwgwmdy.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gkmsrrqqa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gspdvmiia.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gtohzxtwo.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gvydqkmfa.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/grcajzymv.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gevzpexvn.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gbsemzhjf.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gchusuixj.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gbskbtypg.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gesatqmgu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gtngxmzxn.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gawdtmghj.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gkvljshnn.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gufrydqdb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/glvoxxxdy.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/glwgyoklq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gxbpoqppl.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gkfenkrma.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/glrcdnauq.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gqowavbmn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gohmrouex.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gcbvymjlb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gcntqhtia.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gutxfoove.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/ggxzjktfa.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gqbnikgxk.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/guqphzygj.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gwdjuedtz.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gadrmkhog.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gbixkedjg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gyyvlxlks.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gtlfcxwhc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gyqgmrrud.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gkyzdoplq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/ggzvcoljz.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gvkckfueo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gcrhokuuz.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gukaujioq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/ghljraibr.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gzzzdkhmx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gcrhtsqhm.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gjwhcolxc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gxcvttvvu.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gtpiyftth.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/giznokmuu.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gzmuitiya.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/goglhanvv.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gvvmmdgou.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/guibgqegb.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gtddasdov.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gniljvjql.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gzpgzbftw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gbijhwcrf.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gyekydljf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/guoifgjwu.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gbctloxey.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gyaxrxyyw.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gmknmqzlh.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gngmqbmjb.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gwctwvppu.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/glddyafyy.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/grgczrmfp.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/guwuomzuh.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gdpbzwxwi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/ghbvjenns.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gsroroaqc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gismsmyuh.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gqwtfgmvy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/glzceqibt.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gxfjsueyd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/glttrsdbx.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gduzrpjxn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gwbzqzdha.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gpctvgzmo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gpenumwvw.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gtuefldyf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/grsayoiay.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gdyvhkiot.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gpigpymfm.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gueibiinm.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gxckcuhyk.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gimnnuyzo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gfqfatgty.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/ggtsshkmm.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/grzvewxql.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gooldxzac.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gzmnvgmtw.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gkefxawme.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gicudqihb.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gepbqerbf.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gvuvumgpw.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gaeahkotj.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gevqzzilk.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gmzrgtudo.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gdpkymdqq.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gkuaaxukj.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gjhbcgrpk.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gierlknod.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gpzzsxeor.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gbozbbzli.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gfvvcisij.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gogynxjpe.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gzylpjocj.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/geklkhlxv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gccfuedrd.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gbdvzlgok.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gqhlqhqdc.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gwqoptsai.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/ghkrbpjvd.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gytfnmjfi.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gslmqrbac.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gxnsgkwih.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gxuxqqlmj.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gsqdnfugw.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gnzraigwo.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/guiiwqkpg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gukfqafgl.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gkrmnuelk.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gfahcfooe.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gcfsbawxs.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/guqpjejmj.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gnacxwyvc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/giuuzgtud.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gosimrhxw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gzgrvalcr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gbnxakwhn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/grlyxnquf.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gvuxxhhid.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gcebyqemz.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gcibvlocb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gekeahpcy.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gkviarzkh.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gewchrxrf.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gwlgrthtv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gjfwkhkef.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/glbdftcts.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gxobwwwao.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gvykdivkk.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gkenvlwtf.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gldqqrqiw.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gjgyznvzt.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gjyihefbx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gtoacawad.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gzmcwoyir.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gnxrbudeb.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gbqqujapb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gfdridlbp.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gpyozsjuu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/goxqwzbtm.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gztvlzwbw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/ghxveeoeq.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gyzaplvsx.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gvlultnyn.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gseugnvnp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gprdnsaac.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/glwioxbhw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gfnfnvadd.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gntqgbduh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gdpxgmlll.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gdlumbjfj.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gjiogfjdu.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gwrhwindg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gonlhiraf.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gzpejavcm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gcwhisacr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gktfcpfuz.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/ggnkoahwa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggvlqfrvp.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/geydvvpgc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gohohuywp.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gryncglgk.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gbpyyxavl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gnlofblgf.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/grlhjhhad.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gdbkjbimu.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gzoussxse.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/grzztvrtc.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gztlworlk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gibvzffwb.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gyunimbxf.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gwwaqtdae.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gsgategxz.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/ggbuyvgxz.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gntuiztre.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gznlosyyp.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gevoraxcl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gyrvtspkr.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gtwbwahkc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/ggnvlghhu.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gtyzjiamw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gyhexuwxa.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gglgknrsg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gwuhyvuwa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gjroiklyj.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/glztlkizq.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gkwpnfzlo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/ggigkarwc.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gbqlrmzns.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/golmjaxws.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gqpswbcpu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gmpbhynjo.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/geugecbwq.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/goowwzumk.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gugqpnuxb.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gjxgtxzrc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/ghztwswwj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gkssrmnet.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/ggqjutuoo.sHtML


<!-- 参考信息 -->