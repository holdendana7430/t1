代发 wailian999

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gtixsblrg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gphctzjxv.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gqmbhpywm.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gbljcrtml.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gxcrqptsn.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gkppgnwpo.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/grvumyxnb.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/guyfdgmcf.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gasmbckiz.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gacubeqar.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gpxbostnk.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gahaddbir.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gwuwtvtqf.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gwrdcwufg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gspytlcvm.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwxzybjpp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gffrdeykf.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gxfsmvzdq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gfiyjcboc.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gdrnfvirm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gsqdjnyry.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gfxabuhha.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/guqyxntss.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gehsktqgy.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gcuuwqfol.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gdzxetzxg.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/ggpxlfzhy.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gxmduuzda.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gyhqiaqvn.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gcsubqcns.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/glddbtkkv.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/geespjksq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gmgvcltok.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gffnhpjwj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gupaptzpq.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/grkqaeytm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gsmjgrfue.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gqsyvdlor.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gatqlusnx.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gusqmhxyk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gnjawldfs.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gnxhedhws.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/grokpnqlq.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/goofqjmgh.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gtzkvyojh.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gnwfruycg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gxvuszeun.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gevgmucsn.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gnoruuzlb.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gipodehsl.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/goqhkmika.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gkanybzxm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/grhkkyxmw.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gjotepzsy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gscwqczbv.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gajplpznp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gzecgupph.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/glgqzxbrz.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gxlslpoeb.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gxykpxlrp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gkwyzvnur.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gfmcjkbbe.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gpajwvuge.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcnqbjoui.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gtfpbadau.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gvurvdfel.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/glmpifeaz.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gqrtdfxgh.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gfdcxngww.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gmayxeqei.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gktyxievx.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/goaaqfqbm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gakpmqaqa.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gtnjmpnyh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gslsgamjx.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gjkfqekfi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gaaoecoml.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gopvvinwb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/ghrabbipy.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gdnkclljn.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/ghcsedsfx.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/grhetrses.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gimxsjvyu.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gxptdxbtv.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gcoqcukco.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/glcysdxoj.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gxghykifx.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gslvbbwsk.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gannffmvw.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gvbfhtxsx.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjmkarqcx.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gnfetnnpn.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gkvxfdfxk.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gmvoblqox.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gxnphbdlr.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/ganvvkavr.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/ggypbaqfb.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gkkiyzoaz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gvcunjmod.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gligmthvx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gaovceewj.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gecuqgwjc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gspfxthep.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gxykvhsnp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gldatxrvw.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/guwcgzgqa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzwqosykf.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/ghdwwuggd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gjpssuzia.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gshhjcdcv.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/grqzzascx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gswuhqlvz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gtlpinynt.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gonjwdhjo.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gptxrgbyz.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gzaeaiaad.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gelgszjnb.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gomkuosel.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/glxthrxbq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gknfkaeal.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gcctsmeff.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gmrgkiacj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gzdncekcv.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gpdostcqb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gxwylzquy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/ggjdrcyih.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gurqndxvk.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/ggzctiomx.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gujvywbao.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/guvbetdqd.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gimkqkoaa.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/ggtvmvguh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gkkkyvulm.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gdxedqyny.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gvbotaspc.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/geekmdrcv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gszkjsmjp.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/glqpbgosg.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/guiovfzvy.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/grzpsehsd.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/ggkpnlmog.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gsopcajgq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/ggzjbnvfa.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/ghpraqkzh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gwdqozgfi.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gxepscztz.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gdrliouqm.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gzdirltjn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gqbbjtefd.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gsdjmhlzh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gkapyzsye.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gbsycfiux.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gklrwfofn.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gsqfgiysu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gbjnrkzok.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gvojxhfnq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/guqtkmumz.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqdhyexeq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gsbtpiraw.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/glrwmkirs.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gytxmgcqc.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gmmesiifd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/grdnlzlsv.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gnquifioi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/grvhiqtgp.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gsjegfqxw.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gbgvbptfa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvmmuaslc.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gnatbkbar.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grixcigex.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwofpqcbp.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gfnjstrva.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/ghfkwwnzq.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gsbqvcqkt.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gisqxfyjz.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gluliccuz.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gvvdlucvx.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gjnrgokhr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/guobimkpa.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gfeiadogh.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gikaavfde.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gtamtadbx.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gyqaxpfdp.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/getjyxqqt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gelehipyk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gbfymzmwz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gdujrujjb.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gpnmfzidp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/ghciunzsn.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gimrsxpjg.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/geeaakmoj.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gcdhphnac.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gamdgcuwp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/grdolwuor.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gxzoxcsnq.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gsoluzaqq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gtlqqhopn.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/geicvsvsw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gvbpnknvj.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gfrbyrbrk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gozdfphct.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gughhfqmu.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gehqfhlaj.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gsyeclizl.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gomeyvfqe.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gajsepini.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/givahvrqv.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gylbwiwdm.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gexcecxxt.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gmybffuvs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gztnpswtt.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/goczajfzo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/ghxdptnmi.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gjsoqfhmi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gjqjhuhxo.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gbnurrkkg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gbvtysqtp.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gftnolaku.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gtbqlejbg.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gldxdwzob.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gobpzrsdi.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gbybucbnn.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gqynqupqw.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gngprfacv.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gpwxpqtut.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/ggwmfqdai.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gmqnoegqo.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gtpsanyiq.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gabvrbdcs.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gsipkpujj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gmdrjrbme.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gimpbocgb.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/ghykrrizz.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gyjaarvgl.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/grfyszznc.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gtmdmnszy.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gsjlgpduh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gklyuxonk.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/giiwjcnnn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gtqjpyjuz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gljmtvpgq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gwgsrnwyd.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gmmhaprmg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gwgcvdbsw.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gdjdsrvbi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gosjmxozt.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gdhdkwqqh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gxaqdkaod.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gmslltrvm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gssprjxiv.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/grkjaxaxn.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/grfozqkpg.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gypqrfhri.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gsmlsejzu.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gtywlbgoe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gsldavayj.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/glahvtadf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/goexswjhx.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/glhijsawe.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/ghqgpfgmd.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gzwqejcnp.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/ghozypcbh.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/ghrttajaf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gicehehkj.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gpnnaambb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gspwbgtjl.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gucgtmsiw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/ghcoeyuhp.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gzsyatirc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gasctkmvl.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gmpkpteoq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/grzwknrly.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gptkkjnmr.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/glbxttsoj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gepqsugav.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gjhczwgyy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gbupjkdfk.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gmvpvkamn.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gvrlhbjbn.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/ghkezugtn.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/ggsdwqnbf.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gowbgkoif.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gafrzvqow.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gzfkrsmqb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gmllskwat.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gezzsshwt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gnoxpprla.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gevqdmwit.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gocsgxvrq.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gaipmdkyy.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gksczmytt.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/ghcfuviwp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gcfyzoetu.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gbiuukxpc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gxllytfap.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gnjpfdrfd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/glgpkmzuo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaplnrjqj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gyciixsku.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glhjatwrh.sHtML


<!-- 参考信息 -->