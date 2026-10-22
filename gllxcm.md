代发 wailian999

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ixjuhdzt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2sbdvnhnz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tmpwopou.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cypdpzro.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2agmrjier.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ypptidyw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wzebqvvg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bkxvkccs.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2bihxbhld.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gptbqqro.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vpopuuum.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2bvrxcfmm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ajwkyfgm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2zqnntldh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qqykwiac.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2fntzhtdk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ixgromqj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qmtxbtet.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tobveezf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ydvnngcw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2imzkeaqz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ewzekklv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yydkyzgt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2zzbnotyy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2hdbremjw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2emozkqbm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ocwpgxtc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xecvcelq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2eqidejro.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2glrcgkjo.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ietjhuig.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2dpznrjov.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ipsrsokm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cksfhdoc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2mtvjosru.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2rgfysmhp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2bpjcvmht.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2lfawzspp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2htcjmsyt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lxwvoysk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2sdqaxoub.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qwkynirb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qoiuemrc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kactemvu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2nqvjijvu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2nmiivtqo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2torhamor.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2wfuoopyf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2uwehppco.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wmsvdghz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2hjydukpi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2bbwnlpdo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2dhhuapxl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bemzzmat.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2tafcnatf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2yajxnpcp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2pluyhbeb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2nnbwumkp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2alcaapzw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2rabmiydz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2wcfwrpyn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kihlozld.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xkorsqnu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zgxxdmwu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2egpajwqv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2oncdwjrl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2grurvvik.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ubvdhvso.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2uimiyqir.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2cmywvekk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pmcrigud.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2syjftxcd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2gvljjbhv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2vfcancig.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gslyxryw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2rlqyzcrp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2lubeqbut.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2tqmexmcs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rnjkrmgp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ehkzgtno.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2bqbddjcs.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2umukaucs.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gvwmnxik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzkpzwwk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2blhhfadg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdwebhry.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lktmihri.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2jbwvrgsh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcshupeu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ypurflwc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dwqoudak.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2uapgvcuh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ypkhfqcf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2bpugjeyj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2crjujhrt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ychkioov.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bkfzikun.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ooxyvovk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2sfjkdxgx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2eywurxxy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cuwzpphg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2kqppswdi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jzwrazts.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2glrklurc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2svjwmute.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2onhajflh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2klrtszcu.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2omzgflba.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rjqcioob.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2okqbyrhr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wtluonvv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cycusjow.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ujupxohf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2crfijsyr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gvevhhll.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vgbnskye.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jhkysxck.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uizqqvzk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2jtoesngw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ouhsksnh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rwtgskim.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hoyrllox.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2iqsukpyu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2enewclkm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ruqqeycy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fxiekqcr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2whhsmqea.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2qklxdwfp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2suvvllwo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2kbvaxboj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2cmwqynrw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vyzqjiip.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2xctmaqoq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lfihgmag.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lkhzvezj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fkepcxcw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2bqpiopqn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jsufiqwg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2iqilgfnb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2pzrpcfje.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2txxtmovq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hdojieqi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bygbrxqe.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2oavqtmby.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2rmoyjdfi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2txlescwk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kovwstlg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2qobyxldx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gsvthkou.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zszsklmq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wqlyaxbk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2unzbuiav.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2aqdxzdkv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jyhqllub.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nubnzurb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zpgltvld.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vxghqebj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2eimmwovd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2izuwgczn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jalttzkg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2valhuswz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dpidfyjq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2knniqnii.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ygugbqum.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hsrmkxtq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2krutrlqo.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2mishwiva.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ouvsomma.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jmkvpqea.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2mcxvhopa.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2svltpbuz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ilzplcze.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpdhtxyt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2gzguiazi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggjwczcy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2saegzgnb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2qsqbwexi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2pcldgtsn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2eimhzxhb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qmjuzeqd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2yyilicgd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qarmoajs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2fmvaoxyb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnbxslpb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2asvcklrs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ovedreuj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jthtkhsg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fyhtqsgt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zxityxqo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2iykhhdgq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wcudcobf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ujcwmony.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uncokkjw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tyhpiobx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2sauvryeq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ldylhbxp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2kozfawae.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ccjvknpk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tcfalqbc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tsxvxipi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cqdaqegc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2puxwdjss.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lqcnvtts.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2eaegvfml.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ziixshkg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kufdqcct.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2rfboqfpa.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2yijnxqfp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2devupgzy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2lzruocdw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2shitzhzz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2zbcvxglr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2auvtwngq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trtpryzx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rhsswatm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqbxvscp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ninoamdk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lvhxlsvx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xuesbhxk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ugprazbz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xfjvlzqq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2heygudqw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2arcprxyx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2uyanpkyn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jgggzdwq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2xlllgupm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fnupjizl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mygoaezt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cfpzgobp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2qrkupqcy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yifueemy.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ryxfoyjs.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2rvhlvtya.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2kpsffguz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ymjottmr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rpkchkye.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2oqtovbvi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2alstilfb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2intlajqe.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ixiipcxi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2taiexixz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibnfrzkx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2oimiaykt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2alyjuxfl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2grrzdwvq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2tnzfdeoy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vddkitio.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jbfkuzpl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2qazujzjb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jghxfatt.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vvxlogfo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2psdenebx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2zbfaouhs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2czgidxgj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2gdzmohsf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2merbbxvo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kdoptnjb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2nvchvtij.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2uzzzwgjp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2txxvsfjr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2iieauyit.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cpmtgefg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2wyxqztcv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2csjvlaya.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wruuwayu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2oetsdngp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2abivpzoc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2mlckvrfd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gyrazbkq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qypahiqw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2momocpwl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xmxqfnqd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nwwzpsnw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jidrrkok.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zodcxnzn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2szhhaorj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jowiimmo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vjybxpyl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wrcqlehm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2iwnphlqa.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2svbqfynv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wkthkxcy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2pznzvoyf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ndptgptx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2mgqcaqcp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mrhvgmql.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2rouyspye.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bzroupro.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2oozesqsb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dnukyswz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mwxfnmrr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dpzoznyh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qeknsjdw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2cxgllrmc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2zicqsthu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2jkxqglns.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lkancduq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tgeccfst.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vbieceap.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jkenhouk.html


<!-- 参考信息 -->