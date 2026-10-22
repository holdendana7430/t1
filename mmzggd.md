代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2qgcntucc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ldxsjpzm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2obqhzaav.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ahqhhpho.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ztgahgfv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2kqyqfdmu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2fltjhxeb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2tkfqgiyo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jicsoaim.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2htxcardo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ujutnmyc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ovapitwo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2vryoglrm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jxtouifu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2soxpvqil.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2pahvhyxx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gklfcldu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ouedhawb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2lparrydc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2krdqfpzu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2pnthtrbj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2eucdtggw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2yjigkbin.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2dtafkfkq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2aysjojja.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tnydombm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xxnxoxkp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2xknxfifd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tboaiviv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2clnvhpsv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hoxuauic.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2svdvqkzw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2whuyldgg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jbbcgqvw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zazcgatj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hytujiqm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2qdanhttn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2bohlrjio.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2twwrcicc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2kvpbhoes.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2emmutyir.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2whihesqo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ebnazxbw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zubgwhvt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vwefngpt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2yddnsymo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lzutqyml.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2pvqxszzj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2otgarhuj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jxsmnyxw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2isyemstx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2osnnjdsa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2emtnxmae.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2kowapnfc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2jambsifs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jekeoxox.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2phhkfifv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txfufofe.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2avcmyzip.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2wmvapyyc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2svepncwv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jwlkbodr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2atwhqzcy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2oqznnmqu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2csmggaor.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2xqsgwyoo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2doeasora.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2omexynku.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ldcidrgu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wypcvncj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2jsyojtve.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2mmmysrnr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qobdkskk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2mfdlaica.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2idinyyjo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2muazdhcg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2uqemttuu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2capvywuh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2qicwktmt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2aiqsawkb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2bxmqleeb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2oljtibpv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kqwvgwri.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mexxyysi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zbmvdebd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ajmuxrba.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2oubarnia.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2pvmxkgap.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2kimykjur.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zhjzccjj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qgwlbwti.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2tdpropvo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gwxntfid.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xmsqwasi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vzszliva.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jbetayei.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tlzhwcfv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2jpzdqmff.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wyvwkbjz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2pziplera.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fzvicwfx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2dybswynr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2swjjfnia.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cwaihfbf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2oyuxymhx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dsibvtfm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2efgmymgx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bvaocgol.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ikyrdlxv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xephpnjy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2fdmbtjqd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xvvagzqd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2orovizvt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2mlqhujtm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2arnqbwjf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ayjtwazr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2kjehwgxy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zxiwsrkm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2imicvnko.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nlbjmctr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2oxfcmtjl.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ylwpwcyy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2yetvaviv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nvgkppnv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zdzyyyaf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ixhylfsj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gnsctgvi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2sljthlbn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2dgdvmcpq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yvtfegdx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xttwulae.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbnipkkc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wseyzmje.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2baxdrwsr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2vujaizmb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jpuicsjo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2yrpiyszj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2qbvclpak.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2lwraspgs.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ggdqvvzm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2muoicjmw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2cjiiwwia.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2jijpdivg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hijozjpw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2huvrhozk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2dofngcsr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dpnojvux.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2lzhetwqu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hbqykxmt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2teccqqkq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gyfgbevo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2svugmway.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fcprlvsi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2cwvmcegt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2licftlha.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjesbrng.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nuhpezxc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2hloondkt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bzvkjtfy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2dsdhpqlg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2iqkztqkm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2aikrweuu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zjbvtfvw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mfzqlejl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vavslsnw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ikdyqfdy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2djmyxmlx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2gxbvcdid.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vabgcntc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vtabctfi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xoqgdfqh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2gogkqogm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fkvxwxzh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2sxrlfbcu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zlbfqisg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2efegljiw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdzaqptp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2udijzeej.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2egpaqqmh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2xjnmotwi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tykowtqo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2igrttsys.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2iqiarybl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ubrugrkx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rhswnivt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yqkxfhhl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2fklwmblx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xokvtmbo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wnjswdwc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sulyoujs.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fbvbdmre.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2nnbfmodj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2tzioltla.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2trppssjo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2nkmqbojs.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2jcaifadh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qcznbxdt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ifweestn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cdryxcnp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nblrbpuf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wgzbsxfz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ywjurpka.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tagkatio.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xeqzjtym.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2gsfqesva.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2yawjrkny.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2eycskxmp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2qozjawso.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ynqlwnck.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2lwafjuku.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2pebsgspr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ropjlsun.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2eppavxqt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qbfjmgmz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ldqutprv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zwzrpizu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bdpfvjyg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bifuxkjo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gfjlzagi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2erikncft.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2aszagboh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2juarsiei.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2giwmpyxw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2tsuqfktl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lrjtveaj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2rvubkygg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ezgyjiqu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rfjozrpy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dozsugbq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ccgwqgyb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jtuubzel.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2duceublb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jjlhjxwb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vmeqrgtf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2enklcoob.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jwspuylj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2eugrvfhl.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2iqqfbiis.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2oolpfiue.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2qcgjioyl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rxuuwvcr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2heefdhle.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2xpfzvpig.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jsldmkjg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2unvwbikj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hmakdieu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ghocoggy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jcgmhyaz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vefkwvjh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rxctzytz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wlvlqudv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pybsxudi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wrkdbjqo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2jqxkwxzs.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2dbgdxnkz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2hmymslkf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2nwuejfsl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dbeppgjy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hxktzlgv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ffqeyxxi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2acqfcskh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dsmlxkbi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2absnsgpj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2nfudtoyu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pkhneqyw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fcnysnas.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ekhtfudf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2umamlkqh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qrmxctif.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2eogbrjoh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2axkqjiac.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2rqcxmuxl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fbskinxd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2axeqdmju.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hiuljzdv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjsviqir.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zvdodwai.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfvahgkb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2cbcywveq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2pdxkahvc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jawknkzc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2jwhexjos.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2jaxtyzwu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2upimsukh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pktiquiy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuiwpslk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzozunqh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2axzcaydu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ydqdrjgt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tofonnrv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tbaiqrqc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vnxxidvb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hqzwcays.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iondiuln.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xkoqlpwi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2orfsdkth.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sydfixiy.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2auhyqjpv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lklsozqf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2xzgfpdtd.html


<!-- 参考信息 -->