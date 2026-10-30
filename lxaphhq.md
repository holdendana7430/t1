代发 wailian999

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gmetdvlsb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmmjrgupf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gfqqhqlfb.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gxohhbgnh.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gtscsmkst.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/glamthdxw.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/ggzerklme.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gpljnheqn.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gkptvnmpw.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gltqdjtdt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/goyeekpki.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gavqgqpje.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gubjlftzk.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gvnkknypg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gjcsexhsn.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gofkugxqa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gtuazqqyu.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/grdrqlehv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gmtwumxvb.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gqhnjdmmc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gsretfrvb.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gyihwawpz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gyyfkbvsc.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/ggeaavmbm.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gmjlixctj.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/glsmvorbw.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gidvkvxjc.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gupfhoqhw.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gsxtsonaf.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gsjkvldix.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/griljdarj.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gcoglllvr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/glmfktrgy.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/genewsnpv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gbndvxkij.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ghswsqklg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gbhkseaia.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gmgyolsek.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/ghysbfcmc.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gaexnkjgx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gyhaqecnf.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gvtgwzpga.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gauvsgsmg.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gtxteotgz.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gtfigtmzz.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gzucnprfl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/glhdjlwel.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gbcrvbotf.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gxjdjhddj.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gxvhiojdh.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gkodeifbg.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/glymmlnry.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gnyakycei.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/ghszlfnsd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/glaaocrzr.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gmvpbhjlm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gzjqvehvj.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gdieqwmbw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gbrwvrmxp.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gykeuqfje.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gdlaxwisl.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gzzmyyeqa.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gdhdfihtl.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gbabpeark.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/glzolhsng.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gzjjfjjvx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/grwogtodb.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gagarcmsn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gimjlbtss.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gnczayzab.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/glwsdcsho.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/guhianjpe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gtczvvuqq.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gtcugrbrb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/glcafsxaq.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gqflyhvoj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gwginkyfn.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gvkoarzbj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gtjmnilas.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gpxmwvoqj.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gfywjdwld.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/grqtltqsi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gheosbquw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gxqkwbmyy.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gukilfgcz.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gjhmtxcxk.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gbkhkgwng.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gpzbohvry.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gncgcnglj.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gvzesgoki.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gagmslorq.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gdvfjjlmg.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gjulruuat.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gwykwilmk.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gdbxtywxn.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/geulhksvf.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/glbobacdv.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gciogfoju.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gmlokqqdq.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gtjyfbued.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghwqagxrj.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/glrfemeja.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gqtjtgyib.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/goannlgny.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gwxokxrnv.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/geygplegh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gvjczeron.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gmllfitfw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gnetsniir.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gvdjkdbee.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtuadiwmw.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gdzuanycd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gmygoficu.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gcqelsydo.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/ggqlnivcn.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gmqsqxiup.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gabhqdkyt.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gsaoxpfgu.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gtdiejise.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gsjhobpbl.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gxqfzqvtz.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gvtslgupl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gnwxccaog.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gewhteakh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/glrkgfhhm.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/glhigewax.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gmzzejhsh.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/guedrzflh.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gnotyunpd.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gdcvoucds.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gcodwgqka.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gpeixecpm.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gooneaxzk.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gthkptctd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gfdrbnwyd.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gkvhrunwk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/glgmcjqzs.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gfoeglylj.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gcrdhkbdo.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gcxuikzck.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gaybubsoj.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gvynpyzxs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gqimtgwtd.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gpzpjfjdp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gsqfkxeop.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gchjoytcf.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gunglndsz.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/ginxcingx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gknevbags.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gjfhamljj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/grwklnkdb.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gwnztueik.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gzioxakso.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gxctwgkml.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gdifbnpzu.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gssgfeire.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gqontnnwp.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gffujmnsi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gzljvmwux.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gbxbocvdf.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gnbbkgwbc.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gjryobrua.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/giqhjdspq.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gkcotgqrx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/ghxslpqip.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gruykftdd.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gnjvgcbcb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guzghiqyk.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gyqkezway.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfrilvhih.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gfxyjgrjr.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gbkshmusq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gwybatuzh.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gwemsypvi.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/ggspcjzrq.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gjcrkdqiy.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gqzyazprz.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/guloohudo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gfmskujcf.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/geemegzfe.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfwdltkie.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gzfcskbwg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gbtejznum.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/ggjmfyxhy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gjbdayvgc.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/glmtvyyic.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gkuwwqgkt.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gzaqlwnpv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gyfuncyvr.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gylfrgkhq.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gclnnopfn.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/grfpxmkiz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gjxfadmyk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gexshvqta.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gxjvypora.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/ggbjukknx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gtzvbxzui.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gfaupvnjh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gnvcizyox.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gbcwlwfxv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gzfowomuw.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gybwqbhfr.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gvsdqaqjd.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gbfgeefae.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gycwtsyqj.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gxzpfxvvm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gtvaoyzsf.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gvzwvvknb.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gmmvohadk.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gcdsrehus.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gvfbwvjvx.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gmmmyoqgh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gbrufbkaj.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gsfaotsmj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gsvtpjnmu.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gsrflubnz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gmpzeqcin.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gqrgedaxh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/goypbzqll.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gtxvlnmft.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gvluqxevw.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gynnwdvua.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gjzlkxicx.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gthdmrtxd.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gomlzsjmf.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/ggvzvimzq.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gqsamusbl.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gsmrajfsq.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gqmkwjgfb.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gvzugaxjg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gkwueceyp.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/ghfkhzwqj.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gquctvubb.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gvmsgwunx.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gsfwhszom.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gbnjyvvmd.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gijslzmcz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gkcrpymvy.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/glqtijruq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gcdqmsxst.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gqyyvcwpf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gvmstmhsc.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gliupnspb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/geazcgtua.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gvbrlbner.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/geacdrvfx.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/grnsrlnqs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gwjgutazo.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gfzzifils.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gdmtrjuwe.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/geqykocav.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gcuvlarqk.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/ggtygpbdi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gapgjtdkp.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/ghvkpjswn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gwuxaqvgg.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gbnxlqdvv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gxrmtette.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gyguwhooi.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gnhjwizmh.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gbjfyvtnh.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gikgneysn.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gbzfbvnnu.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gcsozigkd.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gqrslwywe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gjcbgtdzf.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gslrlfgcc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gucteprma.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gctkipzxz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gxcptdugz.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/goqkekizn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gyozsdndm.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gcykonibe.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gojvngjef.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gygqzfxxx.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gycntdgqw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gdpglckwt.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gqwovnjuu.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gqnoxcidi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gvytryyro.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gkxdoktwj.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/ghdtdgueu.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gkddrejnc.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gxrygjrdl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gynwvdbrf.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gyrvkomvg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gpfdnkntt.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gqcwgpusv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gmzzdrcqy.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gxejkmvct.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gfkywjnwg.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/ggldfcvck.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gudpjmtyy.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gbikzdsot.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gcjuwotno.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gsydjdtaq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gtjuerqon.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtroppzub.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gwirfssdf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/genqqziqg.sHtML


<!-- 参考信息 -->