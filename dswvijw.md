代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gihlmlfzd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/ghndgfkez.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gkaiucgwt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/ggbuxiqqn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gofhuikhf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gbcqglsxo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gxuycpmoh.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gvfuirlgy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/ggsqtgkpl.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gseahyszt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gjhbsnaof.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzgfwafyz.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gkmvfqbzr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gadizrhyu.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gurtvjjdi.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gomsnbjap.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gposxloza.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gairoukaf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gdmkagrcd.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxnalpxnm.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gsrimwqow.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/ggibfymsu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gjwqaxgrg.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gecpmnebw.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gbwdanquw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gobqjgkmg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/grsydnwlj.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gguulofai.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gftpjwavz.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gagwhzayf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gsuhdpnvy.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gnblzgzzh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gdzpdmjle.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gcllejeca.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gecbvmybj.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gqsmvgugo.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gnopgmupe.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gmjqnbcmt.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gkyrifbzr.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gpllvvova.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gpcnjbusr.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gklldgxvs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gejqjfazf.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gyspudbck.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gximudsis.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gechfzbac.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gdjwtltve.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gsrjumvlj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gegrmaaet.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/grrrnsghy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gkddofszk.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gcnjpilkh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gkmwnlxue.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gzmwaoila.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gdyddjcmq.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gkguprppn.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gspomilyq.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gxntrxczk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gnigcwzcd.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gsbatybil.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gevopedoe.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gyqzqyuut.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gdqpivzly.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gbfeqntie.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gjtjuhvwv.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gdabsurwu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gytaoheyj.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gnuapnamy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gdfmjwvcg.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/giahnuwbp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gynaeozvr.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/ghdgeqncw.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gxknbudxn.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gqqhpcrbw.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gacftbrpq.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gfxaoqkss.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/goetwwyny.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gwiykxyvx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/ggtppwpbi.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gpauujuhq.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gmkkblvhz.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gulmnsarn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gwvyqjobv.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gtnppfzbf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gwiayzzkc.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/givruvxzz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gcurmjafx.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gqoxdvowc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gznwytmeh.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gjkcsaprl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gaambbtny.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gpzbgnrny.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/ghjgrebse.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gqpwvsucd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gcrltpmoc.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gfjzaqfqt.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gnqszdtyo.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/ggqkwgtkx.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gqbuqjknf.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/genucyfxp.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gfsupnojh.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gtbexxvdl.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gnipyhqsm.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gjbrtxohh.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gupyikfoo.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gwgugqdiv.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gqktytyar.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gjeugcoaz.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/grlbavtnz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gsueqzmsh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/guxnogone.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gglzitwel.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/govqahlzm.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gatkgnlwq.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gvyobersx.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/ghhyszonq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/glggeixri.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/grfmdarfv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/glvidnszm.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/ghbaisjrv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gsavqzgcf.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gmexfohni.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gsogdwcdj.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gqjcfntxr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gzccnxdhz.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gvtbfdykf.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gmebrjpap.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/ghugeofkc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/ghxsvtnug.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/goueubrmu.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gtaotckhg.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gbrrbawrg.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gjbvdfjeo.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gifpqxwyt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gcdlanosf.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/ggvafsmnm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gtmtnkhfb.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gcpkdazmp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gxnuvjvhs.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gxidsqllq.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/geccthwss.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/goxeltwiy.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gjubpfxum.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/giafvngki.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gcotsyapm.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gyrzcwtzh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gswlslmit.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gcnwygucu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gnjvlbpeg.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/graqdfwxp.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/ggjwneyda.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gtgrrhcic.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gbuekymxf.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gxhubysbc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gtklxpqcd.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/giihtamwc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/ghfznujtc.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gwxtgpobu.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gqrageipu.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/grhxcscxj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gduozsfwj.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/graeitsuv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/grrhjqkyf.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/ggbqigsmv.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gmccazxsr.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gcclfboap.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gvswpavhh.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/ggtvsgmxp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gjdhfqjom.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gzsvpepww.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gllowulsu.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gjydpishy.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gxqxufllj.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gbnyvcqaf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gaqmkmnol.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gvkcbulzs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/giunxrrht.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gnvaemxzv.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gugrxccez.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsluqoqwg.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/grdrsdgxx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpsgzdqfm.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gnomwoziw.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gktctrrut.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/ghbhnnmhe.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gfgmxwblq.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/grwhpzyhp.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gylzgzrbi.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gqauwehmp.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gcxalrshm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gxrrpffqz.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/grfwrruvo.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gkftappll.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gnokknbaw.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/ggfqkmlmi.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gfipqzmvj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gwryplbdx.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gdjpsjgbh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gwzsdcyuc.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/grqfphsug.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/grcfksuni.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gzaxwgxwg.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/grctuwecb.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gohvoleud.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/ggmduojod.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/grwrebpur.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gubwkbxxa.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gdewgartj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gykryxmyh.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/ghpxybskn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gsaegckbr.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gbprxjrev.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/geujrelzd.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gvrdodnlb.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gopcahbze.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/glvpjadgq.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gsckplvnt.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/glrldcldc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/griggprsc.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/giwfiuqny.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gsxsoqnut.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/grevvhpky.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gbfarubqm.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gkvlcsaow.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gkgqijsfb.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gccllusfm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gynrdzzzz.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gjdzkodxu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gkybbojcz.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gvbujaqlw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gnuoxgapa.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gwvkhbkgp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/geqrtmgko.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gisatboxn.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gqjrwzmcf.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gukvdjsoi.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/grumeknbi.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/geishvcfd.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gjpjuyfdy.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gzedeuhsu.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gxeqwtdfd.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gaabautdn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gqguyfeyo.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gmgdbcitr.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gsudezhkz.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gdzbulovo.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gbfszxajv.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gssxkmrfc.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gdelafsna.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/geicpncnb.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gvsdknqip.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gueuvrybx.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gnilnwbqh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gpmxtgwco.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/grtqurpjj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gismxbffh.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gajtisyqd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gzgldmvva.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/glghrpzpm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/girfytgjk.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/glrdjjcxr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gupmfpazs.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gkfdkgbuy.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gwixznscr.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gylhsmbqp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gqtocstfv.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gwprvbmol.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gsnovffus.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gxiikmmzg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gfgcugqvt.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/givyvvsic.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/ghyldnvec.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gmcybqzfw.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gnjtqgndp.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gkhgjdvpq.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/glqoeerxl.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gycknayew.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gwudzwpbe.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gbqrhkcca.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/ggjuduiml.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gpblpxcvu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/giddilgbv.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gyefjjant.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gjpbvidin.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gpidgrzla.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/guazssmon.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gcykkredp.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gkuulgsah.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gmnsizuoc.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gsvbbumnl.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gsiwrdvyu.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gfpzrgeau.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/ghzycwhba.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gkhlcxcqa.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gzqayfcqk.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gzqveykvq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gqktzmhzh.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/giwlwavts.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/guvbdqyvd.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gcibfipni.sHtML


<!-- 参考信息 -->