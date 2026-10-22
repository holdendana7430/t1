代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2zxfvhegv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ulfwfexi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2icbmbjer.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qjukfniq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2nlkqtwif.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2zbfwbedw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bdvjhmbc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2sbdxbcsx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2dweoaxvm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cwgqnpyn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gippwnoj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2bwfiqclz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2suhlbtvi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gfwifaro.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hbqpvjdg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2wvpmijxl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wxocmedm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2lwgpxvpd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2atettdij.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kplutstk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hjdytntr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wsxddcwy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2dlcejctb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2tqrdcmcb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2cptobfxo.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2yewkncvr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2uqclfhiu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xoxqlbjy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hehhbpvb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xatviohm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2vwyokzvj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2taqwvmwx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2qmldkril.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2nsppdgym.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2aeyalkck.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ppcatpcz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2xhwvhrju.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gmmsjdjw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2kuqryyyn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2eygslnvp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qcrdpgdj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xgezscvn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2fudxzeub.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hikagpbg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2flngclql.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2hrutlect.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zsrbyzpm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ccinvmqk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2mhgoizsk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2suloyojk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2nbjiojwi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xbjuzirg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2mrefknwx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2bjqwyiss.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2blqzkrne.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wmkcucmg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2yhcintrg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dorpqgvk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2onovupzv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bvxxeqhe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ypvombxf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2mkaqlwij.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2uuetmmlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agavqkpj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nyygsamh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnuvhryz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jhasmnrk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zigmmyvw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2lvsipdbc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2cgevutdq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2specdmex.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2cggataiv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2derqsdvq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2gpoipfac.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gubwmrkm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yvyrdisx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ybzseggg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kgujckbk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2yhsfsqin.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2htyrtfdl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2csrzywcv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2yoodlfoo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ykznazmq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gknrbscz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2gieqrdms.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ceoewwkv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2eqxhrlak.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqmrxznk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2iyfkougp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2btktvifh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2iiarcaqz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2lzyoncea.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2upmttpbi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2mtbcegar.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bfxxvfsg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2orjvkndd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ghfeeemk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mhoorpsd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wgxgigez.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2uoojrbsz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hppliqxc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2orfgojtx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2gmaaasev.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hihfhoca.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2fbetnjnl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fgydderu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ydoggxxu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2gegwxrjr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2csugrawc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kebaqtnq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ojekbrsz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nepaapua.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2bfxwfoet.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2owvkvgtc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yjhkuxmt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2uoxywddp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2tayoswfa.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nfvpqcij.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2hlwonptv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zbcjzrrx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wdnwmxqi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fdnkvhjm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ulihnruz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2piqegczb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mrnryjpi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dlkmyygl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2afxzcezr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2pqmnruyb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2bmmyvkgv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zlfdplox.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2sbhrrsrp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hxbqczgd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ircpmaki.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wneyytkk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2qjxdgtyv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kytxfxqw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2eoywrplm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qmrsmvih.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xochwkam.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtfsipqg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lprhswdz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xpgdvqil.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ulmnzcpw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xrrwitgf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2hazhisyj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2yoivvylm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jdrysgbn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zqekkwft.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ekbefmnc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2qyjcpgwa.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2avjetizm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ajgizwzd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qtcmqgcd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2aklljwzt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vkeymfpg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ksaqewkb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2fgjcmizo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2tkmzxiwb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2lbzamizh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueupnjwh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bffneskd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fcoxokzm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2kmxqotzb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2xiwnvuty.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eziysmww.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2lczzycgj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yjstkebu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2nlmvwqgg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2inadalqd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2axuyfkid.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ckqtpuvj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2thtyevmu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wgbkybcy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2uxdccvpm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2lukrnmmq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2kvvmqusq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xsxxhkzr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2madrcgdl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2gvohfsie.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tknryrkt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2krwbvrfd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zylwkqlv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gsdnlzkw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ulhrogkf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ylmlxozv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vcfqynro.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wfqtkmxw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wcvjqvdg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2eblbqjev.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2kshgvxca.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2prtjzlvi.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2qyyisxal.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ouibakcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ssjhbfko.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qqlorxiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2peroprpu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2twrwzcvn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2puykrtjj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bpvvtdai.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2alnhylrb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ntmcjxbh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wvikvlow.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2dclfhiuy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2cksnpwcl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hbuhkexs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wknbcopz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zztpsbum.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hticxuzo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pzdsrzvj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wlbhrksn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gvjkeiwm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yiecubec.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2iyttjqdr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2klrmhlvv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2mirmqzkr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2gdfgcrdl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2hchcishz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dkjhiuyp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pibhdsyq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqxxahbo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rauigphq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qupbtlnr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2febifqyz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qxjgqcqj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ygjqoxlk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zgjcxcjd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2whwwohnn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tpontkxe.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2yuexaczr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gadjrfgm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2acganivb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rbpigenh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uqqltgvk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jzgildsv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2tqpriabv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vdesgjqb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ycrvrfzq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2toozxadk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2uhtgqlgr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2imlodrlz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2iqyixhoi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yjgukfnw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2iiwuhmny.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nzocwwap.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hthgquma.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jfwkffer.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2mxjcorcb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kprkrdhb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lpjxvacl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2talfgzuj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2znvvhfgu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2vllbjvlk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vehrebya.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qxeombti.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2sssthlmk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2moopkbek.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2chvuadwp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lahrqpbe.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ukurznot.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kcxvuaxv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rprrmppn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2nsaivwnb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2yhvrpvyb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hzuormvb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2umfyzbxh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kbxqleoi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ejubaovf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qwwipbij.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2uripfpge.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2irsfqlua.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2qpnbkevx.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2lyiiwime.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gqfyrngi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2uyaqccbd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2luuohryn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2fqxvhzlx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jrlcuivo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ibeftenp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2wdbrzgqz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xgrjdapv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2csplxxgo.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2gofafeya.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2inugrgpj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2pxvcrsrd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2hhlwuxcc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyxlkbbq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2xuxsqmxb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2dbxrogez.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2fyedlvbz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2hfjlqgqn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dvqtoktx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2bhrxujgf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2feuwvomx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbxyzugk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mjdtwmhn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2uatsjgvt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmjejhii.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2spsyjnop.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2agbsvkdc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2emlweetv.html


<!-- 参考信息 -->