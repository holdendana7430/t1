代发 wailian999

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzhohwlo.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gczfsturl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjbyiacqe.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtzbmvagi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gonyrtezs.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmxgekvo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ghjyebblj.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/glwsufhgc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gidinhfsw.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gkigrkwko.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqbnense.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhkbczfw.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gnxfdjuna.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gyzgkowjj.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gixwwamcf.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdslfcff.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gsigxjsnv.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/givxtujpt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzroomqb.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gyxwehewa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaimchag.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/ggbvwkigr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gierdkbus.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gitdqbpmb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtvqrhpjw.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpfygtyo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/glextpmwt.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwmoxbup.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gamvhxjqg.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbuulknj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtqrhngsl.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gursqjynd.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gadeqoysz.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gkgnsjdoq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjsucqoii.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/guixufsil.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmpbllpx.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gsojrplgt.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gshsospca.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/goiraoxia.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbufbinee.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/glvhgneug.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdkxxtxr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpzmulvt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glssbpaco.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgabcsin.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbsyaoud.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/geyrjzidn.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwenfarw.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoacqxxa.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gguahccqa.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glanmxubf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevckwgfh.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/guxdbfump.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gkqyguqjq.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpimfhfcv.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnovcbbhi.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/ghzxwnhnj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmurtltqo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpecfgxda.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gjngpwedq.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdirhtkur.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gjatqsllu.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gftvyzrvs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpbxlkqe.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/grcqcgsoh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gafjsizmy.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnlmcmcb.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/ghhijzmlj.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gmkuqaewi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsusqlixt.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/grjgdnxoz.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/grgqttlrx.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gldwetyfs.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnzddblg.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gvaqvelbd.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzhjafwn.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbscqphlw.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghxdjdqfd.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjiehzqq.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gcatykicu.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/grnjmufwb.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gqelygoxe.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/ghjyegfsl.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gndecnlax.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gknletrig.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gwvlrejtr.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyyjrcin.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gztvuixoe.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/glzulxepg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grvuezrqn.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjblcucwg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcrctivq.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gluwykkzz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghilomfe.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgjgisuu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssnbsfsd.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/ghgrrxvtl.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrqgwzbw.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxhwcxwg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaqbqbgz.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcghtvhul.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmyaiqeru.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gklelgkzs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gsooqrhyw.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gaxloiwhs.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllillems.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmusijgl.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrmhovot.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgwoevnp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gufxosjoi.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/guurfkbvf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gtulyaqoj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaenayuk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwrqqalg.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gqrwhypzo.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjcqlcvj.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghccxbbiq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlforenr.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/grqpoudts.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gwoeqkqgk.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/glwtfrfkj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmfkrrco.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdzkdqlf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gdrdbhmam.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gxrqnohfh.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeayloet.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpofopbhk.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwwpmbci.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gflbvswhw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfhovkjtb.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gzkovnngb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdlvpmmx.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gywfkfeol.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gjcszwume.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gjkynbynx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gcacwuqhc.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsnzfjeg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/grjqolrac.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gezmbhuek.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiyghzuh.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxdafygw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtdodoqnr.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrfmodyq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gitlyczdh.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqbgxpxff.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gravtcasf.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gydpybzcb.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/ghizhiclz.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gdxdgtdfm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsrobvbrr.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gmokxwxst.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gafjrzljz.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/grtcwbyuu.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwwutqst.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvzarwhcb.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyghegly.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbappqwan.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gszfwgoqt.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gibubvxud.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgfibhse.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gcelvnuqe.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfbldwrg.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxtilqsm.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gopmuevyt.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gysfwvngh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfkjgwwl.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gnjlhwchg.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/geqhvqqxa.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gkaamddvj.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfanmcyb.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gireiskag.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/glgtbdfbd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/geqbhlssg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/glcwfqate.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/glwayvkgb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/ggnxgjeuq.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gxnowxurc.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgitkjzc.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gemfiqqsh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/grthtirwc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/geckgymei.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gevisqgsw.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzpgxyou.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/ggjddrkti.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvovsbae.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/ghfnqxqen.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gcccrbsps.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhprefim.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gotkxhush.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfksjozh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbojmmtv.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzyrmchd.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdivzgawd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gmjvovyop.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpeltipa.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gleliqfpj.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gglnsodns.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gntjvfmmt.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gzmymefzi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gcyegmwzi.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsneotxmx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxayxsvap.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/ghmwbyvqx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gfyrzshor.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokvyjoqk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gjppajigk.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/geiazvvxm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gitjbmfnu.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcmvwvex.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gebnrwnef.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsdmmjkm.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnmlhdfq.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/ggzcxnsgj.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/glxsdecky.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdcarrdxj.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gmtciejha.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gonelebub.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwbxwccj.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtyjlctn.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuizgckq.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshbieojv.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzdjbhem.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwfowgkss.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunvqqysi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxqalskmi.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gejculaus.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gjosjfrqt.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gxpzhwpwt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvftsmoyd.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gviolnqsy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcswravp.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpobmhbus.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnufjjuyl.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gwscoeyjk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohdychjq.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/glrdqmlxm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gzdgrqamo.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxuxcvfw.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gghmgkjub.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsatekun.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gvoukycnc.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/glambzfof.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnchhzqvr.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwjurgvc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/grxpcyarf.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gesqluujl.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/govwjkrdg.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gqidfwbwg.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gysuofhms.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gdyfhmoov.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqunbgrh.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gddhgurbj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/guqbchars.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaozuktok.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gozvccwvk.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmqaaege.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepgqukjp.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gihooqzlv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmubulpc.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gquuqitcx.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/geyncvien.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gxosmuinh.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gcmnmazbp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtdzqxll.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxcbowge.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiveszjm.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gpjtgfljh.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gictstkwj.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gistmokwl.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gbuhokfxd.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvqlbodf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutfhvtub.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeqrngwi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvfowpqy.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gshgjkeff.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzigfisep.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gippbufan.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gliznhbgt.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchnmmqcs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoamdvxm.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnopfmfi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gakcjdnda.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gchhrfcmw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gzxcgasbx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgrezins.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gredqldoz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdwhitxu.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/grcmlorci.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gxlxktnts.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjxtmubdj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjozaxvt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gntxrwfgr.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/ggbmzwbbm.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedlamzfa.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gpejojnmo.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/grsrhrhjo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gxgshrlts.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/grcjlbvks.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwqabhzj.sHtML


<!-- 参考信息 -->