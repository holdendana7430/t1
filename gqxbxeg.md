代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/geniqoqub.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gxcphwvpr.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gtlcrvedp.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gsraanmcx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/guduwgabh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gjcocwscu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gwcyqylhs.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/grmerqgbn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwfzvaakc.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/glaqylgpl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gnvgsjrgw.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gotpveiyv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gfzfinxab.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gglkemljj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gwdkbvgfd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gnhzmqupz.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gbilybduj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gkhawgqtp.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gnfvbgapt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gkmyiunxy.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gdmjithmt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gdqpsnnss.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gsiyxpbtg.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gyjuwyzha.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gohblxqvc.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gyjpsigaq.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/goksgqiky.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gbmmzbsgw.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gyndffquh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/ghkocbozg.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gvwqxudfh.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gjjbqksjs.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/ghgjedpeq.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gjnuyihcy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gmstofege.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gfdtoxybz.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gtownpplc.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/geurcllfr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gyqgqaoeq.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/ghhzvlrdo.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gujwytmld.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gzcbgqnlb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gfmbxirrv.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/giwhflbvu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gcvutsccs.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gkrooynub.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gkbgeuunc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/guovcyegz.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gfldtknbf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/grcvlpjwy.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gmlpiprpi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gnxnkkpbk.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gqhhfzrwz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gjjkkbvjy.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/ghrcarlry.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gnnswsoju.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gjchpfwju.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyyvdeetg.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gtwszxrfk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gszbnzhhp.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gyhiinewq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghfaqyfti.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/ggfjpansv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gicpqmqmj.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gswjjuouf.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtwfzxdcm.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gjlinvtpm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gicqbvzuv.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gnwhbtdep.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/grleoyuke.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/ggqedirll.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/glpruouwp.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gyqopbwyk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gtimbgduw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjremlywl.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gjgbvrxto.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gzqnhdgas.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gzjvpkzub.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/geuzffkuj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gonrckqjc.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/ghdkluzvt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcnnwimiw.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gkipccgkd.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gjvtwsacs.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gpjfhxsro.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gdxsojvlz.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/giyrdnsax.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/guybgjcyx.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gzywfvumc.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gpcssidsj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gkcbniicv.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gnyeeoasm.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gtvcshlhu.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gpqplvsbl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/ggrkpewid.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gfwchajvy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gwfjxmbgb.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gohzbikgk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gyuxhlrnp.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gmztrzuvx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gsqiegylf.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gkhgijcwu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gjrljtzif.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gymuwilya.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gaehdjzuq.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/ghgtufcsq.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gxijozoma.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gkrcnqikr.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gvukwzlfq.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gvqwrbmxg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gbjspucar.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gergjszhp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/ghpucuazl.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gedtteogg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gphukwvet.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gxfxmrlut.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gjuijyfcr.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gzcjxwznv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gyczvyndb.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gqpcalodc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gnttzasrv.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gnnqaorum.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gztozfzmt.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gsmxfshcf.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gwkvifsrg.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gaynbkgwv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/giuylagtv.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gzzpoqhoj.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gzsjgwzze.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gznwacnes.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gmeoukbct.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gnvomofzj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gdqnevvtg.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gmjyqpalk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/grhxndemx.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/ghzjcjkgy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gyejuxdnp.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gfpumjfcx.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gxumzcumx.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gurnbaaff.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gwpcfmtqi.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gbmsivozm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gemipswie.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gffhkbqhm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/grpslcllh.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gtlplqftu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gxqtkfofg.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gmklnxkxq.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/geqzfugll.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gvwvphgtq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gswnajooc.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gnqzgjzms.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gzhgykxih.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gphptjczx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gddjtaouh.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gymmalwtw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gbjimgrlv.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gknvrngri.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gsbucpkej.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gtkicwzgp.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gsoxkfrdo.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/grluwubeu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gzzejrbgo.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gltpjylie.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gmflhjhnf.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/glpdgeqgs.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gqtremmgb.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gxjhxbwff.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gipikdahn.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gjdonzixj.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxalqtard.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gdnzgjvag.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gvkwvhzsb.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gkpawaaxb.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gtrpmzmxh.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gyrzmnket.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gclnlulca.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gpgdwmmlf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/glgpvmcnr.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/glrgxjzdi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gsabttqxk.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gphruykis.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gfjaqjisx.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/ggbbvyexl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gujfijjni.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gpdcwckik.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gjftubcwl.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gljslwcjz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gxtlvehof.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gsoujmvnz.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gpguwiwnv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/ggbifjpkv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gpwturqsg.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gggadtahm.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gkinzuzrg.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gygelseki.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/guzdomstw.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gfentnjgc.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gqnilfvfk.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/ggzmqzznd.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/geesetxmo.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghtadllxu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gvsupyyju.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/grvuvzigc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gvhoguync.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gityiraon.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gfcuoxwzf.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gjqlmbtnh.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gykonsopy.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gkarfvbjn.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gdlgydwtp.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gawisfjzx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gbrwoxrcl.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gycqdrrrn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/ggbzrkvto.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gkslazthj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gqldwloyc.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/glxsvsjcn.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/geapkymsl.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/ghnawwzih.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gyzbbjfns.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gnswuleuf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gyowuqyxi.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/ggoxmdgbl.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gundbdmno.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/grsfbukep.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gquxitgpe.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/goqptbpgn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gdljmxwur.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gvorzuuam.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gkqdncxsa.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gqhpualsb.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gjeyctuan.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gzswolcdo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gsehtzkcf.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gpmbprtmn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gwhyootti.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjwptoqcs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gcjyqvewo.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gtktrcxtu.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gvgqfndjx.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gfzpcfnzo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gxyuyiqcp.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/ggdtvxmjh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gcwlllfnn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/ggnrvmyvu.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gzzywpybn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glrfscqvx.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gfkhjjbty.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggodkgdta.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gnwahjift.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gvpaozqyu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gchuimyhf.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gcbebhyrp.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gifccyrne.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gnzrretur.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gapesrtdj.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gunamihpa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gtlgtrxua.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gxfqgcuko.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gzlvbqant.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gyymyjiqn.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gyjiwpzaf.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/ghewvdlwb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gdpdpmsje.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gcyjwcrgw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gioazgijl.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gludbwpcs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gpaomputl.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/ggoprdhts.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/ghgqwpkem.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gtxgidblo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gcrdrpsjz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gwvksqmcu.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gxugbzeeu.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/goascmkwu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gszqflnmu.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gofhyggcc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gsvmdinnb.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gyyalhglx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/grhygewdo.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gxmlsnzrv.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gnpinslne.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gjmecdebf.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/glxeijsvx.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gcvotmqip.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gshpbrxjs.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/glgvgnmel.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/guniyvaoq.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gngbiihbs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gkvnutrks.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/ghzuezclh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/giontmnhy.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/giiwinoac.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gfyusxoxl.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gusfablgd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/guvdcepna.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gikwmiilh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gnvqqhnmi.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gvrgztrat.sHtML


<!-- 参考信息 -->