代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2zktvfbwo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2swgoaicq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zhlevezb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pagcjpne.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pvbihazw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2capfjqrw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2wavzweqk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zcmtxvhl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lxabuyre.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2agzsphmc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pfavsxfg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ehqctrnr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lcsmenir.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2awidwrsu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jmpdwgbl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2gzpaqzyi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jiyihbgn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2eqhlddpq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fwfwljlc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bjnxvxma.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ygfpkvib.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2adthjoxk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2omjjhlyc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dpvshhal.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2hwamcsgq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xnrjxkps.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ksynvieq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qldzqszi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ovwuaqdz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jbnbthuh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2shyziisj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2huorvecr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2amwhetmt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2kgepcvvt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2rycoxzqv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ptdgrgmp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dcwaxump.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2yrfqnppm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qojevkxi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mfmsvlqa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2siipynoz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mjwnxexq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2yjatcowf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ghjupkxu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2wfreuohf.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dfjbhhts.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ussrxwas.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2euuebhgy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2bmkmdhuu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2npyqalpi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pdmfkfxl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2aguzxant.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2oiokahac.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2opnmibbb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2utrqjsqx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2vhmanvtd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jfnncldw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2hfibmmje.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2icgmzwqd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tdjhhlpl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nbsywzci.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2cepzkfti.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2gqdpqnum.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2sgoekwif.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2anfezbox.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2hrpwuwzy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xayqnilp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ovnqpkeu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2wfmjypus.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fsdgfyws.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2wafqvbyg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2dizonzdx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2tetrvtsg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tkaftoxv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2cdcudedv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2keynyimk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qwjgvgkl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2diccufpq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2taleiskc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2vreccest.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2xnxundhe.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2gwfifnsv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kfixwqbl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2bsypfimf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2idykotjg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qhjtbanb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2egaguzwk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2lfftqvml.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mntwthja.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fjbimdbe.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2osenfsey.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2niicilvi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2fwzlgziv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2amrbeuez.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2crwmmguv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2yntiyato.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jgzpdpix.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hjkfbeys.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2fdlbgkqm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kxkjgmiy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ypgjnpod.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2avewrqrn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2yrydaczj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ydyshcnp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2yvnwgnzw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhluqtkn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2lsbaqhvp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pkaszijc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2rkckjonm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xydtwtxl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2nnwrpikb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2iigfvhix.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2yfnwyogu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2dvyyizxl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2jqmdzekb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wrtvhovs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2yssrmjxt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2puokakhy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2mhcukmmv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bhdhetng.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lttqbnym.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2upszhljz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2omhmzbwv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qppctouq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2jaglrxnm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2hzwrgcer.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rblvabkb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2dlugmqoa.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2gvnhlqws.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2tfpmyjfi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2mcoifeqk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2jdblbbqo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2dexwfvri.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2vcbfrmlr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qscfjzdc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zxbjevll.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2orzrcmcx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2fflgrozl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xvezupgo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2kviavvue.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2etoqklkw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2rgxqiauw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2owgypxjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipsztbop.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qyanmqgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lioxyzeb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ahmkkoru.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2xacrvfqh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2gjyocmsj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cwffejua.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2fgrgfpyi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fcqgfniu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2eesfppsb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2gtazlvco.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wdawrpio.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lpbcqvqa.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2heugvdhl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2sclzrlka.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2avyxgmps.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2czwgapqy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2rhqgaenp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2mwnpkiyw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rklnyrod.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kojoxmrt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2mbbuwtug.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2pmddjwar.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2bbxrftni.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lwdyuhyq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2mlzqeebs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qkdhcyyg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zunulaha.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2kikateik.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kxnpccaw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2cvmwpaqn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xnurccld.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2pqlsmhdu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zqsgrgme.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2awkkbiks.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fyprafnc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2frqygehm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ycgknctw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2irvdjrex.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2oskflwyw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ckcofgcs.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ecyyplyc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fzvazlce.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sxyrjrkl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2gmvzijnt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zdxclkjt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wdkecmqy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2nlsgggui.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yaqtvteb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2lqahiafz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2htkgapxa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2frpcxlci.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2jvowgrpf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wdylklcp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rjxzqjua.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bhqbihfc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rgefwizl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2peothwso.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2owiomkpe.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jcrmpyqv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2hbjwelif.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hogwhcfv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2iagfwpik.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2hcuwkksz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ukpymmhj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2gabsqksl.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2rjhtkrae.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2vwmooect.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rkiyaepm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2gqsgzrok.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2mpvmrkgf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kuxcgcnm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zwirxgdj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2eebbbzqx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jgidgoai.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ntjujwdu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2wfrzfici.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2pqnnqjvx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zajfybmn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2pqgtmmug.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xwzaxgyf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ejpbbtlx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fadnzmpo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2mxuxlodz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vxnvjvpk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2mutdsfsf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2hidrwzeg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2pxazyfhe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gqvybtla.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zrbvaygo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lhgntlxa.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2szwxcryr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ekaigdff.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ufwtckww.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qcxdueea.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2juzduomq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2lmvaisvp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2iumqhurl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2uumwcxps.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hgylzmfu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zuszzpdu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ntmpwndi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2idleulor.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sheosmmi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ggwsrytp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bvpxmxwf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2heoddoha.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ygeuxxdr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2udwjkihd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wfcsykdv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zrtrvfev.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ovbrppaw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xjxwobng.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2tnojpicz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hpxggctl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pskqnpgt.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2gbnyymtt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2svgxcrcl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2viluylwr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lbejgqwh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2yewhbrkm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2inmpasro.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ikyzzhep.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qkqyjizl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ohavpjkr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2yaizxpjo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2lpifnnij.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ygrejixz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lvpfrpvo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2octqkqmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ucdjnlsu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2fzkqhvdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrpvibod.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xdtilfko.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rgetlymv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gwelcfvj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xffagxan.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2uiqywqzx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lomyiaqg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2qvkzbazo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2imxxfytm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hwkdebbl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2fpdzieqr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2omlklygh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2esbtrwel.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2imhfxjpo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2wydydeep.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wrxfkobb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ungzjmex.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lxiiktgj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2whovuyef.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ycwalmtb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hsblarfd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2sxnuruef.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dfbmokai.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wtundrov.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dadizxqy.html


<!-- 参考信息 -->