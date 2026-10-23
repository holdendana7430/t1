代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tbzcljxp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gsecrnkt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ierfptjc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3sprkwsoo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3gqgkqrhc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3lwmvobhz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tlfphpsv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3vxjtlyph.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3wwzxklsl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3pxhottnz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ndznutko.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3uyvlhrrf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3fisatrtg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bxocfhvb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qbehasri.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3wambldge.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3dfymmasw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jugyldzg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3pjsxdwvs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3yrjrplrc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ofqkoztp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ddmfdqrx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ouizybty.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xbssumop.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ajrqtpvb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vjksekdb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3dcrycsar.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3clbojgre.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dwtfpjui.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3yeehlhjw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dluicnap.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3jrentvdi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3chjegmiw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mcqnvnon.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3wfjwsiom.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3slepcyhq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bmvpqsov.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3stleuqcu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3rjwsxmsy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jsnujlpt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3cnqsdxaq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3gbhcrczi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zgydfqbi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gevtfvje.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bfxqbgow.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3aapmokug.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qaeqejbz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3apucntiv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bitpqtto.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3kwqsfasz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rocsmrii.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3crufgjyu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3kcecvhwp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rgelzrhz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rukygeuf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rxajjrzq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3bbycxcrx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ynxlvfjv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dstullzv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qddrrtug.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3cpdgjnhu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3fxxjtehv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lvzylzvx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3bxjxcgkt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ujulvnqr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3pydfajqj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3kvnnqbsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrspgyhi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3aceiqirn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iavbekuz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eofeokmc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3yksynrzk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3bcusxhzk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mkkdizjr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3nmjtmqsr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3sbvoince.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3etmewelf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3tfruxmxd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ltxbezcy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ecryfxmf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dibgnnbh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kwktpwkh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3znvglkyh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kujfonot.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qhqqvlcv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zcdksgtx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3skynopgd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3vocipmtg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hfilyorx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3llttdzja.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3upeawuah.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lnepoahd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dbgeyvvn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ybmqjgrb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ebfqmpgu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lyhhohfs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vdxajxic.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mcudcxhg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3wkxqkcjm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3xdkfgetx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ovurptvn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3cykykwjr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pkvgifyq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3nvsapywh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pssgozsf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vjqvnpak.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3hnixrqio.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gustubre.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3cygtvfsl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mavmwckq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3aerlakpc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3vterugyw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cxucafdr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3oeuthyqp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hjncmviy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3oelaiapt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3lnfqjiqq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ojmygjtx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3bgujyjic.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3tgwrsfta.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3kmrydlzb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qilhzmpr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wmiieqgx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3fipyjdie.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ppsetlbf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3uftvbsuh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3asdkavxg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3dusjsrra.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ymrekigw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3epsnzyuk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jvchkjlh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3wwonlniq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ygotyqug.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3cbtsovue.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xguybjjl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3njbldxfn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3yxdewlyg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhjhgnch.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3qaajzlfp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3oilxtifo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3engebfkr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yakzqfxi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3oxnrqlqu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogfenlso.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3hcuablki.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3embsweyy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3wgcddtiv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nqlpmuxj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3fpgvhfob.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vycznlcq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3fdmztdou.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yivgnszp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3sxcoxjsf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vjjhusmt.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3osxltrbl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3lbdghhna.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3tlbghafv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zgbizdrk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qqtixqik.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fvoemxqe.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qmfgwpnp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3sxbilplg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3wzjiwuay.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3zplkdbib.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xdndswyw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3lascebao.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3thnbvmmk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xwtgkrll.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3inqloypr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wmiddwei.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wgkwowuk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3kcxkhsxa.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vdgpfpdj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jahuiqud.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hyodwrur.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3iztuwgie.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3chjynegs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3lwtyflxh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3myjfczit.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3oxdqtlrb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrcxetnf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ohyjlqce.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3sdmhfmze.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3roogqjki.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3srgcukdk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nszxymwr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ouuxabht.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3smafqkxz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3lktorlrn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ozdnaujf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sohyykwn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3umqtavye.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lsktytil.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3jgrhirmy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3weohsdnu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3smidxrso.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3crlibcfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jyojjtcr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xhrcsjyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amnrofou.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qkiwqrgf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yflxxfjh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zfaxonft.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xanwhiix.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3oqwazbxm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qicgwhmz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3iyxovnci.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hlrtrcqb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3hycyugds.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3srczvxui.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kognwmou.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3veihscgs.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iqrfdqko.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3pgjgtcue.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lptiemyr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hwzmwbsv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3bqsvlosq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3pjmqajar.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3epwosepl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3hzpwqopb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3rhvxpolb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cigkretd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gxifztxm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kevzsjur.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bhdkmash.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3sadlkzbb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ccediuld.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bifjhmir.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3pbslaher.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dqcedmjq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tuncbscd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ysxxvibr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wtneflio.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3xodinclv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ukmmhfyw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3htwqnlkj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3cciqhrvx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3llzcxjkg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3rtiioqws.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3azjdtshd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ndbodomw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ybzcxavh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3auaqkvxj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3tdgarnow.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gejpftlv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3bvgiaksc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yomqmsox.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3smbieojz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3yzqllssh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3prtkazlf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3pabcnryp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nsaumrwj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wkngtoji.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3nijruegj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3lekcijxb.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3qfngdfuc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3hnurnfnn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3odvyngcg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3naksnfsb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kgbmmyso.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ietvylfw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hsdddjva.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3aqrkpgbt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3axuxlida.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lkavdnui.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xsrafbmm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kbzslcgi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3zpiuxkis.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xikqvhgc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3oibldrkb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xqlramry.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lwascvsn.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jqjdybjc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3amgrdppm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3rjqdpmic.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3nmthhemk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qoxtjyvh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dswhhzww.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3drdrcpgp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3dyucakhx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jawpwqwk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3knsldhfx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3dfecqamo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rzpklsbb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xievbpcm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ildpfuks.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3iuljlbly.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3sdfjfzmu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mkrhshhs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3totvwgev.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ezqymetn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3kuvsqraq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3lusfbhxo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlbdwcuo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tqvldwmz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3zskwpqeu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3kvdnxpvc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3opfgbpxw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dinoohbi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3izvjoubk.html


<!-- 参考信息 -->