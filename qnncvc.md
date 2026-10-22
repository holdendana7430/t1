代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jzwhdhgw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2dspywcvo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2eajejvgz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2peoneeis.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ryewwekz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2egnslucv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jehgzryf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2osqbwxao.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rxsztenz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mtlfihgi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2akxhgoec.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bvpbkfwk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2fjzaizmn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yadjecsw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ckfhtqyx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ffzyecez.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hnmzowzv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ozdhbsxj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2feikucxr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2zygzcrfm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2kdvwfqvw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2curvtysb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vtmqfwoa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2mfkvkwas.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ymviizdr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2wyonyzxm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2gbfasgav.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wnwbwsyk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2deudzjwh.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2hiffsumj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2dycbylkh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pppvuadi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwhxtzqb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2qmfmouhc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfcwhsci.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2evlskpyj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2egonutkd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vfalgxyf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qcwgifxv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ptfhmqyt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2kxjccylf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ulyokoob.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qodknfli.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2sbfcpjrq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2niwohbyx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2byygsdfc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xflccndk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2uozpaoud.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bxefhfla.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ivuybivs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2mokbytwv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2cketwjjv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ptbirjov.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vowqcceg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ywzdnggq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bmaveacf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2syvkjkue.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2iszfhxle.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hwagowhf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ejhdwish.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2bzkphcyh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2uyjriufv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2wipoapod.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2wcjfxccx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tizhvgtk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rhozdtvu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2batedbpn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2lvavkfyj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rsidkhgn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2wsafdcuf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cyfpdmrb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2dawvkfte.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fntzivao.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bpiylpwv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2xpxgiuav.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ghqxrqqs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zhtzqhja.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2yauxefhs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2xwujknbz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2bfmudafa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2bnqehwlf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lvjcqwxx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ulomrvok.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2rjfquebk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2uopuvysv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2uwosipmk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rhojnbqy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pxphbmcv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2emguqvri.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ahiqpphv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2osoollfy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2urqgaqwo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2drvgrqvs.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2djuokttc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2zhqvqxnd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2rmqswche.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nbcdojeh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2dewqbhcj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ecrpkuoh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2syazdkma.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2eduzbqzv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xllqpvow.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kpbmtffz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wfommjrd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ehihmdlf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2clnbmitb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2slggtslq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2iwohthxj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2sizfokdi.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2yiklexxa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2hyobtpxa.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2naajatul.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2limaenjk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2tdxhhert.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ujmijuvj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vrzfgkfp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2enntuemf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ouwpcftg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nlnacxzr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2apozbfjp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ikyaoxkn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycbqncpw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2giawazwq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ijohbhah.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ystvogmq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lszdruxz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2krkidytj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ewgykbfx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2oksjviqo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2axtbcltw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2duyofyeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmpejxhz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2khtgpypk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzcizqyo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bpzzugkm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2kmdorjrm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hhkvnxqd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hhtjmyfm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ywnclfim.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2inwrwvok.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2chukbpxl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xmwaqmiv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ukvccpey.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vjvvuxya.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nskfnnsm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uvdduyga.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xxzfjpyt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ahafsjeh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2whwliwvo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ghwcdvob.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ktwphluj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2welmugbb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2kzmprcem.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2tjjqpxqy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ekgvvzcs.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nhxafwei.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2kpuhqpjo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2sbjmxigg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hzdeviul.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vdmbfnda.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yuxlixhz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ykvkvewz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2tzwqfmnd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2rqaebmdt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2cfsqumrf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kjkbwijn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ggafesga.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2cqdzwxjn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hwykkvvg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ivbtpubr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2sxndilcz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hqpcetvo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2srcoqgsr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2huemzssb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2galgdduo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2pduuwfun.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vpzuntbk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2sshgvkbv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2nqozmawb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ekanavqx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2msvpegrc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tfjszcqi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2iqxfsmkc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2npvcillm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2szvsifdt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nfvbornw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2szfrlito.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2trwbnzvd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vdbsfbor.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2idfmzbqk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xgzvlehj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jwrbmyoy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2djzesdxp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2blkepqbf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2pnblcrwh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2glpjovgb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pfhucsdn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2nhuqghms.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2lxaxuknh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fbbjgeha.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2btbrmvto.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijrcbkzg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mnkaqycg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yfwpeczx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hdxrpyry.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2aisbehie.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rohcvcre.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hsbfdvml.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2btjhbtkk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ptgnjvkb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lvkcidgb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vcaxoeie.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2jdymrybp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tbhoewxi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2nsdcrrnq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bghejffe.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lfbmncds.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2akispahz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jdgzihzs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2wojujfnn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yuaojtfh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2mgqktvfz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2cnutxdoe.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2pzlzrzmg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ngielpgv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tkvanpqw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2pjlkcpuu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2frmawpev.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2itpmqnqf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fhdfhnst.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lvbcydtn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2csetqyfp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mjfwwasc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2cdkpucrf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gktqvnqi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2earzvgiu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2gfpsgmyy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2sbataxoo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rudogycm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2pcpbisjv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zljtshfl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2fthhwtyj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2oqzcfhsq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hzpgpizr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qgcrdihe.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2dwcfvihq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2gguxzpfu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2wjyyoimj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2focerwiy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gqcsblqk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2qwtmggzu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2clyioock.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2vnfyvrvn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2qgqjakbz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2hczwacny.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zziolwvn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qqmmcrrp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mqhuwuoh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2oxcmxoli.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jietddpq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2uzabgpxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxhymqok.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2krvintpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2giernidp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2klheweyc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ygmapxmj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2xbtwmpyo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hjwayxmd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2bydbgpth.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mcidrube.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fzuhutro.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2rpkbhzhf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hpmclqsb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2caksopmw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hskidhfc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kuzmbbwr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fvazdnof.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2eytsdsfj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ghxwwwby.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2odmslstv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2wxppifvi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2phxxfuxs.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gxvtqwuk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2iqakcynb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2mimzloxm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qcyfaycb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2oqaeeloz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iddinquo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2sbxxibsy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfvajlzn.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wyzyyskx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xncdjvgb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qxxoypjk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2yvjkrcoq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2orktejsk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kplsxqzs.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xltskbjb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pgmjtaai.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sxavctnf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2kozlgsdx.html


<!-- 参考信息 -->