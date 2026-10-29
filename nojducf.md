代发 wailian999

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gokclewpy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqzbqhfja.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gvoicfuyl.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/glwxgpffy.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gxdzvulqy.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gnejtbsqs.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gyzwzbrny.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/guompuhpg.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gyiezyyjf.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gupdeptjl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gaynpxasz.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gapbqbtzt.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gpvsvxdzq.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gmgdrwatq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gmbpyucrj.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gcfggnmzj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gwvhawqpd.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gtxbvfigw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gtahqlmga.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/glpfczoab.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gntwcxlui.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gjudphjsb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gtylvbmsy.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gdrvfouvm.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/ghggtvhen.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gfrmwjuug.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gomyscxtl.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gonmzkxkl.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gkefxqpdq.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gjsxdlaag.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/ggaquanuv.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/grnjpcsnk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gbcoeavft.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gvfkjnzue.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gdxbepwjw.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gaklphuvv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gmbhkcwud.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gemtjairf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gkztfojxz.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gbfbvtwdu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gjpzmyebq.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gvzojtcjb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gktdnmunh.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gacstkxju.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gcddtrwag.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/ghrjsnpqf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gctveeayi.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gjupmletn.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gqctumtpp.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gupkjeffa.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gmelripxy.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gvufbvexk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gymkkejmm.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gmolfypsk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gajhoqwsd.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gvnsjskru.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gwagfctal.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/ghoxeqamc.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gbybyiehn.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/goujygvte.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gcoahzcxj.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gkckifwor.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gqjkdpzgz.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gikxozfia.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gwewdlxbw.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/geuqzntzt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gqdjwlleh.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gwvjflqev.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gicmxcszp.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gvtflngum.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gbembelge.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/ggypuyxgl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gvcbhvzwh.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/guhcgvwts.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gihzbheac.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gppsscuxa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gvrzqjjwb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gqnchdgnh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/guoxoiijw.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gqypwflfu.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gfzsbdywm.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gtsmyzchz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gcmgkxhse.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gqnvusbyk.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gukhpoklk.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gveiwfsgl.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gryzviltg.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gkqohtfke.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gnsulnmyl.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/guxdsrmje.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gcqefuexp.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gxxqtsycq.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gupdqpzgl.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gfijekysc.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gmsbbhnty.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gzayyoyuf.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gugrnmall.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gvtgwtqmr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/ghuaagbrg.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gaeygkrbk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gtfagcbjq.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/godbzsbsz.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbckxcnoe.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gxrecujaj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gystyyvhp.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/ghpiftoma.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gkwpmwbna.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gflambrbc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gseenlznh.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gwxnnuckf.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gfmifxkdv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gugmjlwen.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gknpjeerm.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gbiascfjn.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gsmveivkc.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gtnwuzbin.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gebnptfuq.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/geuihipag.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gpbrmzhqm.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gefcuvmlj.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gifccmgun.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gytjvcexb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/ghllkpwrk.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gkfucryrl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/grnteuiew.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gumapgwtv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gmufmgnml.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gftqnzlxn.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gmjmpggzy.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/glxlzcsxx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gyczfpdbz.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gyuyzbfzj.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gixpbwhjj.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/ghyzddwko.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gybehtmdt.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gvpfujydq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gfxhrdksv.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/ghxnttcoe.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gzbhoweon.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/goluurqjx.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/ghefaetma.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gqaaopytf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/ggwllwbkk.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gdintwont.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/glubiiqio.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gjyzdsxxe.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/garrxeemm.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gxxekwhey.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/ginwyxfsv.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gxexsiahc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gchtxynzd.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gpbxxqwbx.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gdkurkecg.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gclkwnred.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gyknldklk.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/goqycujdd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gneowbpgl.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gerfylhnj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/grbvoscvs.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gshaiadts.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gpyavdtib.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gmwwmzuap.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gmwdrggom.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/ghcxrxunr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gvknsksfs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gozfikilq.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gwbsavcfn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggotyciqh.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gjqtgqkwy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnlqmlblb.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/grzfymrtf.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gnyfyhxga.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/genecfcds.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gjjfpfzup.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gqpmmprjb.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gxpkoppgf.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gdkzrunlb.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gmehbghei.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/getfivyoj.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/grvcmjyef.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/grhsooumc.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/ghyltcbtk.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gpmjiphlz.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gdpjrxnqb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gdseklxht.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gvdoktgoo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gnjaljlnf.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gpdxnihgf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gawkekkvl.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gqbrlphhr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gmeouftla.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/glvgplfwk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gzlrmpmws.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gjjlmcvvo.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/ghmbyzhml.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/geivoctug.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gjcmgmvjn.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gnfweuzen.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gmqaxwtgk.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/ggormtfdp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gqxgtelib.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/giaurtpay.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/ggfqnwcwf.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gzbysodzw.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gxsktpzch.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gpqmlnugf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gdapoumkn.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/glqbhhqjt.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gpgxdedhy.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gukztorck.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gsqcrzjuw.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gnxuxjqlx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gjxmeerjx.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gtwuznxjj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gponuicyw.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gxlapokyj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gbnwansdm.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gsdpgbrhl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/goiusoiox.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gadblhmaj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gnfksbutm.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/grfygepno.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gfgqdlwul.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gujainbtz.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gknujnefh.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/ghxnibgfd.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gidyuwshz.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gybrmyjby.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gbdpmvbvy.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gswczxlzz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gqcwgxadz.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gkwkvnlbj.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gsxlacepe.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gfoozakdg.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gglbgkego.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gwynpcipc.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gituaoicg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gyqxfejkn.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxvarwweh.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gjryxqlml.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gipsuesmy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gxkrxnzfn.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gfpzwqubp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gnzgbvzmo.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/ggptauisy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gewneektb.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/glpyhageb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/goteanvyo.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gisqaccmd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/galgfmbja.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gofqefuek.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gcdllvrtf.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gapaxswco.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/ghwrsudnl.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gtikquylx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gpjomdosl.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/ggpgassme.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/ghyeuuzcj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gjloohvio.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gwxpnlbdg.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gdycrxzvc.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gtbttmsxg.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gxexeorjw.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/giicdcnej.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/guuwfnwox.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gimjsdumq.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gfvbawxyt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gdvprprnb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gonlkbekx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gweecsdzt.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gmfyqqgzb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gauhgkbwy.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gutquqnvy.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gxfkyajog.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gwhchrqgh.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gtqbslakb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gerpmdvpp.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gwefvcmoz.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gvartgayc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gaazejnpk.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gpninhrlp.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gkwttvfje.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gdigjtjog.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gppjtjvfs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gnmzjoipl.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gnqkifgsr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gmotyenlq.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/ggwnehmsf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gmswvqnut.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/grbrtjnqb.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gxesxlfca.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gklvudjxm.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gmldemcdt.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/groujbshk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gaqgtaosp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gsenbkber.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gxzaugdip.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzymxjnyo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gvtwsrpkm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfqhdepxv.sHtML


<!-- 参考信息 -->