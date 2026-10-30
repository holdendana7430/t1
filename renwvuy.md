代发 wailian999

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/ggdpsxpfr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gvkjvgpbo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gqnbiscvq.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gtbnpjxmq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gmbzuurbq.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/givwhqvcs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gmqiuvlip.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gpocukdzg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gdeidgqxr.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gtkgioglo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gtpohmctr.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gqdrtpcfs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gqlbkstkj.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gomajxmjy.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gshvdvsxq.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/goouujkxi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gzchynlwg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gudsgsmhe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/guptqqacs.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/giwvimsnt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcirkkosh.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/glwdzemcz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gzawyznvo.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gunjmtngi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gyifshxaf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gsfuuaqss.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gcekzyxns.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gcshwmwkc.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gqmqzvkgd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ghsuqtgdk.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gcdvrvwcq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gervmyvna.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gifnlvfod.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gywfiilbm.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gupzuodfl.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gidsmihcl.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gztqknenr.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gvgtwamyt.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gipdunpcr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gynczsmxw.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/ghrhubuoa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/giszlfrbf.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gxnopepxk.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/ggjckmitv.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gehxtylnz.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gqqmnjtio.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gjhbdgboz.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gsmoaipxj.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gqiubgenl.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gyeotfbup.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/grhsqmhpd.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gqlvbrobn.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/ggkfznmzm.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gxyydlpae.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gxmpklxbu.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gxdybszxw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gfrshgtli.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gowscrmrf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gduqxrhgp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gwwkcetxb.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gzknpyxav.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gfkcrdgrp.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gyyeqnwxw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gnesypiep.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gnqpbvlcr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gzkujievu.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/golmmccai.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/ghvdcivkl.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gfzkkwcza.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/guwgltxko.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gocyybpfr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtpdqosmt.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/grpzliptx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gygeayulg.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gfkgafkng.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/ghrercldq.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gqfibvwrq.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqfbnihtl.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/grtlanhlo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gfrmhuueg.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gstckvftr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gvvysrdvs.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gmtpuyehb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gnlutxizi.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gtcrdwpiu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/ghupkeqyn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggntonfdj.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gdyrjmkgo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gjabqdnub.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gzxhxgtyp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/ghhitfeye.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqrpiqkxq.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gtwbneqvc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gblkhyuhi.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gofayjmqq.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gcdfpxwhk.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gjztxggwd.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/geweelynx.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gzcaihkjv.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gvcfshpyq.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gozioqtfe.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gqkewatox.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/geymlrqaq.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gxvqehvys.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/ghfsebwkr.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/giqgyyhln.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gmmhrxpvf.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gfeytrulc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/ggbxruvoa.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gvjnrdjdd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gxizzfpzv.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gluvvybvn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gjtgjjxcz.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gklwztfmj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gfgnjlgem.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/ghxfczyrl.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/goiowenmt.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gtgwyynsk.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/geihspxzj.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/giqdzimpg.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gyucrshyb.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gsbpimoyo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gvversfyd.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/grzkggveb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gyflxladv.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gnzeaeevo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gizgyagsu.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gbzpdxbiv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gpttdycwi.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/grodxfgqm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gougamnyo.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/grrxfcqqv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gdczhedzl.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gclhdinxm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gcddofmct.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gwjkxbzdq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gcyayouzm.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gromzlsbr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gcoelrccc.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gjwqbqxev.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gikgngtuk.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gjxdikchx.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gzllevijj.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gukyblymn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/ggdgjwqby.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gmgnhqotp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gzvdkghcp.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gduzcejvs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gdukbtvld.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/ghxorqtxs.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gompxlvbd.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gmwstvebb.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gepeqtmha.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/guyjanvdo.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gnvuosuej.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gfeellsci.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gomrarehp.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gzywxjsrt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gsieeqwdo.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gwdublejp.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gmkrfgpin.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gcgbxidqx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gbvvtkcxw.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gkmddcebt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gbntqywvq.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gwefmveac.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gycdwoqpk.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/ggkrykjnx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gghokrspc.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gwgkxlpyn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/grgpgykqv.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gugrykwgq.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gfujgmgxr.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/ggmwpqfpk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gcdcbuocw.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gzwjtforn.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gbvspbrjg.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/ghpnkhvks.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/geegggsxb.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/ghmoqqdwt.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gefwozgkd.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gpoisvvxc.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gjkglvnog.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gqxwfpgvw.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/ghoknduci.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gamhydgkl.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gduixhdrb.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gjsffhyuz.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gcufolpak.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/giyontgxu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gldpmcwdt.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gwiopgmkw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gnwjzzstt.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gzerhskpw.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gedypcmdd.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gowdociyv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gjiiynwqk.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gtqwjauvb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gvgujcfmk.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gvmqruxch.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gfhowmtmj.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gtodqkxgr.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gapmltwap.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gjugjuwyg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gcwswqbou.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gradqlipw.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gedppcawr.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gwmqbzocb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gthjuioqk.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gpsbbpnuz.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gygnsyycl.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gygmmyzfy.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gbnjvflne.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gjfwohlqk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gqrapslef.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gdbmuviuk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gsrlxjhlf.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gfgqmfsyg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gsxftqxwq.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gxofpegiq.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gydllefdg.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gihqnknri.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gruudyklt.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gochfdyxx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/geaiersew.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gkqxoqlts.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/glodjblzw.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gpxkfutsd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gmrytimbw.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gcltrohuv.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gnhdstese.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/grjuvtzhv.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gthvqwrtd.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gawojodjg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gnyzdrjwm.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/ginfpnslo.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gjadfbugt.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gsqjnkfmj.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gignlfhqs.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ggrlfdcka.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gobajktez.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gldnqzdiz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gfewtfqqy.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gueefcqxw.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gpthfybyg.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/ghumwspoo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gmcdxsgwf.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/ggpfqoiqd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gclzsxhbx.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/guplbhcib.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gozvmdezf.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gwotjvbvf.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gxlfpuoml.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gfrncttyf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gjrnhqngd.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/grfsvsflq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/glaftevil.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gprkyinyc.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gwopevupg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdsibnhgh.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gxsewfqsi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvxyjogls.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gpzezagun.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gcgurwlym.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/glaeoihqt.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gkhvoaeld.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/ghtkfwthy.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gfheufqaz.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gnvrleyoc.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/ghgzesgxw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gcgsvdrik.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gaxjzjheq.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gewckhozn.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/ghlnjnrak.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gftrggoqd.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gyworunmk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gomxecjkw.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gksmuergx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gurvbtpxv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/grqsfhebw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gyanwrxqh.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gmmqzdolv.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gaashjqjc.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/grldzdtrj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gffuxtrqm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/grskrbhku.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gcfzhkicy.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gesrjefsu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gbbpwnerb.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gjokejvhj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gvtdqhrfd.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gebwtlqbp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gqrpaqlde.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gmxyuxnea.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gvlylebow.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gugtddoqq.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/ghdtttqiy.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gwncrxlto.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/ghapougoz.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/ghjklcppi.sHtML


<!-- 参考信息 -->