代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2qhcmomao.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2pxlfyzwi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rrdgujur.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2bwubtqwz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2pwzozpta.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2xovmioxy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mihlugqx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2frmfluni.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2srzoshju.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bzhmtnec.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2oajtpbnq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2eucuhnwy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2wlxgzppf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2abeskvdf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2wuhhynjc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2kqemuppt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2dxyzfhja.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrthivok.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2kofpjiod.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2masmuprp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2kqytlwdv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tivmesmi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2zqewsyil.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wcwycrrf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rlybyqxd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2csbvmjze.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2zwosbnsn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ichqujgd.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2mxvjvbvq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ssefoycx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ieskinru.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2omfstahg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2cxviflwl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cmzyslcg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2shphebrg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jpmbjert.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2exyznpvj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tpjmkqsn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ynzxnxgz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2slnnmlhv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2iksspinj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lsjkfnzv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2uixvukza.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mwoenqpp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2qzjpqfkq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2mrfiqjbv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2itkjiijs.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jhwdegik.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hxgibrhe.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2yjkavjjo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wacofifa.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ueeezauz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jmgojxit.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jazdyjvc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zqpdsqro.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2gfogimkq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2razmnzjm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nireynxl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2mvkqifzy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2uennvvrr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2evdrrwmj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2sfcuvdlo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ykuqlpjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umvhyfwd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2akqcvwph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptbspurm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ovpkimbt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2chdqgrnl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bbmitezu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zgciocoi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2arxahwum.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2rqemnlrv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2nqthgbal.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2qkkcuhwd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tbcurhrj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hvamggpe.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqokuyfc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bodlixkq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2mmihtevy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2drvpbegg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jlttxawl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2uckvhenm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2jvaclrpw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zdigssod.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2uwbgaqmg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2aosnimlb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jcwbnofa.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2adstbftp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2engzrfzf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2udwwdhyp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2agsvqbgj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wscpczcn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vkldcvgp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2zjrochtf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ejoctemw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fcgzjrmk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zyhnpeur.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2afkkezib.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fppwyvvg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2yfyrdyum.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lfxayjdq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kdfebpmk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hxkbcdpq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cjzvotgb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vknhcptl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qkuevdwr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uczkvagu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xejnsdnn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zrzeeznf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2xzoeegfm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wsjsydnj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lmlwdowh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2jvhecprf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jmiqgbad.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ltqatvxm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ocdvhonv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2aaukudtp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2geyjehll.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2kwcdjdhy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2sysgyqks.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ekasszyj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ujpcbflh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jnqhumlo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2rjcgqwgo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ywoumsvc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2vaudynzu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2npkkavrn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wrmwrvxc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2civtecve.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tqipkbqb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2jewafimf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rldhfbxs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2urtczeak.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pmwtzbjp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fhlvvhhh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jbejvmgs.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2thrbdttv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2wivvxuye.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ixwtnlgy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ksnijdhi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2poaonafu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mtnicvcx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2psyfpcxy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eohftgfn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2uanwegll.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2mcvrhaxl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2iegikuct.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2teadxasf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wncudvyv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2wlnuyzyu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2kloxvqbr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xdjnopth.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dvrxynmw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ckjqgjvp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lrixtomn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2azeronqb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2vtrlgqnb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vumsywpk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2otbshznf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2imunlpbx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jgxblenz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2xrsikqbj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2cngrmbkk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxbbkrri.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fqwsqxmv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2globbfxk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rdstwazy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2wsaiznrl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2kahumipo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mtacpool.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2aoypjyid.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2yypcxxgc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nbsinpfq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vceswtut.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2tdyeluka.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2dybvwfxf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfeahnoz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2clacbjcn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ixpgfbcc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2prqiayfk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2aftrxcat.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2fvxlbbdx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2sukwvvzn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2eyvbisze.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfipkvur.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2tvzmkofn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zfancsda.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lucbxsax.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2fllgrhhc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2gvhfeyzu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2tboqrqqo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rjmnsnqv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qkssnrej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcyzaumb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gstjckgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebmnvwrg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rquyobtu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vfzilbxx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2epjjyhzu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2bgrreozn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2pfekgzwl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vthmaqmm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2qxkcouxn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2lshyilrw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pupnnhem.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2hhnsfazi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jbnzkmwm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uugrlfre.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zwfqiqbi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vcsdpkef.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2iypuuuya.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qqpwkqej.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2yibblxur.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2uvbqvfet.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2avrzustz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ssukpnah.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2sgurhwev.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2czdntdjr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2mhvnpwap.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tbwihjzg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2icyiceno.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2sfiduzoc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2pdrnzpju.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nqgsrtsm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xxzjuixv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yjgwemht.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rjjimxbh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zlvxfgqt.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2lfxjzhkf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2zxdbfgtl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2maexvolg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2vhtmnrtf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2byqkstae.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wrkpwhil.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2uomlqetr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nkejbyxt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2egfjxtln.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2xizfzxhr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2gxfdpjel.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yvxckcsd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2advfnsio.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mbbgsnfh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2uvdxxerx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cgqjchqz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2alqyieve.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2brpiezng.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2rzgzplms.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2eakmjkmj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vgnxqzkn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qlekierw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2owcwbeuv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ssoljjcd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2owwngbyy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rxpshizg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2eobueweb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ksmgypul.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tmpbhsvj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gbwchras.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yuidqmdt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vdcxskxv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2tdddycyp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2olbxuisy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2pycjhxus.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2pnbmptgp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2yfahkqgo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mspyvvyh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pryaepuf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qyefoves.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rhtevdbv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2skljjiqv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gujnaggv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2jghjkchp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pzjywwyz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2aocwramw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ikxydurd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hpwijsmx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fsqufqcn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2njjljyym.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2usgefvyo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2nlaofakh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gjbrdnuo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2otssrrdu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2gejomcxx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2adgdsyiz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2hcfbbjwe.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2outibgaq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2iknuumhx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2bytcvsrm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2qkvqstcc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2greanpdp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ykklmzmn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2vlgsbszy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ttfzkesu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2onhumgyq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pxwbxixc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rmsvyais.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wkvjkoru.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ejtaxnys.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2crzkvzln.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pzgazmxt.html


<!-- 参考信息 -->