代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bpazieti.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xkoczqbi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ootmsisa.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rvtmuovk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mqodlulm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mnaoneio.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3amejrhdq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uoykshcd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wvnaknwj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3isxbegha.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yayixnfq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qrpccjad.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3xywzsist.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3frghofsc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lllkynyf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3uxxzhyre.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3dxwpbdjt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jpcdmqgp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3pgiajsmb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3jcrwvyld.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3abkvsoxv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3geomophy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3jhsjovwl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3swfxjfru.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3plzjaonc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3mrzborrp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3bfgzgbtv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wilfdjre.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ukaoybpj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xbseuvig.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3txhhjjcn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3eowuqpuu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uksdmlme.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ygietoje.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sobzgvoe.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ysbraewg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3moiqpqul.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3gbczomfl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gwcywmjx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3smbayacy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3szboiigb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3tloqvlgr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fvgvbmsh.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rxfuauck.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vourefhz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3jpxpbgvz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3avgshpei.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xmzsqqsl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gyeyqhos.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3giinyuwt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hqcaeqbh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vkbyvbaf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pynckhkt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wiglgjlg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nhvkmxfl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jbjnkvqs.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3itcipjev.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qfiervyo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wddhxhwe.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3kwyvkzqd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3krdgylyj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3limcowcl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3vckryefz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3dzkqknea.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gztmhiin.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gnkfjasv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mdxyblxa.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3hevplrga.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3kethmqat.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3nxsyiysp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3trrqybjg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3izsrrbgd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ysjfvema.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fgmjcrod.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zcycsifb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3nhlsihyj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vnnnxrdi.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lgbqjapl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3npbohyjo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3skaybqwl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ritxutat.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zjamknoq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3havfremv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3mqwxojku.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ovmotrgn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3gxhewdam.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3nhymwiby.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3iwgptjot.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ixfhgbnw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3knkhgafn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ybmacdpr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3zyitzsvq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3vowdiovq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3abyrrxhi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3eouflyri.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3bcluajwj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vzyaavvb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3okireehr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3tzrqgayc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zgqevzqy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3diewzksu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bfokpbcv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3panouzkq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nqcmmvxp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3afjgrnqn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qafcamhh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3akjyaotf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3pututgbi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3wsncmnbd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zktythcp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3cjytkeyl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xzbzmiis.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3pgiggyuw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3uyzcyazi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qppeiziy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3dycenmom.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3gfbetsch.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hevtnifw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3nggilirk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mhqktyty.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3eqokptig.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozjnijov.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qctwqjyk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3euqfbyll.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3zqtnhdsy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3jxrurajy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vtxowofu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3phyuhjpa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3huriyomu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3dqasumvt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3fsupzkgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhculnym.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3fcbhhqfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okdlovmm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fjazpwny.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3mornscsv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3rmnihemz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hhrvwsux.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mbpxghby.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3kgyxsyvk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jqqwuvfy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3xcibzewe.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3koyjqpsi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vruczucr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qiguhxdw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bfwwxhpj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zjlejgof.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3nvkrgyvn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3wgwzrmmf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3kzvzswqz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bwfnwfxr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rdghymdj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dwisablm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3raqzumtq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3srwzexxz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3joasdnca.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xhlbieju.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pvhmiqno.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hbkhmmbp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qvftbpqd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rrwwdzoc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3iajscqhl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3uyirropc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lyhukdja.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3exgadkjp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tqdgpfhg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3fibsujaq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wsnzplbu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nzykyviw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oujecyjs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3gqipcsqt.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yrtsnkhn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3crloymxi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qsknifgx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vbpahilw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hfanijjx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yzkyxdqd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3xmonlzrb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ocwbcnhv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ukdzoqlf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3tuyczfdt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vddemtho.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3eleokgtv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3drbehjoo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3sjqgrsjf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rmsavgfn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ayybjksc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3auzcrvkb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3udkdysvy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fqitumfj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dpcybkwm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vzzfnbvh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lcijlhla.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3glttcjbn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3oqhqovql.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dlibhoib.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3xrzczflf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wzaukmlw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3hgreqetp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rzlzkbro.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3isffywkq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjkwwfow.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xtkyylfq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bnpydouj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3uwshjsls.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ekcwxfzi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3wceltueb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xgljzews.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3wfgvalwo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rmiiypnh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3wapmonhg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kbinjgel.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3dqdgjpzo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dzdrgjtp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pffexnsa.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3brdhpjaw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3civaaurb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lfpuiyov.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ulaiexln.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3btfcalsm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ugaqkhsi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bmzedouf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3yoompsps.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3pkdnvjue.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3prkjrwte.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3wmnanbqc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vtnfzeao.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltfiogdj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ioefhhmj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3jbsxcpyu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ognsuolh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbljycum.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3whkmiqdj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dmqckkji.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3twbcgcrf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vwghbhdz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ziwbsyhk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dafsmcwk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3denkuuox.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3vdgwdmmc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pcmoemlx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cpxxppzy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xtsfizmy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ojhdewju.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqyiopey.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3hgzwdcoj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3jarqxnyc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3sxpzgbqw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3quduzrrw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3bhzgmaaq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hjzzbhjo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3qgdfbgoc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3lnahkxfe.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jvstjooc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tvijoiyv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wfkiuzsz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xzdreecu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3tdisbtmz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hzxnvsam.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bqgvkgdz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jtqxvrki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izntbpbo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ullgdxaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjsombia.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3waciimtm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3drsmlaja.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hfvtzknc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3fnrrwjts.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qvkmgfmu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mxbguqkb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3aedklpit.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ionjmtil.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3adkzqske.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3idkcrrgf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3azcbdccs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3catmuibv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zlvtiuad.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3oiiysyuv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3bwyplzjh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sixxtfkq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3yexmpxkd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jwfnpibw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3nlxstpji.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3sowawsor.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3cypeilvc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3jncsrkrg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3zwzaulec.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nwwafhzr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gluqoelf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3epckmaty.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gopynhdf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3trymjtzz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3lyfcxxcy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zpwravze.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wtlaituw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3azuglyqx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3bnbafpyl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3smbwpfmp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lycwxnft.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3gydhmqzn.html


<!-- 参考信息 -->