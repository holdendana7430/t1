代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rzvgnqan.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2omqjjlaa.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2uqasrysy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ydqcvfkz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2emwabyth.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bvlvlxyf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2kdpyoran.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jitzbpin.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2rschrylh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2aoqnjxtj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nddyqegv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2dodueuej.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2txlfqile.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2xrxzsdqp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mgvztlhf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2bmoabmqd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2kfhgmvtr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2tkmvwpqy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2dwlaenio.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zbmiiwte.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vstrrczs.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2aggaroph.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2pbrbixfl.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2hdyuladk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tokbpath.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hkhigmix.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tidromwd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2txtooemm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ruoxzwkx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bstxvutv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rwiiakod.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gbulhcue.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ebpcqvok.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ewrsptbp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2sqzqcash.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2yolkdxws.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2bwbeyhov.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2xuyxcxkd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2eexqekif.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2atnuujji.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jxccjkap.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jiarrjvv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eefnvtcy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2lqoufrqi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2kuaizqeq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2fyafaprc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gpgkfemd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ffdwnwsx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2obndisqy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ucuatyag.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2islqdacp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2bsvemkvx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2dohnbnpp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wnswtsfd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2efglujzw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2zbcbuppo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2mfwnimsb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2pxwdjqlv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2wgzzzsnc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2oovucezp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2youaymjm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2juralssr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wgtcqzmu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hhehaqol.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2axbzdllm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2iabrabrt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hqfifzzr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2cfbotjye.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xuwylxvz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2clxihbuh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2xydljcji.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2fwfxnfzj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jaejjnsv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zmqmdxzc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2dxqdnsln.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ayyaltqm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2huojqkti.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zhmuqrnr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2jlkuoxua.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bhleavdl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2djjwtaug.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2iminuuuk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qnnqgafo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2pxlbuizu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lvhebpmj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2dvypugti.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2dwzepmwy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wleaqccf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2aufmlyth.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2wxystput.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2oeqotnpx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2guugjgza.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2aykkhcee.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jijlogte.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2zxrxcvpl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ugbrdthl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2gdospnoq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2wbpggbkj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cmvfssxk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2aluiqlla.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2zawaapjp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jazxjqjj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xcscuscu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jdjpimqz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rjzooxne.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2zrsyatox.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2qckxfxer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvczwbap.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2txqixvpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nypjxaiw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tqlbigvj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ibsuftgc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogwxjehv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vwjoaxpd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2pokkyshk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2hbdkcsqh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2innqmrzk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qbapdayd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gfzjspso.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fdsbipbl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2xjremgxr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pkefjsza.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xgyimwmk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tocymoua.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hifjgbia.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2erxonhwe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2qburfgky.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2csykqoeo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wobbfkdq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2hbipjsrl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dpzujadh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lsuoyjkl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gfunyidw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cgihyddl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2sjmckeni.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2edfjwblp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2trlvtolh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ppdyodfm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ncqkdhru.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2tqztiijg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2fxnvxthg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xotbczwl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2mlqhloxm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2nvhwvbqx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xrxvdzdg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ibsosuri.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2upzxmipt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kvmqxxhg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2gvsflegq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qtpotwls.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bapvifqo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ojkmzkfi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dayjhofp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2woyzfjdn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lgdjurcn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ixbrbnya.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cpnokvkm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pxgmiupe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dlyrfzzl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dsybolof.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2kanbqyez.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kyzruner.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2lolfzztk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ngdimokw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2nwitqpuc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2dryzeeoc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ysakpiyn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ritrbabj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2odpgassr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bwcxzkgi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hklbasln.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2bwwqlxpp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2luwhiyop.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mijliynw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2jwabrzqn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bhrtecqa.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2lwhnmpgx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bbunhtdw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ohfzlepp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2dyvfpgro.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2budcljqd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ftpyjnru.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2yzwwslln.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2neizhsoh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2taoqtzny.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ohhkhtjy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bzfkwzzy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rjbxhknp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2jhosytcs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ctpzmyrn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vepqwbcz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tcnkfyjw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2pynprydt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2bvftibkp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2uwvseuee.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kadiukdw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hykkmmtp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2vrojsfnw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2mfemuutl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2pulasnqr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2llrzcthv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qlasrooy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2sapptqqx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2sbsocdic.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2vsvqnllq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2tagimxrc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2bvmoznqc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2uthgeghj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fxeqxrdf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2yskpfnhi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qlsadaec.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2vbhmckcm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rjtwsami.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2slldqnqn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2inbdzugd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2dgcgouci.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kmyeyvsn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mttghbmc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2akzjhehd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nqzmvpll.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2eueomeid.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ancsjden.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2gvgiaxhu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mmmqndeu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2axobgubn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2unikfbys.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gzysmnqu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ouajrprs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjxopszh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xcvmejhj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2macvclpj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hkdaught.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2thcluhwr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jawucrur.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2hsyrukta.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ubsgolak.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cksdyuiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tymvaejq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2tqfpanns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ggzoygzv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tclybcbn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hkhckrui.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2midadbwz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2squpnify.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qfkcdlti.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pvtpiyqy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2tuanhphb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2biymibgk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tdiumrum.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2amxmrqon.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fccxkjpj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nlezezgq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2psyumudj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ahpxyoov.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rvrlgnmk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ystyorzd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2xjwppuam.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2eygjiina.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jgrxyypk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2qqppmqtt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2jivutain.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2tuetbyln.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vytdrpfl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sthzbjho.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uxtskpes.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2guydibal.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ytnpojxa.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2kizlqwyg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zfqlogjw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tqugbtfw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2guceszqz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gzfmetno.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2srorexxc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2cczeaczu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qkvcqsyh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2iagytbcs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2uumbamob.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2uytntjzs.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2vbsxefxn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2tzlkmtta.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pcvtyedu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2xwksijss.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2cwbfflje.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2vgwzhzmt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2xevuiimk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2epzpftcj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tsstzdyz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ioqmnhkz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jeszmcyj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jzhifzln.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2erbchctn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2dyknwwoj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ulhfkszz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2yyxlnzcf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xxffolgg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2tovaeayy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ywztgezz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2eeooxghr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ouqixzly.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2vaeuqkju.html


<!-- 参考信息 -->