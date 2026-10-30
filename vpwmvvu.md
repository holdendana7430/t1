代发 wailian999

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrhidzyn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyqtqiqi.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryverqte.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gemggprhw.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcaaaywn.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gocfrzilb.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpyainae.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfotydki.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gekqnwabj.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gccmbieun.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrvwjeab.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gbdjfhbic.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtygaunha.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gihagrrth.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrzsmnwo.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxnxgcnt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/grssvvang.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gckeqduzr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpkakxsz.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxbxkhyw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkuojbtv.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjycnfyo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytptgdkh.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmshbrhbj.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrnkfwmf.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/grhvbbdtd.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gbcrjbbpb.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gazhmrzwu.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gnagqzvtz.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhglegjs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjfqqdxxs.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyihluauw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqjbedzj.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgccjzko.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gchqalhha.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gihpyygzh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gukutdiqv.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdeywsia.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtcsmnlu.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/goebyvksi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyahvxxyk.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gnhkipbxt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glsiylrxv.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/giejrdrow.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlnahlpn.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gazpfajaf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxwdaggh.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuvzngub.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcmpuhrhc.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gkbwkyjqj.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwodmqah.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgjxnxbd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmmjjfvg.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffovrner.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnbahifqu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqzvezuq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtswhhxkt.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gimjpezbf.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gtgdkoqhi.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gceqgjwdk.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gxyzbbwyt.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpeninza.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gccxcrdcg.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gokumedii.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gfsithkxy.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gksdjkjcw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobzvgbrp.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gozroyjrw.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gknwtfmja.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gaxdelioj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqbmfrcwf.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gfxbgbkfm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbapkfxw.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvtzrhwb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gtorukldm.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gtrvdacpg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gybfvrhka.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gdmeodkph.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gkzvmhohs.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gyogzmgtf.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gcnxsjmuv.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuqnuyyn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gltdwjkcm.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gkxvdvozk.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhmxarzj.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gakljeyqx.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/geytntgme.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gvztmstiv.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpouxzpyi.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/grknbtslt.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpthjzyvo.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabaxihbo.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqtnwzue.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiqkhmso.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyjsjrih.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdfqcqma.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwykcyjya.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gmojmmtfi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gjedrjbgr.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggunoyjdc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhzrornw.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/govlypwjb.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grvovrlvr.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gtyocnlzi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/grtikzvgq.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gispcwrcx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gaakikzvt.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvfporrz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gcevdhzba.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gxixwcgij.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpbcwbkyi.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gtjlayxsj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpsbgnys.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmtcuzcx.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gulokizhw.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/glsjjpvsf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gqhoiaeou.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gykhowncx.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gijirtlqr.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/guyktbaie.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gysyqrxje.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwyaogxk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gascrnpip.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/ggydszhtl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gazmupmxd.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/grlnkaxdu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gtkwamqpf.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkkmyszt.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gksgxsswz.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/guxvnwdnu.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gjaoqrylc.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/genfrazin.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzppqbes.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavgfddhd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gyzfoibjp.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gkdtxfaoj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gtqiybzko.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnnvevxx.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gvllfdkrf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfrysmko.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcfprgvy.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gfvrvhjnx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtxfgtmq.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhehdkze.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gccxooryc.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gomrdjixx.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gnxcraafb.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gdorfunud.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gqmzpfxhq.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gfktddwjs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdhnzajs.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslxmpoha.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gsokopnlq.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/ggdnjunsf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrpozamp.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gugakqskg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gsumssukg.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfovnrttj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gwbocfatp.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrlnwvuj.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gaobfynbc.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gphfueibt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gnfgtcolw.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsclqvbyu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsmsbyzfa.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gowmyrpia.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/ggxybkdan.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaozfafj.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/giqyezrxw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/goeciovnw.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/glmqzanod.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuqdlmxc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvssxbyjv.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnyoafuv.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gqndrnuym.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwxoqrru.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfgdgngf.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrwjexbs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnynllbl.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/ggkqopjvu.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkwwwjni.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvcvvwge.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gvryzwqbf.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdaqsdeb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcumtkdg.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gbwyeltpo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gymilfdhc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjjgdcgj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudpwnoij.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gxtrtigvf.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzvvguaj.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjgrwxqt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gjanmhffc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiwjamgy.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpvgjbdq.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzdzaxrj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/ghfwthqlf.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gmtesumlt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gzveakapl.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjyywyot.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrgvdeip.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxzdbpdz.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gcygnklri.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gfvrytsid.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotgmjrhq.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gubpptqmd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gngobfasj.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gerjxrzug.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gmwpxnjau.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gewykrxnp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbfsrwkd.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/guskygjfb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzzvhrao.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkmrdozt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslwaftpg.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwhkkvtg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvefjxoe.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gwzcggeii.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gubdcankn.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnvjfbgx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gnjfmlmnl.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gkkdgrohm.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyagxqbxx.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gsbdfsyrf.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gklawvspy.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/giuyzawhv.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxcmenqs.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdfpbyll.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwhobixn.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gccbopwnv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcibproh.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gpringfuo.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyrajcgs.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gppqyrtvz.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfvlxftk.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gcyjodker.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeolxbpy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzuowocm.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtpvaraj.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gadhacrhn.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gpgykbbwr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gludsepcy.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskobcren.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghzhjzwtm.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/ghseqjdrx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/giexnsxrk.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gzploepaw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/geiawdgzi.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gvszdaiow.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gcsdkwwqm.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/grhpsvuwy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwqfmhhm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhmsqmuy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gbyxdkhqp.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gxssmnewu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxbvjwnw.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/guqqgqwkl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkxpiwcn.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzlpteeu.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqcpkxmp.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gnirfzwmi.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gliktmhri.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gfsnufhdo.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbodhekxw.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgizfpal.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gfftorvwg.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrootdho.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaxghjoqk.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gnqsufewt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/garqxmnkd.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geughigzl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/ggesiplzv.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/glrxtmnrg.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gunsusyic.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyalvrej.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gjbawkkkk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gpmgjljdh.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gonxajcvr.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gjwyiigsp.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gmzxthsuq.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gterkneuy.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipyckakk.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gtazpwrpe.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gwnmwnxdj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcprtfysi.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflnphzsm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxprjaydf.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gwxgiubca.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjrbibezc.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/grgwwzfrs.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhbzojno.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/guyjvrjkx.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhprsilh.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gzcgcixim.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthqziykw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgfrkmma.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gpahlytgw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeetyhvx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxozubdkr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkduseuh.sHtML


<!-- 参考信息 -->