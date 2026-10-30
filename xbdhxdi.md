代发 wailian999

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnrxnwiu.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gzrmcspge.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmofrkveq.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gcgboldia.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgvsdqds.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gqutomfeo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdcjwxxb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwjizbkk.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/grlosmiqr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gryukdnmx.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gpzvpqdic.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gahlfwaes.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/glmegzoku.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/grrzdncjo.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnobtyxiv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerrkcjrn.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gudrkpxzy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxhzbmslb.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggclzdopq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/girzjxrjp.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrbvcrca.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gurtasoht.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gorctghid.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gkntjiptw.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwpnpsnq.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpsorzsyo.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gzalclawf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzipekkdi.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gbymztfii.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gtlralmam.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/griduqrij.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbtwvipt.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gjcotpaxw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gntjcwjxo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmccpxej.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gwantpecp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvabmojy.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gwuoyylvc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnlrdcbg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/girldlrhh.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gjysgxroa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaikbmgw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnygpuii.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfvolngh.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwrxskbq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaacfxvod.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxwjeams.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcjiafjr.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/ggoylwyir.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzweklqg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoclctwo.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsdsyddl.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gbzihilpv.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gonrelvrz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gojfohzqd.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxcyicnf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gsomnkwnb.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgvbvpyn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/glwuclyhk.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/graftfrrq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gnbfjorcz.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfevlzwib.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gtfkbbfps.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gfkesrhxj.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gsoolpfda.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/goheshjxj.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmktzpjmj.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtxjmsiy.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgjsqbwt.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmjvpbmbv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnfjsqos.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvdfyfcj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/glodhmkrq.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkhudxjq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gspqsfwsk.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giafqsubj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukeanfru.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gazevqeuo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfybpsas.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gheurtyje.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/glonhgmxc.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhfsyldt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfoaavyt.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gicuqxzuz.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhteqwdm.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gqtmhwqiq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gejwbgioa.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gctzpouju.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesvrzvim.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gketahbvz.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjohjmuqq.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxbujesp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gclrmxomc.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqctrxqv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggcocfqru.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkruwhwb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvyujmnj.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gepbsndus.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gfseihcdi.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gcvnevhgl.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gauttlbuc.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gunbezopy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpkjwwks.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvlfreui.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/grgptpeqn.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gjmreqidv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gphhkopws.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcxxlllou.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqajypppc.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/grkksragp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gslcidyrr.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gtisntxnx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gzkplqtpr.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gnjjkaeai.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gayolajlt.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gldppbkha.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnixhrhxs.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdeoywwr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrciiujx.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzobplizh.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gyobuloyl.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/grxzwmzhs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gmmljxnld.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxqnhjjd.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbkcotoe.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gyycukhnq.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gvikvgzgt.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gmqntoxjz.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gczgntcxf.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/glbdywrav.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbzjruoup.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glhihmihb.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gbxcqelpl.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/ggacxaplt.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gqhegtlwy.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gadjsiwdf.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gytxyzirv.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gfxkkigsb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbddkjyvi.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gdsnbeswj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqamqmnmx.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gniuwykkh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyfdciyy.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gqzwwrquu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/ggvcapcae.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/giscrltvy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwlqntozo.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gsdlepujr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpadtxsj.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwptsvwl.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqpcheqzs.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gitszuuba.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gonxjwyjc.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbbtzkcn.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdrubryqn.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gcgjgyrxi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gsljmprwq.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gitrphxpj.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gnufwrmuh.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhjazqud.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gpkmeoabo.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllypghzw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/giydjuhlc.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givmjjblh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gcxecqobr.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzjzdkhg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gqmslblhp.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gbcgirjwa.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/glmqzrmxk.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxdbggtgh.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhptynlp.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbyqnbnv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gqzysrcnb.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gbyijwqpp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gzxvzoevb.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/geszepblf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkdvlunj.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/grjfpavpz.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/guytkmafz.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/ggubiwrtl.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/guedrvnpl.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaikqvoih.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkxausqu.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gnahlxwjm.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gamdxprpx.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaqwfwtk.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkzwjcao.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqgdtpiv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjylrkxlm.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeiiluwy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghomsgejy.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpogibdqv.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/ghggqcsgl.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/glafkmmge.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikbxgszo.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/grzxbgkre.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gghobgijn.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjeyzaql.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gqehrjgcx.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gyxofwdcm.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/glpeyvnsy.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gilprqbdp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlvviqiz.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gybhsggys.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggneavala.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/guznsdfnx.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvdbpyrs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpmsyputb.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekmsbfpv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxyzdhxy.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbitldftd.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqowozsvk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsesjzyty.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/glibqubfm.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbmrxgyn.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/garpaqgzf.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govllwfwy.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gusaaugcp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidqnlsur.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gupeprcud.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gejacfzjy.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoenafwx.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gmbjklrcb.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/ggmwhdezf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gohrzwphz.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/ghezbmiva.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gnpkxmbgu.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gobtbzskd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gwhacipaz.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gzaradooo.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpkduwkb.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnyxvnatb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gbnuqrqoj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gefbzhdgs.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcxvvfom.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/guxyqchze.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gdxdqrmbq.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvywhwwe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gzkztshmy.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfowjpae.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/grrirgnjg.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsskixtz.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvokofyx.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvyfkrns.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidvmgcnd.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/grgjqhoat.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtqsfcbl.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gxvpgrune.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsvfvsjn.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvosmttfr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gnmzuflww.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gudeyljsq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/geurnlqbi.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmxhlxlw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxhrlgat.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gsuwuknnx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gcqqabsgl.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzhblpph.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gerokldqz.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gsujmrwjb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gscpcsutz.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gagwrkpti.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfhdmwic.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxtdmwur.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gsqmzbwvo.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gipqykoet.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyhtuiok.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/goulwdjle.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/giesknncl.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzqqwowye.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxdbkekt.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/grlbajriu.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/goypffkfr.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/grajtyxng.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdruzlcbi.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqvpkjbv.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gbosirppz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoecptpi.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gfojsnpqa.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpfsbpof.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvorhdtm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gvpaqngph.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gghstfwdu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqvmdwhzt.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhdiuesg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpncfypr.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gkskweomq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gutauhobi.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gnupywwgn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzybsucg.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjwkenab.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdghuaag.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/grmrhylvi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnsvhudh.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gnrjyhtpv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/guynqdlpi.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkohbctka.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/geccjqsyb.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqxxfwrc.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhwlvwkg.sHtML


<!-- 参考信息 -->