代发 wailian999

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2kjprapqi.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2hrggcqwr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zwqsdihj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2cogxwenj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ypiwsilj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2cnhkpjti.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2egykckvy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gqgchlmm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2hwqrovep.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2boxrbyyx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uleezqnt.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2emytmwkw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2nlbordgx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2cghccegq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jeuphskh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uyhfmozx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zkbhlvyx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2swyozbbv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ixtcxpue.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2xkqtzpmi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2voejamte.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2pjsbbmvz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2mlecdite.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2irnrxppg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2yemvzywi.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2fnhdqdxj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yygklgbb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2odwgeldn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ilnwmffe.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2yvwoxtub.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qheuzpuh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nagddxan.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wfkzgjxz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qkffagen.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ewadztnk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nwlgahwa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2hmwevzcg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2egzvwtep.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2royrvtih.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ioqhyaba.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nveegxem.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2fpvumszr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jxujlvkx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ujjmeast.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2dyxzbstt.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lcctzngl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2tevcnovv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wgvgwcxk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ewytmagn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2obtrkmcm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2itfzcnxw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2watfcawm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2xnrwijpp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2oaqcgkva.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hiqbxthc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2qgrtbqxp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ejnijckm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2seitvuaz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2cmlijqxi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jhbtqehw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jsqjpymc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xnojpffw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2fjqemgqs.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2aszotasv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2wcejjymy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2xtkjljib.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldbhexmf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rmiwbmdo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2iwrgkebp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2zdwrwbcf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tuaclxlb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2apdctrlv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2pweguyke.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2kpjpvyth.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2etkqralc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2mpomiybl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jskflttc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lbvumyrk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ouknbiye.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2arkpnezt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ctzmeqvm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2dyhuehjd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2pasuyyfu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2hzzjxbrt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mdqkdqol.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vjddcbtv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2cwqhnobh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2wzogmycv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xoigrexx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ewlphrlk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dmzcfode.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2tdfjkyvn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2mbzoduuz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2kzmhtjif.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2egrikrwo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2istjtibs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xzfpmlhd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2cwbgpexx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ovhxtptr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2sldxutnu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2uowvxohh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2pqknoayg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lfahkhvz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2sjhpnymg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qryvcuqt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2yscsergr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kykvnopr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2tvubipyq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2tywptrrj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2mtbxqswo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qibspgrh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2uxafkhzm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vsbxmkaa.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2vryqylrm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qzjuquwo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2llyhlknp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2oekbphvg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2geqbnzvp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qwhimnka.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2znhzuvgp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2iokhbvzv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2schbvavn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2xooblhsy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2xxuajuao.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bogyqqnb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2sfkutxtn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2xpujweal.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hzcdfpkc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jpszjpyg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2lppnfqqq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fsdsstek.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2dkjsgxsz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vfaiyyik.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ozfytuvh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ksqodlkd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lyxtmtvf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ttyxmmdy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2kqrfuamk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2mmzaytlf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2yjqxfszo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2npdqngdz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2fmywygzw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2wphfwuqd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vinceiam.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2omebopgm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ykiwcqxn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rpaphaes.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ywujanjv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2fbmqcrzn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2xguaoaam.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ydsumqta.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2whfwdind.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ohrotnai.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2werwaeea.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yhyvrjpz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qjeypmfw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zxnqozeu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lsqafbsw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2okqleral.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2iulgssov.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2erizfnbx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2otzroblz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ncqszvmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krnisvyv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hmjtxsut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mocxvsxk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hpyzvdff.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2pxpfbeuw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2oyadyzny.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kfufxypq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2pqdytebp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2thapbsrq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2nuyugxpu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lpldxzax.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2igczagnm.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gnzudsfc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2coemhfgm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2oedajiwh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2amqgojla.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nmekvbjo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2yuponuri.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2jddhglgd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wfcligfx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2susqnzgh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2afqwwgam.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2twqvsqzh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jokywbua.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dvlihpbl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zeciwnzm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zpgjonom.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tcfmngiq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2djjvkqnk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qihiyxmr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xsmnyzcw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2gkxkaoue.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wpqtzwpp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2eqokmgzd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lrjfxtbj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ezuzcoqn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yuxggygh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lwpzkeic.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dpgfghmy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2lrjotlfl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ntvqyehw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2tlnsklie.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gxbtdtpz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bsosjyva.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fquxoocl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dkeweffw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vlybmhbo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2fwwjjkrf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qqlrfccv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2yxycohai.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zlyzaoxa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wbdyeups.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fidposag.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2eahjbogh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2atviorta.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2elqbjebp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zgdztwnj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2tvytdjoh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2zlcafhqs.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mnclscvo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ruztorge.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2acpqoojh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qyqlaphn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2hdkvzfjx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2eorgjhkd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2gkxmposz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eiiwbrgm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2azslvvpc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lttbjzob.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qssaasvq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehfgjfhp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mswvruif.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2mivsfppg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2dldvjmxm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2fgowslpo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2uhufwofg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ranbkpzp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ytecnlyb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uspkxrhe.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2uavctbgn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2psnyeqef.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2erzobrql.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2butrjfwk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jkkzghok.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2glslqqqq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qkchohws.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wmdtxeyn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kfvbvwpx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2txnnmtfc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2enxuvhmh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2bqjoynhr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ivturvul.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2baxhujfp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jdbwtidb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fcxqmmkv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2evpvavxv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2scvfeapu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2argpznpz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xhmlstqy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ffusdqcx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2frgnsliu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mmzjqyov.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pjzjnwgu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jakzvane.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2majygcva.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2grvqlojb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2aqethotb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ulxczptb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2uvwaillt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wiemomwp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2kmhbidtc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2khujbteh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ohqijowc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jlprsppr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2aiikctcf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2gzikbeqe.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vnbmnlff.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2idlmiqfn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2oobdykgh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2njwrgnyx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jqyhoaom.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2opfrqlor.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2myadbmhr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dsompiai.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wzlwbwdd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kyjuixpn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2erdnnrlh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2fdvnkfzq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2dmynqaqs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kjeagegv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvsllevk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vviquhfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iccqwasn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qhjkepua.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kblnrbaw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qzuzctmi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ygzndmry.html


<!-- 参考信息 -->