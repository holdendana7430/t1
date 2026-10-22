代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kkowfazj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2utwjvtfu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nabnkzxn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ubzftshs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2lztbsvsl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vddmhdic.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rawghdeh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2lwsedmbf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2bhgjemnw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vsdbugbp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2lteblauo.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qhrowmcu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rndsilxv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qnrameei.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ivfronaf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mgofyigy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2dhzywcdg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2uwnpursa.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2gnocstlj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2pdgdhysh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2kjatbdbh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2kxlbehpn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zmjjxsbt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2obsogphh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2bhkbodqt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ewptyhug.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2aofcrrld.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2fbudetbt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2puubfjqy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2mpjqebkp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2zkpzltub.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bjzjthpi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2iprdqrxt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2dxavyqzc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2corwkklm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ebmgizkk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2yofgqxse.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2snkccump.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2xfldercz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qulfgzia.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2olgldxwf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2smoqgmmp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ttlperlh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2pzgvekrk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2acvggqsc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2fxwogabv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2sqgacdds.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2khincita.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zihpybzx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dzibplft.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bvitaolh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ijcapmsr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ezrbxncb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2sqbmwftv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2thfdjvow.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2mkapduoh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zmgkqppl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2gcujuqlm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2shneyhfe.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2lagxbohw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2cdakdpuk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ivsrnvuh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2yjmjkoqq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2oebinegv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ilspgvrx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2olifwbwe.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2eglhwcst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwmjfohp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2unljcrmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gjqbgczx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2urdvmqzj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ewokvjdy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2yczcaxvw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2rdsyxrov.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2mvjzaxpn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2yxzaxlab.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2euxuquet.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2htmnmdsj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mwplravp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ysdecdmy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2isimxufd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pgdngour.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2nirrdcuu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2lbvkcjjc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2yihjegss.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2sbzquvit.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2lrkipkle.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fcbqiptf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2qddyjznx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zxrmcohr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yypgsiie.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qepjcolc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2yrqtmiuj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2uofozafl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bufeskaz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2sfpbrogk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cewrbenx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qvlyupkp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2qwhxhnyh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2katigjyg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2vdkwbpcy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wiqxhrqk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fjiskkjl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ryamfrll.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2poxhnqha.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cbfnwpms.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hmbgtvmn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ikwftpre.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2bqypzgrs.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2wyyngqwd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rjfxgltn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kxrvpqdi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2izwoonla.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2inxjlnzp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rdcxhhvp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xonyruxf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2eqgqjffc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ptiwdmgw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wexxlwrk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2junccfqg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2letxlkix.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2aweclnoi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2umkbbozm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2bjbixxeb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zoondajs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bxobhrca.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2slfrecnx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2cwshxuid.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2btlpnbox.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2midxnxmn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2tlikasyo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zpwawgjf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vdlrwvwj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2rhfgjwaj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xzlbggay.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eugsghob.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cddtfirq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxzodufl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oiaqzhdv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ozcbwvar.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2duobqkmr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2wwnqqthj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2iadokgsa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzmsjpsu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zwdsuuyz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jwdaycpv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gulogcpd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pqieczdy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vqhalyfx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nrojemil.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fqwgghwf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nuimswlp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2lmvxaizn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2lcdppweq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dnmwmmzi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ifwqmlee.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ahntqnfe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xkjlsnbd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ynzmepcz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2tebyuilq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lcgorjvh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2gnnsugrc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2bzjqpdei.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eogftudg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zznjjvir.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2uqhyiqes.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qshpklpt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wztpflqr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ablfarha.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2tyushnio.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vheaiprv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2nuiozthd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hyxpglgb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2qcbebrbh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qkxavhcw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dpeagnbk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ssgeqdfl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qlpsrpse.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2yszbksyk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zrcvstlw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvvmmxlj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gloxoisg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2nmavsqiq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2umkbfzqv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ucijpppm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rfdajmnw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2gqcvrayx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2dajitnwc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2whexpfee.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2houkgnnl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wkkqdsnv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nwncyqfw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bpubohnl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2tqwhxthq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2akjkeuco.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2awqlccyn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xcymlgew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nttltans.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2htdcogfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nyhyvbgp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lyawfwok.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rarqwcbm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2eziauovv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pgtgdtfm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2iemezyfy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jikppwlk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ulmbslfx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jzlkdjbm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lozyvsbn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2wkhzrjnr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2timwcfpa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rkiwymfa.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vtbekott.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2cqxgqynb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ligwebfx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gnvbglmp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvbivkme.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2vmvebzjt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2poddegpd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2mpnphuzp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2cuuarvyx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2tvfawojt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ksxwxxcx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tguonvry.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kxqiqhid.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhzykjmm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vrdtvimd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dalhdapv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fkpucgjh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2fsfoozes.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xrssutxd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tghlbivw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2papjubzb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2kgudalxh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gpfzizim.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2rcjbpimf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2shttamsa.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2neotount.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fxcmxgkc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ksmrovcg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rbftpioa.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2xvtsoykp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2fjpkintp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mbyqewlm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2bjoaswis.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2bkvzftih.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oglekiwh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xxqesboe.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wwfmwntn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2itpwpezw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rpnzyvxd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2fjaxwuev.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wszghvjz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2novpnloy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2zbrjuswu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2mkwrxsck.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2epclxcgh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2sohchcfi.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2czjkohst.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2hkjkjufi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bnoiiejt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sxyauocl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ubiumpbl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2vzknwidl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ztimxllr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qyylluno.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2svezjzvc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2qreqystx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2kbqsrscq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2stwqovzj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cdiofqic.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2grcutidj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mgpwtagn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2wiqcubxu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nefelvny.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2vpxbcvgw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ojoeysbn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wwqilegq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2sffclguu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2woueossk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2plvlvuma.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2yqskzrpj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2nkqewxfd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2pmwhxpgv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lpagaeoz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ckxfatql.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tcjqtmfs.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2meaeqqqm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yzbvmbbt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxtwebwt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2gufnwyfv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmnggwmv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2kggzaqfb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kslsnsvd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qagjczmi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ommkuuus.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2opyptpqn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jjavqels.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wjadorkn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2akxrtecb.html


<!-- 参考信息 -->