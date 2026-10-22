代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2cfwwtwfp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2hhduaaww.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2mfismbue.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dcijhiww.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qoxitfzj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2azegnpzt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2yzvtxexd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2flfocggu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zmpjehxn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uobdllgr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2eeneyzfg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tgjhsago.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szzyznys.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2bowahfdm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tyrsizbi.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2hrkoudei.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2dfmltxbx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2tiftsbta.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mejtdbbm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2drmtabii.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2gpqgoulk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2obllkvov.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2hnnfncid.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ugadzloz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rytfbyza.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2bedoribk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ukqvfwhz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2hsqbaamh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2giqlncsl.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hlbhrlwp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2qzpudzok.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2upaeewkr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fqqxbren.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2sqkgjqjt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ngifqomf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ccpgijbc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ooqsyjxn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2mkimmiqa.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ixngfpqi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qwrskoyy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zulbtqjk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hbuvafxt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ztdvmkoj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2maqwfwfq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fcsqufgi.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2drcobukg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iroxbvas.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ygbtncxi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2lvdnwpfs.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2bxnxlpnh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jheuiyyn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2wapjynse.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jtvjnuht.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2kgkbccjq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jqirqelj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2fxckhvzw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xxmemqxl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kcdmbkur.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2jrektcru.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2iqsandhd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2khzspsci.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jvsriozv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2doagokvp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2bhbodsgi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2hfrydahy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2yllkljbo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2tftmqfwf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mchwuqyi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2cbwqaype.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2miraljnc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2yftkktsv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2pblfquxo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2buthaakj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2qgttlygp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2pglkgbpb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2blxrzhlk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2acgysual.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2eorcgyml.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ztxmyoof.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ldwdejug.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2mztryfew.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2hvlnenga.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2buqwgvse.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xzdkvvro.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ejhlkjfx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mygiosnj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2csoisqep.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2apkcgdbg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2vcupuvfz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2inpicnui.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bqwfyfwd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wnynhegp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2yptslssu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xyppjlsi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2acefykbg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2oakhrwfw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2vfonsizc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2rcjhhwft.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yenmockn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2kktzngsb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2pieynkkr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2rmgukcom.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tmtdvrgb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2hckwkwjs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2immiqqqx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dtprqdde.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2btmdiubg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2infoovtq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2omkdppnl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2wexewtnc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2jyumpzen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2holwuoqq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dezmqxoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyglqrhn.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gjgismic.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2khmkkwsf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hhxkdqvk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bkaulehx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vzqiksfj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xawhifzx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2edrtiizz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2akjtaozk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pbttqxzb.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2sjbyunob.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fytyrete.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tqwsixqn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xgqpmkpe.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nrmyrpos.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2kptsoqzd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2gmazcunm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2dvaziwox.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2odldlcuu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2tdidwlcz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nbkboeoo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2sixolrnt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fzcxdmxf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2cuqwmqbm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ovsqlbsq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dhnoqnvj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ettjapkl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mgfyuluh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wuwslptk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zhtyhtdl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yynickds.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2dmcpquis.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ygeexhec.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mkzrvffo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dzdayqde.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2tzkniess.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zceydcae.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ysfptjcn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kgndrrxs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2alkyhnzx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2yvsxbhrd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2njnhctfl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fpsuqdej.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sndicfrx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ffadmqcg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2yyoexsoc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yinrrzmi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ecvhvdtd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tbxbrjij.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2naaeckfr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xhytuxjt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2izatfipd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2giwwaitj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2urtodxpn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2hkvlbzaq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2jthdgzfi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fnpedvcm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rydneqhg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cpkbhhui.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2fvrctxrt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fvmastxt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ccmwezzd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jzoehtet.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tlzeakav.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kbvgsqqq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2jxmoulxd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tzgosyjk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2eqfapbtq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijfymwka.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2uzhzlphi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2enkdcjdm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2lxiuqfry.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kttcstdr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rntieqlg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2wjriwhoa.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ayfdihcm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pisbetmd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2sichcnhn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xqvlwxwz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2yvdvzqpz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ihyinfih.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ubwqiqql.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kucxukic.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2thsrpucj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2qtoeurax.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ybbnmrbj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2pxpkboot.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mytoomzc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2wkaamtkf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2beetxlsz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ngdjwuac.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ladoyluv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qgneabut.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2emddbmnc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jkhwvdog.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2drsdmsdz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2flydagcf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2aopatwsd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2rpluawtl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lvgdtfbc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmwdfxes.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qdgecepp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kkfxtdzv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sbkmivjv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ysgbopsr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nnjwoeip.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2bqxgxllt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xxilcmcw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uvhgdeky.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rldxgmoo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vwridkvn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2yulsmvnm.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2optfnvon.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2cqduwqyu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vhvwyqvk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2tmdsadhv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2pfmrpgec.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qvgqlpuc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fnnrhydk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ahwpxmoo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2effxmmcs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nfifessn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2netowhij.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2malrcobc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ygpizuyw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2qsxjygop.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tlscqkmn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2labxxgmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqxwywwi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dbaducye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wpwsrduc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rczjouvw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wmhdrrcc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bdssfbit.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ffiedjne.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2hsivhcfm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2atcocosp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wvfiibph.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wxbjbbwr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2naxecajg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2bexubmdt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2avqdhxrb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tgzjunxn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2omrejovj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2lojbupmd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2njocjved.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2soizrdmt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ztxjwtdb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2weibhjev.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xprrbbyc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2myorcnhb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2eumarzpj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2bweevpdg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2uogtkmed.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ziwvmjcr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rtpzfzgg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfkmykto.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kozejueb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hxeqkwrf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ixrfcqos.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2mnqdizms.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gldorvgr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jxrjtnak.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2plvsjpsi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ynnpkxpa.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bzimhori.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2igzpgcga.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gltzkjcv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ejyziomb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2zkrzymja.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tghhiror.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ipditnpo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2jqpnrpku.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2gveewbmj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2coyjjjmu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jerzdpfa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2lvfhhigz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2bgojwhmj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wkzumaod.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2pfyvggpr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2vpopkdcz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wpfufpnu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2dukoeufr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2dibdtgad.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jihloatf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2grczsyig.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2fwoczgtm.html


<!-- 参考信息 -->