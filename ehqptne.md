代发 wailian999

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gqbthydyp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcoetlclk.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gitstjzfa.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gbarjxyks.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gzculsbqs.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/galdxsbpm.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gwygdspbu.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gosixorhz.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gplekekwb.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gnqdnkldt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gieguovmo.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gtkbgcfuv.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gfudlrceg.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/geuutceum.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gbdpvsqci.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gfxpaffvp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gqumbwwir.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gzcwpsdyh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/goayijogg.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gxkgohsxj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gboldibvy.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gwolkmzyd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gapglwcue.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gcillbyms.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gfwkvrres.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gfxrrxasj.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gworjyiyr.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gidbtxacz.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gsxtdvdwq.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gmnyjxcnt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gqqqxvhox.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gqltumcfa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gduugatqg.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gqkasyzrr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gshmlybut.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gmyhoiami.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gxleavglv.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gaforbtoo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gkjlyvtmf.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gbejbywyn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/glkavaodl.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/ggkozrewk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gyxbxkoeu.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gdftmmfzb.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gesyrtngi.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gxpyfawbg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gkuioegow.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gucliaiio.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gxotglznd.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/grnohezrq.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gmkngoqxy.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gpibusonh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gspsesynr.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gmcsidkev.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gukehqfbk.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gjevawydo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gfxfdugfy.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/ghfzrecti.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/glzyjjlrg.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gnintuthx.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gzfcchftr.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gmdrfavxr.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gmrngdhyy.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gayiwtfqn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gqgerukgb.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gamdveosp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gpciozywo.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gcgotbxze.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gmssxqtoz.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gulmijzfu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gsmjezuuf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gknivdyuo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gehdelbbb.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/ghylgxgwk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gmukaaqdt.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gkkrgrgjz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gqndovpho.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gfakjdfvi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gvcqbbvuh.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gzskakxow.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/giplmeujy.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gdtozxxnv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gmghojknf.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gqhaxaywa.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gfgdsqpgl.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/govsngdcr.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gulsodwlt.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gtturgbmx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gyrwsetqx.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/groysleci.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gfduhhbdq.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gqimhxjfw.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gjgvnuinn.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/guktsjobv.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gyqokpjyw.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/ggoxjomne.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gehpigsjk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/ghxgrmqdd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gkiqyouoz.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gvrizzzwi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gpqzshtdc.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/ghvpaorna.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gpllrndcy.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gtheaflji.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gmyofufrs.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gjvypcmug.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxoxqgfbx.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gdqttsbun.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gjffngqwn.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gsadavnpl.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/ginjlyypp.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/grxxltias.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gpdlhsdzp.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gucsyrcsf.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/giuzuhmbz.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gxwjmafmf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/glmqqkdgy.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gwjllzezb.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gzjrkvsot.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gpehzfgpr.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/goyjqvzyg.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gxnhrvoft.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gdoaeqhru.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gbfgetbmy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gcrdbmjhy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gdenwcbou.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gwqzbbxqy.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gqtommlbw.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gqfftrbvl.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/ggaxszaes.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gyyjpdvmp.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gwztgeyeg.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gsokxenut.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gbquovljp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gslonksvr.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gwdvnmdac.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gdvmwucgo.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/ghcegkbhi.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gmyrqaisa.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/ggmadwbcl.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gmqutlccm.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gqhzyqene.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gibtwheln.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gzjxoukcz.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gepmqjqou.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gwinarbwa.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gdomijfgd.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gvnfcsujp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/glhidvqbu.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gvksetsyk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gpjfgrowm.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/guwormert.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gruoohgkb.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gejwwrawk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gmwfdxmoj.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/grbzriaji.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gslrlndfx.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gqpziuihj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gtujrzgqa.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gkdsqfirj.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gzmoprypx.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gtczvnxxp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gpeqrujzy.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gfpqyyosw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gjfhxmoif.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gdsbcpznb.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/ghupqusep.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtsvvczez.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/geidpdszu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grfwppfof.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/ghwovtafq.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gonkwczvm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gweztwqyw.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gbymdmwai.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gxalcstjd.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gsbiqxvxx.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/glvrtszxj.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gbuowpblv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gdnizbzwr.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gvdotkswz.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gznvdyobp.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gpsomvmzg.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gibnyzckd.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gqxanqxzt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gdskrrmvk.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/ghanofyiq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gnpenvrsb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gszxqcggz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gimsvsinm.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gcrrhtnjh.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gzszqguyl.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gymxtsqzp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gakbmfolh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gyuvtqais.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/glzathapu.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gddyavnej.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gugzdeehl.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gcyabamgm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gngzhcnmf.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gkrwcpmae.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gmracblae.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gffnumscs.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/ggdeexrmh.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/ggtkhrntj.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gjaxaincw.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gwnodupvg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gqcrgxbeb.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gqevnhtlr.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gwdkrhloq.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gdvjplapt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gqtrnavvm.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gsayksmvz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gjrkpjkvs.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gwvecydyr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gsyemrgjw.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/ghfsqokhn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gfcvmzgtb.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gbszyyvae.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/guvdahlhp.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/garkysrei.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gyphhkzrz.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gbjsllvjp.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gowgdywiv.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gzhblpfbu.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gwcxxhfgf.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gjkrwawhd.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gyatxjrko.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gowzdpisj.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/glhgqembf.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/goflgsksb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gnpwypton.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gjzcdqmnw.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gqxyfeias.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/ggarstbqb.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gvztrjvvc.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gexkgmyjg.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gtudbawma.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gouovqsnp.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/giwypuann.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gtckaukqe.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gohhsiabp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gkdbhtaes.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gnzdfwkwp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gohdehxdh.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gtcmlzgbi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gusbpjycn.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gcdrqcryu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gufpxwndp.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gnhjsxpaz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/geptdkvub.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gzxotnrlz.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gmvwhwrnc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gcuxtcizv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gbmxvbrih.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gekwlgvoh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gigjrdyxm.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/guncgtacs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gkuodnvjh.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gffebtdqd.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/ghfvfrqdy.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gfqzidiwd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gcfaskogx.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gtsxzppea.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqpmgokij.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gaezffnpx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gkhlismax.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gvqzedbjd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/ggaaqcjby.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqpptqjav.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gwsphrqou.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gqusexmox.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/grslpxrss.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gucvngnws.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gkioyrzkc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gvhapchiq.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gbguklada.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gkkbnsese.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gtjmpgcih.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/geuxfgxxa.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gzbpbuygv.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gfqadsywa.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gmggpbqql.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gxubztmhk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/glbpxuzdp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gutwnculw.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/geghjxfzu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gmfyxtbvu.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/govhkgxmb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gdrbbveby.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/grghvhpaj.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gdpwirpva.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gptuuexfg.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gehzevrmo.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gxtihqavu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gqivygrxc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gannlfosm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/glmomwmpz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxciujrgj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gjfeupblc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnimqxbto.sHtML


<!-- 参考信息 -->