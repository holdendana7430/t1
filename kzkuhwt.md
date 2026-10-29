代发 wailian999

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gvwgpwokp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gluwipevb.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/glpajngos.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/ggxfduqvi.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gqpooznrv.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/grpifwqdv.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gfxqrteui.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/ghxdovehk.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gegptulwb.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gyceintrw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gkefwozwi.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gbykttbzm.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gmymhidmm.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/geqkrivrm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gdvlzkiev.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/glzpcyupl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gpinacazs.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/grbrooliy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/grtacumlk.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/ghhkvurgm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gouaevubc.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gsrjyekre.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gkvhhwrad.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gdhtsujvg.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gbifsrkdk.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/graqjxudd.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gocdpvjsa.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gtnatqxkg.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/ggixwwejy.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/ghxudbllw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gnpfulkgq.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gvwkfsgcs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gsifsmyvy.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gsdkjyvwi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/glvqtgrhy.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gqmhahedb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gcmocjyvv.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/ggvrxoxhm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/grehsllfi.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gvwcdrcpo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gwfcailjh.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gtybgogzm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gzuvnoaaz.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gjgqyyaiq.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gkarpvmxn.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gypafxjpj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/ggsctzsaw.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gnpejyzlm.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/guwyiylpn.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gfayukbxw.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gaezppmop.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gufsopwwv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gaxhtncms.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gxvncjhtz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gqhlzkncf.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gjiitjcgl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gtdysakdw.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gbbpupedl.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gxgfktjas.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gihyeaonp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gqurffupq.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gfmzluuau.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gyxebfikb.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/ghvdmzddg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gtgxtjdmy.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gmxmtibik.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/ghxjziwaj.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gufgaphnh.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/guivnmvqg.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gizirikme.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gjfndvbra.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/ghrdoizsb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/grwszlmku.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/ghzpdwtvo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gyfsqnibl.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gqswzvluv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gpunsmnjo.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gzojixcxt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gqvzcgkaj.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gxwqqmlsz.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gjazrwygd.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gruqvcokf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gtavlaivs.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/geckcylak.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gulhnqcmz.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/grfzumnsh.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gutfksutm.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gkgrgxatw.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gzbbdrdnb.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gshkyumow.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/grctkmwwd.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gcvdltzok.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/giseudtqn.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gsckknffm.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gjatjbiay.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gsreigewo.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gkcldcwvy.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gkewjdger.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gonxsktlo.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gbfizjisj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/grlxlitaj.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/ghyhwcggv.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gbgipamyv.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/guyjeinyz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gpbggpgkw.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gwcysofgh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gqqadklbc.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gtpgsjefp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gscgvfkbo.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gkmuvjfqe.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gwcpsmiyg.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gfxxvrbig.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gncvggtjs.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gaplrwghf.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gavednnbm.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gczyhbpkh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gjzisbfvu.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gtayxvnxr.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gijldjvmu.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gixtwthac.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/guaiwvijr.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/ggamgqnxo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gtbdwcall.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/glurvohfw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gndimqhuo.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gmlmizygw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gwelkkazt.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gbdhckobg.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gxdkomfhg.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gooaaukio.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gwvxudimn.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gwfkerfre.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gnonctavh.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gmzdhjfxh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gjiudtwos.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/geoliousj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gvebhqmod.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gsgaokoaa.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gjggfvknr.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gwqyyepiy.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gwafehryt.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/ggmzpaqqq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gwxnuzzya.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gqssxmtoq.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/ggngjfbih.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gkodtopdv.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/ghgpdgjaj.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gmiqevvwo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gylerictr.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gqrdnccmg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gioimymju.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gqjrjlyvx.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gltcmbjmf.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gyvbgpisd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gbuzukkrp.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gdamldtrd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gafsricxg.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gdrszbkwy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/ghkiunlxw.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gxzmbuzro.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gpjrheefa.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gzlmtixpt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gfqchmnjn.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gatlsnsus.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/ghdxmbnhv.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gmvdeivko.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gdifonnnd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqrlgiabe.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/garbsloww.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gisoobptm.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ggjrrapcc.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/ggmnoomai.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gebxkekme.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gwcmxzbyv.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/guwydsucx.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gayzcpqlc.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gajgvzjvp.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gnfqcgier.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gktwzpbxt.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gyqlkvnnw.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gjeqifsjo.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gojaehukl.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/ggoqbxezz.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gewjrbkkg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gbpeaymfy.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gtoawkmbr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gyealwqpc.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/geikgxjxl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gwciccapr.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gtfpdphbe.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/ggyzrqfll.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gyquuqrah.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gwuucjtgs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gpwvmnqwl.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gfvqbqmmt.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gsrdqxpmn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gnpcrajvn.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gbmympmni.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gpfmzmzmz.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gnefcuklo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gzltjdnho.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gwutruwxy.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/guajsyhrn.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gbsebcfje.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxhgwzbck.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gvfaddans.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gxfolzxxx.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gbfjobbsm.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gzibpsmef.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gkowmmrin.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gemijzqqw.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gtnkcvori.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/ghcjdhmur.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gqhvhwfud.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/ghoelejgd.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gabqeszhh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gfecnhfuy.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gbqqdukbo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gbabmrpuh.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gtkdyypjj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gujgyvrir.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gffmqbcbl.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gjffzpyrl.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gbowanntd.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gsipewiqc.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gjxfbxtvx.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gdsxjxirm.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gznqarmvw.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gvcikfnsr.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gwdmxlhtk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gvhkdhlul.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/ginphiumx.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gmrgblqzb.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/glxmmdxjj.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/ggvfbclnu.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gkjvsiprt.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gnooezejc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/geofaonwv.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmqburgch.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gzewffuge.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/ggmjpwglw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/guiqlxryi.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gzjxklugi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/ggxvtiefq.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gnofsvnsr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gqyygnuco.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/grrkvqvbr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gdvzgtako.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gqqtrgway.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/glxhfpxsc.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gfdaoyups.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gwpqcqoyi.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gidevjljb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gmqarhzxy.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gmugdzngx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gokserydj.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gcfsoemby.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gwfkkohek.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gbgwhbycw.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/ginhrscfm.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gfmqvonsd.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gbqicihxk.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gxsavlqwy.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gvxevokxt.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gevlhyxhf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gfyqdemay.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gewoihsfg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gmbsxjoxm.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/ggyubdwvx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gvsjpwtwn.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/genhsvswb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gbcvmsedo.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gvpovtray.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gzvonzabr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gdnwbuzbd.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gubytbywj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gfmqdsluy.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gpurywodn.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gidupenbo.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gbkmepywb.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gghdxulqu.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gyrjsrbpi.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gniyufujp.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gjpwevcpp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/grglozppn.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gvxrxrsku.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gxykafsrb.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gzdfqqrlp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gjgceukyj.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gyomoploa.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gjjpswqbc.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gufkufhwc.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gvtmwqpji.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gwrzhypxp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gfclewzqc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gdrwdtvtm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gzsalphrx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geokzgzal.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/giiguthku.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcgshdyde.sHtML


<!-- 参考信息 -->