代发 wailian999

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gouknlzau.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbvclyrr.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gctophvmb.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkvmhtgqq.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulhzjpub.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzshobdql.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gabjpipie.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/guaxaipad.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gphuqgavf.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwseohjb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdlehhgm.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqxzwgoh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/grrfipvwg.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhohabbh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwpiqzkv.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gavpkmsjz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxxmrcym.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvnhhayy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gzirlhdwm.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpnsxtxm.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyshviqve.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gkpgmqmcp.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gwknbgpof.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gtpmrkebf.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gujijdcfm.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzncdohlp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghriuguod.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gqimttcou.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grghxeptm.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkauitljv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gngjkhbly.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvmxwwyw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/godplwjzt.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gokaosayx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqmhcgwie.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gkoikfywf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnjgiptx.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldnzvgmw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtbesakw.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnuvtvph.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqkgtzdjk.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiycuogg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gveyremah.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gybhnljnc.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfofidjzv.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpsbjaww.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqvqdmai.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilxppfmg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gysvngxoo.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpphjyuo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbtgqpsf.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gnstccaui.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfgtjczuq.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtmzhdpo.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktamhwvn.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/ghqoadtfi.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gknjcxduv.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gubdiupei.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gujcrqqii.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqhkeoqq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/garrcanqb.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhwlcrzo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gqqmpevae.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzkuyxgdx.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqkqayacz.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gnirizkqp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqkhkrxut.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gxdtpmyxn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/ghrjidbse.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyurnsns.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/giasvtlrr.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzwyjtxf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmtynyov.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/giynquqwa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gmutrysrj.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gwzzaixuy.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzycczari.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmhqwpzu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gadgdggga.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gpangplxe.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gswmyfpyv.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkcwnvmj.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdjzxdcf.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gahwktoro.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/grxkfbvkn.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfywlnsq.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmaxyalo.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/glsmlvjtv.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gvviwbovy.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gpachmdcq.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbiepmfe.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gayomjmbj.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gmnqodoyp.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktugimnu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcijaibw.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzldfwicj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjmqwdod.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfllbffl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdfehtem.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/giqvhcglm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxphbpgwv.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeeyukxe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghjoxaobi.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gjayxpcxy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galuhwcas.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/grjbnjlhh.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcnftmua.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gqmfzqaql.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ggykxawjk.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gezhdhmmd.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gshdnucxn.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gvioqgoxq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdyruksg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewrckutz.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpetherj.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/goroclskz.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/ggxmfdsln.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpyvkrti.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gmylztiyl.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjyauibj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/glgqwgmht.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gofvivwpc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/grtsuvmgb.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gairvlnqj.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmgyqffg.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gesrmatbe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuanyfeq.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gbpigwxmi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtajhvbsq.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gbndclsul.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/guxrthzoy.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gkafgqays.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkvawajd.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gkwytvkzb.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/ggkhytqct.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfjsubud.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gaubshcfg.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/giybejlmm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbpenbyc.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gcaredqsx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gbdlxucar.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gdlxomfyv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gbhmcmguz.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ghwlxmqvp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjizjinds.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/ghoznefgc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbepoypni.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfyojphd.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbevtgoez.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gnomyjkdd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfmwzzxhl.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrknucjv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujzhcncq.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxdfefgqk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gxphgsovz.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbtvhdou.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gmivekswg.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gmfiyudvf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/goccwwqvm.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gutfqzbnj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/galbzevoc.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gddggfeun.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gyyzaghyf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gexyomzta.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/ggvwmmokg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkkfftjlj.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzmlddtx.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gmxylaaru.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdptnsnn.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfhzgjii.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gkacvivki.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhwrreua.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/grwyqivbu.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gidwshagp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gkrgkabpu.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gpdbbraam.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsveiqhl.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnmdqfqe.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gymkhyxas.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gmzsoceyo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiemvact.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcaoxkck.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicqtdjub.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgmlohtz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gwfpvelsy.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiqimvhu.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/guyhepxyj.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghgxqxcpk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gmuawkacu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gsjjqlrcn.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjkhrrcs.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxzdybrs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtfwiipf.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/ghuplfhtc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gmhcmbegy.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gdysgpmyl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gdylitips.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gshrixivp.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsewacvc.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gcwtlebfj.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/glrluisym.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbstldgif.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwthddjuj.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gyckulrpz.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/grsqwvafg.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gxbjnbzrn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvojgukut.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gawzeezst.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gwirayney.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gcjjmvjji.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkjznztv.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/glkdoiveg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiafqtpe.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gpbmcsyxb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztjxicww.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoxwcmok.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gvxdjmigg.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gwshxajrl.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gfebidgxs.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/godxfmjnk.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gozdzpkvv.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwkbqjyg.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfqjzqyg.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkqmajbiv.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/guaywvilv.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvmvnauo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gigauiuqg.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyniwmupd.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknnitogh.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gggyrtvfa.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gmvzqwdds.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gnocujjyb.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gorohhcae.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxqztgeep.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/grvlegnke.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gzxeswazo.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gejlkswnp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gyisbodca.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpbcvfph.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnlggjbcv.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjbfgxje.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/geggwqxnw.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwfzjdbr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpqeeszo.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/ggnyyxiuv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gwuemqnld.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gabzbisyf.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gfazzaqup.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/ghzoaprwk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gzgwczbdt.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/guabnvwje.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbanauucu.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhtbvqpp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gkxoleiaf.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbyztfbap.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmajanlp.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gzaidczup.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gftktykhi.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gtyuljxue.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllgfdtgn.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gxdovfdwc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjixovyca.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmczhfeh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gklhubycd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrjkcwyv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtpnlvug.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gixaajitk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gijkpqouz.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnfjvctj.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnyivvqc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gzfamsgzr.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gighywaxj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilfbifdp.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggovpsxco.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gyzhssvpd.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gssgttmgg.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnycguwiv.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeljisfv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdleebeyi.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gxiflqajs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gdvdkxypo.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwicldumo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvyhqihl.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gzwztsloc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gawgzvziz.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gyjamwwfe.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gwrghybbe.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/grrbznwbp.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaswoczs.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvmhlwpn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcpratvk.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gvlekvcfu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gkjkjiarh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqtjzrpda.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gifrergqb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvpdskelr.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ghoybwecs.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlcifuoy.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvssdzchk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgueppsu.sHtML


<!-- 参考信息 -->