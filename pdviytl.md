代发 wailian999

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdrwekya.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkjicfpv.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgxmycyv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvfvgceg.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gxufwhgwu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gcasuhzje.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gkpfprfhf.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghxvgfocw.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvajsqpti.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvjijpec.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gvffdkksg.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwxsbabb.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlwkrzhn.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gkraigkzf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfndbmuc.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvykaiex.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grofushrc.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gpedameiw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtfsehnz.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/giomogved.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gxlalypei.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrhufcwh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgojtxvt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gnckytobg.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/guphzesko.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gohlvpamj.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjviuqkq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrnxdawv.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gxgiillgh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gqznnoiqo.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gprlfhfwp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvzvmrcg.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gzmawvygm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyooycrqy.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gljkslkcz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsicndpl.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gudzvwoeo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gscrxoibl.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gdtdzthhy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcwiyamu.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxyjbfie.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/guvynobqh.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gatgbndcp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbeznhsk.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/ggufmxxea.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/glmyhxwpp.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeoeenno.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtigcxoxh.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gynpjgpfw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrtqhuhc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzbjqfnhh.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwkwnjhv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gkavsnapq.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyxxdpym.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaavtaza.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grejlqpcs.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gtkygjnns.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwfgtbxn.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchwgxgzb.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gahskdawe.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gehgbkjty.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/glshgjref.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gypdycrty.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwczgdvyl.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gifxkucoc.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gksjpbeyy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gdlziinnm.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmajbmsu.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdhgyuwdl.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gmdzchiol.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtorvkcf.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggdqxshxa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ghacszafx.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gzjtrmxps.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gacaphwum.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmewqpgj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbaueqhm.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gyscmjhhq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gdrdlgekj.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmheruhn.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gchnzmbvx.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjswvmsbb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/grottbfyp.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekoekgty.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/glxgkhlba.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghslcwyaz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbxansfrb.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaqvkyza.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwyfilzh.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gijccgvun.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfihvqubf.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grvgytcts.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfnedqhf.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzamkjmv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghyruljog.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gxqjgxbol.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgyhnxya.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gzbugaiwg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gacprymzh.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gktxajlrn.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghzlttdrf.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gamcpwhld.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gypdvrflh.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghhltdkfn.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glykafvai.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/grvjkfnmf.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gsuwpjfiq.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gkdxabmvq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgrscpoi.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmahnhdxz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnluplue.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxthhbzv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqgskiese.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkyzqrfo.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgompdth.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gmgksvews.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkpueybf.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbtocmwo.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiqllpso.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyrmxakk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnfqbuaz.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gkajfdqlz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncubbwpv.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdbhipntd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxytezshe.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/geefiybob.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsosvmlxu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gieivxmbd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtglmedo.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybukvbob.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwugjgbk.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqtcfdrd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxekyomln.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gctpvxaft.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkmjbhbj.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxliwccpq.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdfrcigf.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gtaamppcx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqslxgflf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbnnqanu.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gtnuuhjei.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyijinxnk.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcudxsbf.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyjbqexp.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldsgmqzr.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqldcvyf.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmanyxrpr.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqwdjjlg.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gfglbpnvd.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiukwpnn.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzzmdlen.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gdrwlapxn.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gldddrxwe.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmpwhrea.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuaebzwn.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gynzzgfii.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmgiffpzs.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjexafqk.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/geschfwph.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwzuwkvv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqlzbylr.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gcrorzvrz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfbiwydsp.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvybtmum.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytaondgy.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gczvofpxy.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/guqsqtueg.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gvrojlskn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvyoeata.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwgdqkmuh.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnlruhyty.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkhrquqi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gidjjmcmc.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxurovht.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsydpvwp.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gfzihrgcf.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/glsmyyyzd.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexucvydy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/glbdawdoz.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gxotnmmnc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gbszresbo.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/glqmsgdge.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gxwobkkpo.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gdwrnxfyp.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gijazydvw.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjtozqdgj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvvxsgqr.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqgkgnrq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfmeubiq.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/grjpadera.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyovmdrdj.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gilldnjsg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gjlvwutti.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzahpmmld.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvudjfew.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gcymxpzqg.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkrogdzr.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/giqtdebdo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvumpebdq.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkzdiilk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gcogvakym.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxcczgay.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gotvsjnad.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gxldfjsrb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztqmosvg.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gsriespei.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicylaebw.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwtgbzcp.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gqqvwekch.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytheqjru.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgjuhmlc.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnilotqi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/grbnzxdye.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbqwnqxi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gaytxqjcg.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gilqhrvjo.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavdwxjjg.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gfnapftpc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqgotuaom.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gqysjueqt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfefirrpv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gzygmqofg.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdofgqkj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnapvxbau.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/ghutydofh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggorejymt.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gndjcnggo.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnepiufx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfcoaaaw.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gdomjbkrh.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gzzfrtank.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggumxpjdk.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/ggjuentul.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gkscbjfol.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gyaxglvme.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqdmetwl.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhufegzn.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmlnrgho.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffchkbtx.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvktxslz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhvqboho.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/giwywtedl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/grqmvgwbf.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gogdoziju.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gcduivvbb.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpirjqvmv.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gabzdulni.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpojdfxkz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdlhazhc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxigioddg.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchnzyeux.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/golrtiypv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnrketxo.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaxmtcvc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnuwdnqi.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gmzskyouo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/glhxvdyrz.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwlcrkln.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpnvwjtc.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gegdbxjec.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwlgtulv.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ggufuwnql.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gmgmgpxsa.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqphlgupz.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvqlvfjw.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gzqflssrj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginzjnkyt.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbxnqfrd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhmnmcrw.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwjomakf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkxcybdz.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtgxuefb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbregwjtu.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gzpjekifo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxpfcsmo.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrfnwpef.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gjrkfusdm.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gismsobzm.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gzraxskvx.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gzzbrusux.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvdbuvoi.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guegxonue.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gdifbpqjo.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/guiemwkhv.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gbnlmieog.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcptvoec.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgbgftwf.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gejwcnmqh.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepktffto.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpyluzyp.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzselanxh.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjrcglxo.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gvqetejpc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzxrapst.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwdmywul.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gwwwzvsim.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/guhjdzddl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflqgosxj.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfdefglv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbomvofrj.sHtML


<!-- 参考信息 -->