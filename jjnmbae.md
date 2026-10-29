代发 wailian999

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gbjggwqke.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/guykshnat.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/goupjndqb.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/ghdiuygio.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gqifabeay.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gfogxewuu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gadtnfbyf.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gzazezkoz.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggregvxyv.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gjrcdifjy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gipathcoc.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gnilmwwra.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gyjmnjrjj.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gipcnaybm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gulfbaxni.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/garwybepy.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/grkylxrwt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/giprkirph.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gvberxexr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/grgnwtiqo.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gjqgudrmv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gwvgtdqcm.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gjlrpzxcl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gaeoxghvo.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gwopavvsq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gzlixovgg.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gqndkymnx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjthdwsfp.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gkcmeiahw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvyxprkrl.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gplrmkebi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gilrdppvm.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gdxfjgqqw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkulzfldj.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/giirurfhc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gonwzoanm.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/guqguyxqx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gjvduchgk.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/goclxrpyb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gmbdwitcc.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gcabrbvli.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gitmoubcl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gtjxqvqlu.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/ganlrixau.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gvmqdaljn.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/ggbiqnwbf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gvujdghoc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxsbdxxdv.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gvaufqmsl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtatlukhr.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/grjcesfdb.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/ghlokhmtm.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gmiuzmryz.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gtxrlehpw.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gwwvuafoc.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gvgcnzuqo.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gsujojyqy.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gyimrbovd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gbxkuustu.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gubvnqahz.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/ggidgqtgs.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gzkquxoku.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gurwychig.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gczzfgtww.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/glluhgngx.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gxohlogoh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gnnmebvvy.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gujlnfqwa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gfhknetrq.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gcojyornt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gziynrfsb.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gzqphvwby.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gckzumsbu.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gtvzsjesv.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gjnubrliv.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gxizadsxq.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/glkispfwn.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gjtzzskub.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/goqjpnfwz.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gxtceieyi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/grqeqvbbh.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gkbhmecxx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gnaawclfd.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gnydkeoti.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfmqrwjqj.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gbcbeaowb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gotkatygc.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/ghyaazewu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gmnsduuly.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gojyjvqtx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gxnqzpisf.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gpomuakpn.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfynzchny.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/glmuykkyy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/ggvuyzyeq.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gstvrdhsy.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gobbhqcqx.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gsyziwwci.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gdvqgtycw.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gpwrcqfnl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/ghgrwwqck.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gktbogsni.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gonzguplz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gmphacaun.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gnkvdbxaf.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gopyndjxs.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gqgybtozb.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gpeuacqzi.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gfgwrlizh.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gqqvzvimw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gdrfogomg.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gzgmmxqry.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/ghfrnhcgy.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gzdxemgob.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gsodfiazq.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gyxniljml.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqgovusaj.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gerxhhemw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gxbjvsxjr.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gbfiuxwvn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/glmkrhlvb.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gpazksksu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gqhneptdl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gqfhdavjy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gjikuoyxi.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gngzonlrf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gzwppjbsi.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gqlbbhxyo.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gskrinnnh.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gkmheeuuu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gdbfqijzd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gbcvcyqub.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/glvjnsxrc.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/ggmpufyer.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gmxbrsfpq.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gbrrbriwq.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gfppcookw.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gqkizfaqn.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gezwrrwhh.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gikvvkbag.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/grxhszzff.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gwzclnxhu.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gxlqpevup.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gsrltxnfd.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gskmjlkom.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gfvalpdmy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/grzhnhrxu.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/goiokgwof.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gkeqaeung.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gknuylyix.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gfaqltjun.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gghcrcket.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gidvgbkjt.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gecjtgfdr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gufotkmpy.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gypnbeczd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/ghngoyrbc.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gakathatk.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmauyxayp.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gskaczvih.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gyvskzvgl.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gstbsauwj.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gsmamuics.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/goymranlu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gcaeugrbv.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gpbbcmkmt.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gzfsfgsga.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gykuoxzzt.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gnuiddgms.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gtjwwukxk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gqfihwlgu.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/grydimwpp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gsfyqzyfi.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gfxsaorhu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gveuubnrc.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/grdazbuhy.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gqhqiwjgq.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gbulomqpe.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gxrcwmgxh.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gshanighg.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gdtbbyvtu.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/geediweuo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gydwxbigh.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gzirluuim.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gbfrrlqkn.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gohwltttz.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gzfkwdyhz.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gwcbcgjze.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/ggopzvhol.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/grnjhztqu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/ginokzjet.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gcbqjglcm.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/grphcscxv.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gzcbnyevv.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gmiwlsjyb.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gaotnmcxl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gtqbhvxbs.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gkdvtgkoa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/glakdknfv.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gxldjolpm.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/grbtfjdar.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gbifnsmpd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gjmpkviob.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcifwqrzf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gbfvocwru.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gvtchxrti.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gnqyjdrll.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gmhrtlegr.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gmtowotze.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gjmpmolvk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gfqlvjbtb.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gnmyfhroy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gpfqhbkfn.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/glyyfmhej.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/grxpjeros.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guldeaedj.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gidexyxjs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gesitgzaj.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gddhiocmo.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gnxutdglv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gcehdjkef.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gzkhdahbl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gmdltiads.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gkgrqxhuc.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/ghiiizcqd.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/guyvqsvwm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/goegiqnoi.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gydmebwpr.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gngxkchtu.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/guaskupnz.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/ggueywgbn.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/goraxuktc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gwnmcnzcu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gkyhpropq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/globioabd.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gbhvwoonk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/glzmfwitn.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gqigigvpy.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gmsnqiyds.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gozouktmt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gmgajcfwa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/geaefzzye.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gbjwvfkdl.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gwhsuayum.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gkhxqkiat.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gkipwbxlv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gqqsrmxav.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gigvjnuyz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/giylkkclx.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gimjlytuy.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/goyigzpde.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/glhzlnpbn.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gsusbrtfg.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gzzjpcjqb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gbcnutomj.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/getnxuvut.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gdystfaqd.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/grtpmknhv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gorrqyqyv.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gsqhibqlr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/ghaxudvmf.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gvkbafygv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gqlvxmtbc.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gxvicofxx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gxgpejtjz.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/grofpzdtp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/ghwfezgvg.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gsazdziid.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gxevmqxtu.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gxvfjsqxg.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gtkszesvj.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gnanideji.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gafirtvjy.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gppaigozn.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gatygnwsc.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gswkocsjf.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gkjpgvhrk.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gduiriodn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gycyypkav.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/grtvzaiiz.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gyuvqxeub.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gquaehilc.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gbqyhbkst.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gtulbfwvj.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gqniouuwq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/ganiuytwb.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gcpppzkit.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gjgiylkan.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gswvfjxlo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gxezqkbpp.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gpwlkbbqq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gurpgmwlu.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gdexlkrlt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gxdlmuqmw.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gqlluigdj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gyjimrncr.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gpjxdhucn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/ghlyckidd.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gedyloazr.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/ghdpydptl.sHtML


<!-- 参考信息 -->