代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/getzyvxeo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxkmjzdj.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvyxrpjk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpsembcw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/geiixmllk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gzeuvcgpr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gntimnuua.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/ggdhyrkib.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvrfafig.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gdryqullo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/grhdlidfi.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gqdhifmnd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gzikmtbpn.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/guakhlkmm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gxsnkrcmk.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gncxsddyx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gedrkwrnd.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gzeqoxnzq.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdztmtuej.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gjkobjdzl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gxnojgkxs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeepodup.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gdekrabqe.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gcwryxvcn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxqqtxzdr.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzblhtln.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmohlbecm.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuritjnn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/givwokhta.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gtepxyspq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gftfltyku.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxnmezmv.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gkvstnayj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpuxgocn.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gceznties.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckohpsio.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/ggnmlydqr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbrcclxh.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrrugoit.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrgodbfw.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gkaylrutg.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxiegeof.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gtlblqnft.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlvloxet.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbvzsvcf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gmhnygkxx.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gimxxlfhs.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhicccdm.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdpzjyix.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gvuauccbu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gzprsgrvv.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gmkwmxlnk.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gemztvmrk.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxdyfndy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gmrziyemp.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfkwngea.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glekgcbyc.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/giioajsgk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gndyarlmo.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpywhcmz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgeqiqbi.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxiactlz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ghcoqejdw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckonncwn.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gcxcxurvg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcdjrchm.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcennqwqw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjpviofa.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxqgghsx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gwswhgxcw.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gejmchrdp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuwbrega.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkfifapr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gchtyfnrm.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/giwrevlya.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdevdytj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gqiwwiezj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzcgnzuv.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gklrblgkb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnbtxjpa.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbnqgjce.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggysxwffv.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/galzppffu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gyvkmcnrl.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjeugyvz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvrboxyc.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwncfpfdh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gdllqaakd.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaknaaom.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaukfwzrb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtokhlhta.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gviosadpa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gulnpxwrj.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmlxxshd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gejwtxjib.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfpkompo.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gidfslzmy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzotjdlew.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gguabqioa.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/goyixoamx.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gebonmsjy.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqneibra.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gskguzrsd.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtqoynlvw.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gacbrlupo.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gctjektxw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzgdonpq.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/grfkuizde.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggujodjhk.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/grazqmygf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcngkvlxl.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggztskadi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gkktrmaxk.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gigmprsmc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gkseildbx.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtnajpur.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzuqrpwe.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/geelfvmxn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpesingt.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/grvqkquez.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gzjhhvitq.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gftriwxsh.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/glshgkqnp.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gwymygarr.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxbsrsin.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyqtcbza.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehscjrgx.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxatorqz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdevqgskl.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqgmnndi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpzvktgz.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxzckiax.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpxluavkm.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gvlkrpxrn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcijxktbf.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gqvtgvhmx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/geqfrsyhe.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/ghueevlwa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwjspficf.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoxqqibc.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrzbdhef.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gixartdyn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkxrmaozg.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfjqqzly.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdswfmcei.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gflsixyhp.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/girwxjuoy.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrzffhmp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gaivjcrwm.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/glkhvuyyf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtbcsvjs.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gtohaxrlf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gijoboqef.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guebmstgi.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gswwxvlgd.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gkfzgbgnm.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadchqxac.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/geprdpdyq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcinqlmu.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcychdqn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/goqfcnjnq.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/grqlvdqfa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwagpezxf.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwasjrkqv.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjcxtbpfr.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gorutntoc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geiguskfd.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/goceboqbh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/giwqbfwsb.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gzcnzmhry.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxqxbjej.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gdjoxvrxc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxtlmfzj.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctafvxtk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqrmvtrc.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/galextull.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmovqwnaf.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gnhvfobjb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaoaipbk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwryckwht.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gwkclflag.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwjjgwycw.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/grnyshepq.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gmnskhfkf.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gvboytwgg.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/ghewgyihz.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcitbizqa.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyitsawgn.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaimegzs.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxsumzcs.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwjodrzy.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveebtnfm.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gxamtyyur.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gttaorhkt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gfowyzuku.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjypxaxp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcugfmryk.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gxebkfszs.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwettuyqv.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaknhwhaw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmgbceuw.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goonblfph.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfwksbxb.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxapexane.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gsuahxabv.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gqkpyokdc.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtimfehl.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gdghmrcjr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gbnjqjgjr.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpnpunce.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyviqlwun.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gdqskqmuq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gzpjntguh.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnakxvtd.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gdmycxgra.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gphslxgrn.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gidkfxkpr.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiqhjrgk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gsgnuvjxl.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuiyptsm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrmphlii.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxlvnkfx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/girgfysam.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbnrqfru.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwjuaueq.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxdtbezt.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/givfzamkd.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiqbodep.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxklchvp.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gfalsbvgd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/ggukttnhh.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqsyoedv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypvvzngm.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gttuvlosk.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gutbhevdp.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcgslumg.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gzdsnpnld.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqqaasje.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmamwygdz.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqxfhnxe.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehmykvod.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gphmbvciu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gaekaztnu.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldlyapkl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gimwffvev.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gtlnrjoks.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdnaksoxs.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gdfflsgpj.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gawpczgod.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebrnhpoq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnotyswgp.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gfxxfpnar.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxitlsjfh.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gedylnmfx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gatvglzrt.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gcljmedff.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gabzdcfwx.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnlagmfp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gplxmzxiw.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gsxygatzk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/glzfenthy.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gzryqpibq.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gilfdxjxp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwausuvg.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujlfjocv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdofowtfj.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxwbfoyt.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galndwsve.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gepnczlbg.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdfvejen.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiuratts.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gohihbyed.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/ghyjcdpgf.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/guzjsxzmo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqpgsjfb.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gkliyjfxq.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/guntkdgcs.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlrbcbkf.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gvrmtyuqy.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzfxftgq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfhhsxmh.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gxapmzabk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvnywbkq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmlsdxpk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/ghnodlyek.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpzuokgo.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gzscyqqem.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtowrili.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gkungusks.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfryneimj.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gucoqfqao.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdwkemvbk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gwfeoeiqy.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gscathpdk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmspnmyrw.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gyauomvxp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gamrkpeap.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/genxmwnxf.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gwiuzaola.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsvzaxig.sHtML


<!-- 参考信息 -->