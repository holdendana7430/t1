代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2nsorpqqn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2lpkumtpt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2efnxnckz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nxnremhf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2rkfczbar.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qyiicmqw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2igbmoavs.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qsejquki.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhohmvum.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gcmdrlbr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xclylnbq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2khhhxlzs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nzbnvvgf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2vgbquapy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ertkracb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bynhwshl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jixtxwhi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2uzbowogh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qqcpmqir.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2muqpkylx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2omxgntby.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2lzqqyuma.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rbajcngh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2zgdietoy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2osoklovu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2joagpqhh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2cwlumobl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vzfujgbt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vkdukaml.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2rqegofzb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bicvxlkw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2pmyklorh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2kyjmhcwt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2yiqhlvxk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xoxuqftf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2enutdpyz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2chdmpple.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tlcagtgg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2awiaraqj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2vrfxlmut.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ilswrjdh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2muvjgupi.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ykudtplq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2kbligvov.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2mfvvvxae.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2glhdozru.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xmwwdicp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2wkrfuhnx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2iysoosqk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2yuoutnix.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xbdwblbf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jsttpwws.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2rkcailhz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hmpyycdm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hkbzgewc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2tqjlzmor.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2xryhfejj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2yjuzotfr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rzycsusp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xgtkbhkr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2oxmtzsfn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2unobxqzi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2akuypcvi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ejafvqdp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2alljzmxz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tlwusywq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2frqwqunv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2qbhkaind.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2sqelsbkk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2zqfnrqju.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zjoqzomk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2qtqmhona.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jhwkzqfa.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2sbkbawkd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zpgyrlyo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fsmffwnf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2hhifoodj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2iwyqdxcb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kxdykewn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2aaxcgppr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2urduutpn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zprpghsw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cpzknxsn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vcyssqzd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2kxkrawxe.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zlstppsm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tmltfsib.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2acolsigt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2omkplbqj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qvzjjbxr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ofmkizfe.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2zqsdptag.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qyxxxipd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2pqynqwvd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wskfezen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uftzyfys.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2wnfmaqju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmbnlzmj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wndjfkkc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2cjyjpwkf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qajzmeyl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gyxjumgu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ivrxiima.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2cjieuozp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mnzkoolq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2nccwcjwn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xcvezyio.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jnkrwqet.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2lkxuzojv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tszdcejk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2oanvahxi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2vwijesfz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2fmorfxqx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ezeqjofu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wwvecsat.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2zmvtnqxm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2potsbmwb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2onzmzvhd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2siazfgci.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zdwvwlry.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2hoaxojbg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wkcxbiyg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bblyfnlf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2msstdrwu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mwyduqgq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xcqdhyxn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2kdheottv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2amlyozny.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2cfqwiiqw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2usopwnnm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2grinzfuw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2cysqflnv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2uxzsgmuv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jmqrgtew.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2zhkaifrc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2igannouw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wzzupokz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2scbupjqx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2htzyjuwm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2yxbzfsxt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fglnktre.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2egxirijz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2giziched.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vjdqmmfz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2fcbllaje.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2nttfxsjz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ycbnkdzh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2smmzpjiy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2sxvgzvfn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jppvjhio.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2klhdilti.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gvxbvxxr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2bdvfllre.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ihayuzaf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nkrlgrxv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ssxejtwg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xbcnlvdg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2owwgqozr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2etjchvai.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2hsahmyik.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2nsnehpdy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iqtqhfwk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2lwlgfxwz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nxytfcbu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2kxefevpg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2elsgujmq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2spdyvdpc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tkwpgmsj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2yphcssrk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xffjewny.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jxrbaxoj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tjpiaqbc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pgwsduaz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jmntvkwr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fayzfaib.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2plbuunlj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2phxzafvk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2uwfexrvq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zyqybanf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2itripmcd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2sqzjqhsa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2pouupfym.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2vavtcwhn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ctrkkvyh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2snrptnmz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2igyvbcnx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2znqtbyoy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ciadnjtc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gzetqspw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vyqqpice.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2lvgixnty.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2dutfcxhb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ljehoino.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ekkxfuec.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ydrjskvg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjcfldub.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ebojpkjs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajkglbot.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jdnmpjkp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fsgjfkxk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zmkkhldj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rggcirrc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nqbmgvlk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2eyowefzy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2juqkkefw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2prmtpddq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vphkfahv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ykjiiqti.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2khlmbrrf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2nqnrfmqq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2inuvqxyu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2remcgkgh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zbdpsnqp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zvudbvvf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2amphqasm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2irhakczq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbtdyeth.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2mgregqlx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ezbwyrkh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2idffqkbp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2hrpqtnap.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2cykttunz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2yvorparu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2taxicbvo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2avrxqevt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otlkaxos.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ltvtucbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghojulac.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ywouwwhd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2scvgfond.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2biqtrrvx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gzojssxl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ghkxaktt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2srgmscgm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ezjdezrw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2lnhwfkbd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2oztxehxn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jovcdhrm.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ghtubcte.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kdcjnuqt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vzqcvqpm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2scsatsky.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2sapylbbm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2iyrvquaj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vfkkchub.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lykvcclu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xicgyqer.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jiigqekp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2npdkxpxn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2pgcfwpwx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ocxbdjod.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wuyezkwq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bcrxonxn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ffmcitxd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ihentwqs.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2duhmedgp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ptjmimsf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vqrzextm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2shhixhuw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nlaakdmh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ltvcfjgv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2amgqffme.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xdoinhgy.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2upearjob.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ntcylipd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qavrygos.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ydtnhnhz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2eomhyejd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hemauphy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2xvfyhxrj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2xuvjpcrb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ozkfgqrh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hgiaiyql.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2erfdebgf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2fiywcnbg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fwaudtra.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ffdqjvwo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2cbidqgfr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2shrfefdt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zxzakkre.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2fchmkmdg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ijvxpsjx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qvwgwxxx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2peohrxaq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gsrpqkpf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2kwbokesv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vkpcfnok.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rlvrtuwk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ptzwkpfq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tzegspxs.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zmsfvqym.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2nxejrwaf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hnyudnpc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2utfkqesw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qlhgmtid.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ztxywxjp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2fixhzoaa.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2kizigfyr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2cbqobiaw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2wfhdnzzu.html


<!-- 参考信息 -->