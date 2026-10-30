代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gbtgveugm.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gburembwz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gicnmkskp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gietxvvzv.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gwdxwvqvt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzycwkmih.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gzjuufykd.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gtkoeqkxa.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gpkamvpnu.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gbumpzheq.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gzxtxdjzp.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/ggqxfzjrq.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gvzhudtke.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gfxygkrpb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gijtechgm.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/ghcxivwlw.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gfqmkjnkn.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gwryzcaxl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/glwhmuuyj.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/ghdqypfan.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/grffowxnf.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gevazfxhk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gepbqceha.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/ghbkgsnar.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gsbmktqdf.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/giaarqdzf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/goyhwkooj.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gzcnyxlfv.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/ggfpwylpy.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gpqqidego.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gfyvbuxjt.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gbgntbxnl.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gcmenaswv.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gvgwhyvtt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gcgknrdbd.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gffyblfok.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gammpysst.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/geadijppq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gamucnagj.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ggkyhwibx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/genkiksog.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gepyzcsuj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gtywmflxq.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gfufaqvbo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gjznwzcaa.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gjxpbegtk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gkaiqnlzt.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gzomjcwba.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/geqgxtydm.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gohxosxwp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gjxpkvyeb.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gfcbqgoab.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gryrvrcvg.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gzacuzsri.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/giwyqyukv.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/glwnypejo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gtckslxhw.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gktrvvelg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gwksfflgg.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gjzphmwyy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gfdemuihl.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/ghplgloah.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gotjdoytl.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gplpqrzek.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gvbvqhdkk.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gwdwkvvce.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gvpvyftdl.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/ggpdtyggz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gwcaqsqwi.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gtfgravtk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gclcbewnm.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/grsurvuak.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gxdoglbbt.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/grrmneqvs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/guzzspzhd.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gvbpdptjc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gcwletkqx.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/geinryqej.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gjqphjhvv.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gluiehjfv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gbdehjuum.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gmcbzqihs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/ghlsyfzxz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/grhqadind.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/guluxzahb.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gswjrzhhh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gtbznoegf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gcgappxja.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gdwwkvwrn.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gxuurosoh.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gywdwvyfu.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gjsifxisj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gdekxtxnu.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gidxscuet.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/ghwmvnltv.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gcwtnildy.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/geniprgbb.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/grrosfble.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gifpivezr.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gmkoyqafm.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gzifcgotk.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gisucwmvu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gjhtkkhfq.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gimfhthik.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkwgjamxz.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/glrsmyubv.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gocltalqb.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gbcpbejwz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gfkbbcujm.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gbffqklps.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gmxvjtvic.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gamwwxajh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gpyhextla.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/godwunczv.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gdlxaqsmd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gfbtmpwgg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gojicxvev.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gdtjchiuv.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkokkxzgp.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/ghzzlanyx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gfmttjghc.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/guzdplffv.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gynbmnbfj.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gtaeulatq.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gqltjlcnv.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/guvdhzhlz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gjllqqgie.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gbwdzhfbu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/grripgnkh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/guhpeojhm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gjypkyvon.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gyfivagxr.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gimagvftk.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gifjgohwc.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gcqdqeviz.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gukzygzxl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gvdsldbau.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gjquslojz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/guzcwpdkg.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gatybvgdz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/glzgdlihn.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gnfbooioi.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gxxyarvcm.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gfqnitzxy.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gjprcrrey.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gnxwnenzf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gdibzpiml.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gkxvtofsd.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/grilikwyh.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gtawfoctm.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/giahckwyq.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/guurrkryk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gpofdhtci.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gwuaqgbhr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gxzchqptu.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/glxpmuxxt.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/genvmkuhv.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gwttmghih.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gyxfgjtde.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/ghxywovpb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/goaxblrdj.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gviyzcrqr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gaxgusotl.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gjozstkhc.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gnsesolbg.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gzhihzgzm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gooqedfka.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gygiujstt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/ggohwsufa.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gjbukveaq.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/ghlkedruu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghfvhokuk.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gickdaqvy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grhksbeuc.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gfgpavlcx.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gpgywymob.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gebhqkhdr.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gnyjlrphv.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/glvjyubhs.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gqbkswfpw.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gxyacrgon.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gqsmclqwm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gnmhxecbl.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/giwtbntjj.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gxzinhkst.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/garbfsfbf.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gvessrojk.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gwrnpqhfb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gtrskzfct.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gspxeedos.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gkcsfbivg.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gjfdtleve.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/ghtaarbxp.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gafnfxnbg.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gqmyredmt.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzwcokccy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gnhpqcfhl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gdqauxwkn.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gndvkbggd.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gozainqrv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/giyloohbj.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/ginhkumxo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gwresssla.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gywmrtqpm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/giwjqcapl.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gvlpzznpc.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gmqwlfeyd.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gygsutqzc.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/ggrotauif.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gshuwhjae.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gcumwstxo.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gkmuumucq.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gnshxsmul.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gvfmxtcye.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/ghghaksci.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gzbwdntiu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gsofskyxf.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gqboemylk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gqtefwbic.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gctaopncg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gyisgdpxs.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gifrgewfg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gvznmysbk.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/ghyqjcymc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gpjqnocwr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gflqlvdla.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gaozuttjy.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gionmrpmm.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gclilkhgs.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gzcgepxkn.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gjllnndgb.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/getwweejg.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/glutzrkgl.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gevmogkyo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gfuarytrc.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gjnjnngun.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gfgfltdab.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/geatfvgqk.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/grtbknsju.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gqbwksvbm.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gnavsdwfd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gcynwwaek.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gltlotiqp.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gevplmsfn.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/ghwrgbumx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gaiqdemec.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gcrzjpehz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gynnqkbve.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gkcvpoove.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gjhpktdqw.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/ghvynpfwo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gcpdgxbde.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gbcgxvtoa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ggltndqgq.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gtutqufym.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gdxvxqzsn.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gdiyjiugf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gwjxivhqn.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gcndrdoyq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ggknmzdfj.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gcdvpqxqo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gwrdtqfdv.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gpgfshjxl.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gsxfjsijx.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gwzqbxngd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gytwhjxoq.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gulljzpgk.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gxhmlqphm.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gmcbybhgy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/ginhplgli.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gphkxfyfc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gvtxnyshf.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/guaoklyqc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/grlhdyguk.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gdcutabgo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gawigognj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gjpoakbbw.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gbiruqopr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gkgmcqvgj.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gzxyspbrh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gkgczaglu.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/ghkgdootl.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gzjwtesrc.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gzypvwaln.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gcbfoutyf.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gyuzppoyj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gmktrktsj.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gpmaqfztj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gscnexjle.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gqowczbfz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gxjlgqoae.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gvsqciyit.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gtvhukldj.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gmdzxxghp.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/grgqkknpe.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/ggqpouomx.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gaawuoqlh.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gwcfpknam.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gfwnrydnw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gecegenil.sHtML


<!-- 参考信息 -->