代发 wailian999

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gzgmgojms.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwstaygbv.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gbwhyaghy.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gyelsoddi.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gbwvpmgzf.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gkyhdgsln.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gvupmgzpe.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gaqpqkxmy.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gyzzcjjvi.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gvpcdhddc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gjdhaglat.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/ggfmfiezn.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gazbbciuw.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gxebikabf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/golrtkpnm.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gbvqetvsq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/ghallpwcy.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gehjtpkac.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gcmxcupna.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/ggjswaqry.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gwpczsfif.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gxxtfdodq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gstooubax.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gljfeucfk.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gfqmhkcsk.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/giovueirz.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gfqgznowm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/giyidbuaj.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/geejccdgi.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gulgjkoho.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gmuygcwfy.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gofecgybs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gbnauqavi.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gwlpeisnr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gavbuifom.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/glgbyqzec.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gwyvmbwqm.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gjypfjsmd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gyqcejufn.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gysqryasg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gdzwblogq.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gouidvuls.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gntgmwrvu.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/guvftdqxg.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/grabmwsur.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/grtvnxquq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gnkakbpiv.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/genzsnyoc.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gezsqitxu.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gulyncwhr.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/glersjapu.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gzbeyibhz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/ghgyurupj.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/guhoauzmo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gwwevthbl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gxrrlkyha.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gaavefsla.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gptxnbknc.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gjifmhsec.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gvsjxgkxh.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gfcoarzvw.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/glfkhrekt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/giyivoltw.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/giqcciwix.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gjytopfst.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gyypjiwbc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gjtiojwii.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/giqmnacii.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gdelcryka.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gjcmntfgf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gyehodmqp.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gkhuultrd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gieccbpuc.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/geswtmuzf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gwjtgoluc.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gydszabcm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gwrvkegsh.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/glieqqscx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gxwmdhtot.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gsaccsbzz.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gvppfeykv.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gfrtbvbun.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gdhyxbkre.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gxtiqjsxp.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gvgiwafjm.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gmryhycgu.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gfpfgjyqm.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/glouyatap.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gsgqgqvoz.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gtxwtapvo.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gzswxuucs.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gjggudntj.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gktzqwbsw.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gswdghpei.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/ggmygfrcc.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gjsnfurof.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gcwbonhom.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/ghrnpmqxc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gzavouchc.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/ggzsjmtgv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/ggenqmckx.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gpdwncgun.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxtgwaesq.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gxqqydhao.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/ggvqclmtw.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gunzmyark.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/geknxgiqu.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gsvgofmlw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/glkvcfhqp.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gseqzqpwa.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gbvevyqkf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gjctmvhxn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/ggerokegs.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gdvgsqctr.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gjggelhcd.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/govhomatd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gyneauxml.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/grmetyrnz.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gbrheejdw.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gfqzxwxvk.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gpiezkcht.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gmaqgvjdk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gmjkfbbfo.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gdnmffgfs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gctddqnzq.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gdczyyfyy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gssplqlmo.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gahxdeyxb.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/guugjasfs.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gidlyuumb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gxdrkhgyl.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/geyoffnxe.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gvaxqvveb.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/genragtyz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gqtuewebp.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gtsychpqi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gtpfluifs.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gnbutzaeh.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gjnzhbilv.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gyrrlpbbg.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/giskaeahk.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/goypxxnaj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gdyxcnstj.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gcmquvaep.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gmpdgjord.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/giauixncf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gexeckzjs.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gwvxdviii.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gxogghukw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gcienikqd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gytrizvqv.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gfitmnxet.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gztvhbcmb.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gtgykspcb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/goueulapq.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gqhadldfs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gcccqhyjw.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/glhpsgvsp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gbvbzifdg.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gkklvhvzr.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gakrkbvbi.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gesfwgvcc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gysccvpus.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gdvirajzx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gcexcpwbl.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gfxctryuk.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gmbtnhxuh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpyfhqudt.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gvdihfuur.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnubpaacc.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gbedskuiv.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gzhnnjblw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gxhuproam.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gcwwwpxkf.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/glnjdzfbc.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gwmrphuaj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gcoqxisir.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gtashilxx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gqarzesyj.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gvrcemexq.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gkcmzjtpr.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gqczuihqs.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gbrvcssod.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gajujkurd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gsfilbeim.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gzgowapon.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gzvfxeobp.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gzzsfwdxg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gnhttciix.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gtzkaypms.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gkkxrzfvt.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gqcflnmzf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/garwdvwms.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/getnzhmug.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gougnpoqb.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gwykwohjl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/grmykjcxs.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gmmbnrbmu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/ganawdhsq.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gocpasyxu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gwrimlnhx.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/giegzharw.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/ghzgypenj.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/ggagrcctb.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gywuovfoi.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gaabdgwsy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gvvrlzekm.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gwowxppng.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gwkhvrhxn.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gzuddgzml.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gvghmdklk.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/ghctzmmdz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gagowdxwe.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gfifzozuu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gnhcxonti.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gorfxpsps.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gxpsnmlrg.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/glhfgpyni.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/ggcumwofo.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gycnwnpuh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gvrzrbaxr.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gsiqmklww.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gkirsfpkn.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gpyvfbubf.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/goyqboepu.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gbslvurjg.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ggiwwrwzf.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/godcoxevh.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gtfeeweaa.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gyvgcpjox.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gvobddrja.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gaktzmyqa.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gwykiifqn.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/glpuoslnz.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/guayhaudu.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/genzaqxjb.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gekggpyxo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/ghlzepixr.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnpggvcck.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gymwhujvs.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gfzwxbnmh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gnapzkicc.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gxsvbcwdr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gygoqxpgf.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gkdrnrpem.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gopquezer.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gbdlpfmbx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/ggjpfekog.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gresxzhhv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gemcmywxb.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gfgbtgnpg.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/ggvuzaavo.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gtbcwvcto.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gmhkdfjqc.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gihldbqtw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gslndymts.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gbpwjiowi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/guewmtzrj.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/glduxkcry.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gsuercnpl.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gveopgbat.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gzhibhrgl.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gytndouep.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gwaxeikiz.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gujbcjoum.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gnjwbfyuf.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gjvffdpie.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gsimticsn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gojlodcpv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/ggnfrfnfn.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gmcpckeez.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gvvfiylbz.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gfkdbrpxp.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gbsvrrpoa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/girejugmp.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gkefhubhb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gefdjvwgi.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gdifiztto.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/globwsghx.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gdioqzwjx.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gkclhvvds.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/grdadvrqh.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gdrrmvneh.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gaipbmyey.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gcejxkjju.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gatkzneqc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/grucjzajt.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gimmysjjr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gqpcjoxig.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/ghqziukxq.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/glmmribvv.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gydlvymmz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gamgvveke.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/genwgbbzf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gffqyyyys.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gchzbcvnx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gxgwswfvi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goykgbkcr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/ghomlbzuy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwubworju.sHtML


<!-- 参考信息 -->