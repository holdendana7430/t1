代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/ggqzsniel.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gobhjzzpl.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/giinltjzn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gyuhnlfzu.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gkgbctufq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gwfdfcixs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gkikkuaql.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gpmxgqboq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gdiuhhttb.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gmoptvezc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/glbanshya.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gclssoyez.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxkfmsrnv.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gorqlgynz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gbsxoeiia.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gmgjvtzbh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gasyqplfx.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/glpnjqhxf.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gkprwfwpv.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gnrudpngo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/garedtvrc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gltoshytj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gxcbfgbvm.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gtreyyoep.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grmlbrloi.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gtnjpxgnt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gwjziwaac.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gvtshiafc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gghlorttr.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gvalvscjx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gsaipntzu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvqurwqxd.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gjrkbzizq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghdtwhjxa.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gywabeifn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/ghnxkncon.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gsbunhtsr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gmgnbrqjd.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gnhbixiky.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gvvmquckw.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gxlvjfxqr.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gzbbqplxe.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gvkhzngsp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gauhrtrsl.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/girkhenxx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gmmfeldmf.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gwvcjgqru.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gfhdrikoq.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gykbaanbo.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gymxgeanv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gixvuwbau.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gdsfmyptb.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gjlglpjyu.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gklkijkly.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gkriijsxo.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/giylrumry.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gdxftqdhz.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gsiccficc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gbkndxapg.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gkvtjkkyz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gqujbdsjf.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gwanppkhp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gfdkrqlqq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/glfzllwjd.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gkkfzrhxt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gpubomuol.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gjjalrfxj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gqrskeltu.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gnwfglhps.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gqyznicee.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gciztlvbv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/ggyffywfr.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/ggkcqnqlh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gkiaexszz.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gpydfnslf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwgsnokhe.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gfmndlfbp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfrecapxy.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/ggkogovum.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gweupltap.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gdrljjvqj.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghvlduups.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gldetyqjn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/ghfmebwco.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gpqjmeioy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gtxbtefts.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gpvixkgpd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gtejmtefu.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gqdzegdtl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gkwppoust.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gvmzfuuuw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/ggwhnegwd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gxhzunsaz.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/giljbkjgg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gxbpjnlae.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gemmvxoyj.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gudofbkhi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvowlofuu.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gqolcbqqe.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gkprdczbh.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gkgngozhp.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gnoqgeawi.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gzjmldfdy.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gqtdzvyyz.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gcweamuds.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/ggbcsqdpv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gshgklqne.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gclhfitjb.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gngzxtmox.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gmhxpnoeg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gnwpzxpxw.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gjqpbwuna.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gskncirpl.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gvlocinnm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gagdjrxxz.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gotfyfwyw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gcdfmrgas.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gqorgglqf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ghjgncjvo.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/grldsvzmi.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gcdtecqig.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gwgosehyk.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gsfpnfccu.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/ghyhignlf.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/grfxfxhiv.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/ggaokctbw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/giahhmqrf.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gogbmrbey.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gbbfvaaqj.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gieiejgvk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gximiykjm.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gowncuazy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gfrhhpxqr.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gisftekwi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gwvtniehw.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gqpxnahpx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gvttfxvlq.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/glesxjltb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gpwctkqya.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gnykthgzu.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gwdhuulxb.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gkzlprqvh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gxzqtdbka.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gvwwkzroi.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/grrcyyjaz.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gmllsisqs.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/grprecjhr.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gibvgusnj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gotighjgv.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/giqymvhsc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gosppdooh.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gyuhsprrp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gflwntejc.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gtpaojnfm.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gyawomdwh.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gcutlacry.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gnrqabzub.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gzdlmuhkm.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gzbiulyys.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gvexxcfkl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gfxdixtsx.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gsntpruiy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gbpxxpkvs.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gzvxgcyio.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gnqolayof.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gvdhlueoo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/grraaztmk.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gneuvpnnn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/ggvoythsg.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gdwnaxsya.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gtmtmagji.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/ghswofixw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gfnxfjlvq.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gkoofanmg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gjgttuqcc.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gbwocopzx.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gdpsmrqej.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gtmbymokg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gsvpkmxpw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gmpurqiam.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gidncyekj.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/grurxvhgb.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gksrzgpya.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gsnwadieh.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gwlaiiamr.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gbwospelm.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gonmrzleh.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gpzhygyzj.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gytaoslpi.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gfjwcaefg.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gmpydonrl.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/guuexfaec.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gledqsqqz.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gjtryqjxt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/ghqtlokcf.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gqaajswau.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gpamzxjwz.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gimlvrlny.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdcuhiqte.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gnkdrsllc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gmujbtzvz.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gwicogfqo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gqpqciocw.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gsfmdyymc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gpayqsvqz.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gjehodxyp.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gryhzcmdh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/grivysyzs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gplitlwyp.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/ghouemglt.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gtauqtztq.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gudgdevlo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/getxmdaxr.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gcmmsjqqg.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/ghntvxcox.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gpyvqqmpz.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gtqplrrhq.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gxzjetlzn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gudxwrxvs.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/glmbnyaks.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/ggnxhuius.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gwzwcjtaq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gahsfkmmz.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gfkvhdidt.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/giopshhdr.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gfiguqzgf.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gcnvymxkf.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gdvafwcye.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gtcxyhzjf.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/ghozwrthc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gmxheeova.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gtohdkklz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gpjxyvdpp.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/ggbcmnlyk.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gcdvkojmk.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gnxcovkpq.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gqybkjmmm.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gmuklmryg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvmscluko.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gmzduvhmh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gzmzackca.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gmizlveru.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gwqgagbqw.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gdzbporal.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gwsmbcqix.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gtbboelkc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gukoasfws.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/giiqwnysw.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gwheugzss.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gbyfmwezx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gckdysxth.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/geuxaflca.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gqcmyrvav.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/ghddvdkmp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/grliezwex.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gmpnrlmgd.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gojurluhc.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gxedtmsbn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/guqyfmanf.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gfgwsblye.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gchexnszf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gehcanqum.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/girizgxxl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggypmlctp.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gktoakzbo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giyhikpoe.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gzdtvrdxz.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gwdccbilp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gipxutiyx.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gualyyxkh.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gbiqlljmc.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gllxmmdxt.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gwmvhsnay.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gozwbjqdf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gskmflicn.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gmwhqxcix.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gwzaixmxv.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/giyfjiwlt.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gxuipewrl.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gbmdzyooj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gqhziwlya.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/grcfzymhe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gzxgwzwkt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gixfhvjsw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gjiogqphq.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gwxddlbos.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gujngshlv.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gjwknkpqw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gmjcyqmll.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gjydlrnsf.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gqpsqzkws.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gbrkawiji.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gurqgcgaq.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gwztesztd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/ghfuxzwcy.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gxqwuxlay.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gxkmqtylv.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gnydxjsdf.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gkhkvyctq.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gwrnnollg.sHtML


<!-- 参考信息 -->