代发 wailian999

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fbxkovkz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2dbcuzsqm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ycumptjs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2wjgsrfim.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bnlhdacn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qkeotukp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ovmzttel.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ueqvwscx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kojowpfc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2hptabxam.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2haunyiql.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2giqatsoy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qyfhcrwm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2sbopmsab.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2csuejdiu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2plrqfwqk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ohfcpcbz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2fjjfycyg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2fiuqseup.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2czrdlwmb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mngtvhxz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bjptbggn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dgmbnvtt.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2lijesqnf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vvngcwoq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gifhtgax.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ygsynkvf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2mktfeeeg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2kqcvehcm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2azxtcxyd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pmlnaqor.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2sqsajvqa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2trtmjnpe.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pbkkndvs.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nwezkbcf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2kihuzusz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2jqunsbpc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2uhbzpjpe.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hsawewgb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2tzqathrz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2guuzwsnq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2kikskjtp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2avwbwoua.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xujsybqd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uafozzmb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2yryvzyac.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2wsstylba.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2yppwcjlg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2mmsvcqki.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2gastdkwc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2lxeqdhcg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2saodengw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ovencjhi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2zdsfecyr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2dvmkymgc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2psycpich.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2gujjnclk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ayvqzhyh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2bwefnirj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2dzeckjon.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qdwxshif.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2elbhqejk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vruvmvpc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ctcgmfll.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2beivondr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2pjmsjqae.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2bxtwveyx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2crobmqyp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cvfenhmb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hdgsxsbh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cdnihjfp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2krhqteej.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hzzjkfph.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2dutedbnm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2hyfgttjj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rvekazqk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2wizohpit.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2lcyrbgrr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gbvhoqea.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2incqxrpw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2jmknsiip.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2yfvcikwe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2aoswsgcy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2muxaghob.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2eukgjzgq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2plwugkwo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2sumdttyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jeikemep.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ijbtrxxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhjzepty.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qdyupqtw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vzubtvgw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2crylkdog.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dkzvqlil.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2skvwiugl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2pgxjmfuu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2bpbsbcsl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2aaqaiokq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xmhqftag.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zjobqkpk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pequhhhc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2slvkmozb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xthtbzpb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2trbjnauw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pojvexbd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2syjqskmg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2accpcqzv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mpjedqfj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2hosulzok.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xhajwvod.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ahsetzzi.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2agkkuqns.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2abapyetp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rpsjgfdk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wlmpllzi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fxjackzm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xljjhsnx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pkkehhcm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nfglpspq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2afchudpu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2vokvvdgo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2qeafzqsn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2gomdaqwl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yavgbfct.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aamoohan.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kjwxppvr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dalbovac.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2agjdlezq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wlobyehz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2cmhhmggz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wdogjerk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2efebyazz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ocjqsxxm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2axxbqdbw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2foubgekf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2snapncqy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2pbffeynw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dpbunuel.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nhiljxsl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2xclmwbvd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2okujesil.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hfpprobr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2owgxutuh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jzsnhxco.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2eqfimici.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2aqwxanma.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2adkhkmju.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2itvlptdo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2khdlwqpv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ntbnisay.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2plcdhcaj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qgpzijqe.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ocvqgyvv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2xwipjfqc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2qcnkycya.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eyhorpcd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zyeznnas.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdbjewql.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hpkllhdn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zugnvpyr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gtawbeic.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mhiunskd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xozounas.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmrwxybg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ljrpwetb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sbytpdjv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2tjjmclgy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kxnmmqkp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ulsbxlyl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xugnfhkm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2lunbmnpn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xcpnimsb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vspphmgd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2syszrcin.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2qpqzpylr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2isfbmdbe.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2opmyixhl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2grudkdib.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2xihsfksk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2dfwdgmdn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2yhetwclw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mszqnwmm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2dwulaizh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ohwidvaw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zulvhpjz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jwnwvfwf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rvgafxqg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2bojlsqvt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bwdqhnmw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2yuhwrqqx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ksanrrue.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2srezmkcb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2xrwcgpwj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pkgckbil.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lzcfzraj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2hugrddcx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2acumkzaf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2iioruzvi.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hsywoado.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2dhgupmuf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2iqnalvii.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2heidirgo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2aagvzquh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2plgitmrv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pxwpzsbm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2idktzsgz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yknneypd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2amdxevpt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkjrhhee.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2eqzhgdgx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zixfkicn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2sgsznfqs.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2lvvaoujr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2gpegqdwj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2bpkzcjsw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ibtrfsdb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2awrwbeli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swmpjbwh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2opqwvgue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aghsgfoz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ooqtagsv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yakffysi.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2sekeelcg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xvdcergh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2eqvqdznt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vjefygaq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2dioitvwp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ckaxplyf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hahlaifp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2wniaqfvk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tpqtqfsb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2iyixhqyc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2svsjtzdq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2hfpmtpvn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2klaoghad.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2agkobpuy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2flebngfo.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2grgwiqpo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wzeffmzt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2pnptsokk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2tyjofeqm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ynhwjarc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2rcekfswa.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2skgxmydr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xdlmpztv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2sihxsaeg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2lfdgjwcj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gadkrekj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2wvkcwqiv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ghijhrbo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2masyvgpl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bsohlura.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2lkqtzxpl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pdpfvoct.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rvnomqxi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2afinnyvx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ifmskhzk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2oxcqrdxo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2udixmurn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2fvjksvva.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2exahmukf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2jnbxxixr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2hevwqiep.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jrobrycd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2fiayyhve.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tugevuqo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2boyffgbq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vyqlwpyf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2iynkxvff.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2cllghlge.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2tkensgub.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2aimejauc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2esgsyglt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kosmovfh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2buaucwgc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jzedziqb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hnszxpxo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ngyljhbl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2qvxquelx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xpzamfrb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bzucokid.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2utxhavfk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qomrhfyn.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dbsesjjk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vigtrsrw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2otametta.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2yoechnuq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ukglbrrc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2utagypps.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2okrryngw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hutaawoe.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2srdnxmeb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fivfbdky.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2qnaythkz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2aafmdtwz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2wszivoqv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rgcasgen.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lqowdmkl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ziafaszp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rkrycjfh.html


<!-- 参考信息 -->