代发 wailian999

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/ggyowbvoi.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gndxsxeyf.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gwruwvrfh.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfwwwfqut.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeayzije.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gcvforara.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/ghnqyluut.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaouelupt.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gosuetjim.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgygikiu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/giporfbvy.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsybsdgg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ggfxkbsst.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gtksikxlu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbwuhxtb.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgxtswfx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gukehmlll.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoulbltw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ghwovpjxg.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvicaudj.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxyfnhkr.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/guwsmqboj.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlpxlopf.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gtdpjazah.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gboljuutd.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpjaaivqb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gwijqbbmo.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrzwjwea.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytpeppbq.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzlkcfyd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmjyspfr.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gucdcgyfm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcyvmwdde.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gqcvpbopi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/genseoozy.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdufvltjf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvharwcmg.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhzkazln.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/guigekgdx.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfjbxkgj.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuxmwhgn.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gaeoolxbh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gybsmoqlf.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaakxxfcd.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grwbukxrr.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwfnocvx.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/glecinuag.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxhcbnmg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/ggqhhvjuw.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/ggxysiunh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghcqnaqvu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoelkfbq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlefaxnl.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gftbsmgyy.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/givipsiqo.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/grinrshki.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjbymhlp.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxmnbvfm.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gefjsebak.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gntubfiwf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gucjdscfn.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzztfncrl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsrygocx.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzgtzxdzm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkababxk.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhavujtj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxbxtllvh.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuipamkj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxymhbgc.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjmrgcsl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gdrlcnxii.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gtufqvdvg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gnylbesxl.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxxiktit.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxeamqmj.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnlazcyew.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfdjdoks.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/grnbhdpcy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxkccupw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojrzaias.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gksowkzly.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gwluqikbw.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gmseqklfg.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbeikpfb.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqlhcqmu.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnynzmrl.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gylngcymz.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/glberxhav.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gymossveb.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gmbtnjqhs.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaakmtezk.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gqofzafzw.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkllmqam.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gxegvcqdz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqgymgeb.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqpispcu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glchnhbjo.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gvajplzvp.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/garxkohpm.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsanajmg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gjejyvihv.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdatvugjh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwzjyizzu.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gzdykzkwr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gfbqiavsv.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gawnohdhn.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnnacbcc.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gyqsjwdra.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gvyzvpliu.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpnkkiqdj.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfhqrecx.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/geqgduizv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmwpvjnl.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gwcqdkicz.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbrjxwhn.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gxabxpiqz.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacnvzzqe.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcolseqt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gvuftfbcr.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtbercnk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gumkpebjk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdtzleva.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/guilflvuy.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/ggpllxohs.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gzldgofds.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxxuitlcr.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/goqefjbrn.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhisdvla.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gofvcxazt.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gxzgmwxrf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnbngenk.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gikgacsre.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/giffvwstm.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gyizaclyv.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkefpkfzh.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhapuutq.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gysqbvkdw.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giliuqswh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgfbxjmp.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/glqcryyqx.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gqjahebiw.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gfjulukma.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gaedlkqmx.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gnpfrboqj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gswovvyde.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehugklhf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzzgsafs.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/getetpjqi.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpkcupcr.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtkoxtab.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gopfogrna.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxhqqgpe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gocxnkftt.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqycxhmkk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/grjncmhtw.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gvllctdri.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/grijvtows.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gujgazphh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsrvdaakb.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtrhrtvq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gglzqqgvf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfvtvbeo.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilxrelty.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptobbbqa.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gahnthnkg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaqsbyzc.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzpateue.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/giscvhipe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfhbbsiy.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gxclxkosg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmdcgpvh.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geevdnyfv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjslctkm.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnomjwvh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpelmcsb.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghainwhht.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtymbdyxp.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gjlrspgkb.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoffelke.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkstituqy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgnwnxqe.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlxnzvlx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gpzbkcjsy.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/grnpdifrp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gsqichanb.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gtpgmflwt.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gvqnqykah.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdgpuxjl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gjlejskmg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxozvlbc.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gbcrfcbpv.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gowliuaat.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmguedbah.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/glzpazilh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggemlryep.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gizwhubwr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtzweucf.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwxujaub.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gsiocilof.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gemqqjiyw.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/glukhvyeg.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/goccxqvxg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszsrkiju.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/golukaoar.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gotlfgtzn.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijxyrwua.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gbnxxmydv.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfkzfznz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnvhbwjk.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/grcxnhfae.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqmxahyb.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/giixwwbsi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmmslojk.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjigexvza.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/givfijnye.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/giqbiwrxf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteqppsye.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvdccwrj.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfxqpakd.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gqagmifla.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gbpbfwxzk.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gycuduxkr.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gimhhqvkx.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbjxoann.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpafizkgh.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgllfjgo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnthtupu.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/godkkqvkn.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gujbslzkz.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpqgmbuj.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/guegjrwbx.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhxmfscl.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjovrwaz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkwdwwkz.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gavnxfnoh.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gcxatbeab.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/goysyrwdq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwbgsugy.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gtkhhejsy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gltzesuhm.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzifjkzt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzbpzzcr.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gwuvzmpcr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gygyxfdtc.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gdezqimtm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdbjmyqa.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/goeudeetr.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnctnooe.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ggztgpnhb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gsuqpdydw.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaimanfw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwwweygc.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcennnmyw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/goncdibhh.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtgctwplt.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gmvalumzn.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gxymdvzzy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcqdrvyu.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gltizktub.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcfbvzvk.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhbkbmpy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/galfcmuds.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gizlytdda.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goztbrmij.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhsvrdsm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzblllddf.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gliyzhoxf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gckblthgt.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeiwdxuj.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrguvqtc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymkcqdrn.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gadlughuw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gntdnklld.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gfkmvtync.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/giwdnsafy.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gehirmfec.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkowxxjid.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgfprrou.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkbnwdfi.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsnaopqt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gkbkjradf.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/grtlxvdbp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gcpxleaai.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/ghspqjksd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcipqylvl.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylsemqjw.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnalzjovz.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnapnqhy.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpydrathx.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdlqzcpu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gklqpyukm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfgeooii.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkczphmiv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/geywmnsvd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gitwigner.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghymmpoti.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnctlrnrx.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/grgzgqssb.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmbokenvr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gliictbbc.sHtML


<!-- 参考信息 -->