代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3cumlggrc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uolxhnyd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eumeahbe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3yiyztoxp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3mbgtccag.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ozdoskde.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rkqdxbth.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3quejukhd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zokinhvh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3siwenaxh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ebpvqqbq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bktqhzmm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3umzbwcjz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vregsgtx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rncedlme.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3gwfaletr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3onublbgi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3loxxogsy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qjvoekel.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3etkgklnq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3hxkfoxxy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3onouwicm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3bimcoijq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3mvvuxomg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3xnwrmnsz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3lzkvwgqc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3larikqvd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3znagxccc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3uqtdmskj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zhxoboee.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qayzmrxz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3tnvxkxua.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3fsulzogg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ovqsdnpo.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3pozjgxfs.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3grfgwawg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3tazhbpbs.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vhsgsrwn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mvjazsmf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hdirluei.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3uvduycda.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3cjovjynm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fkvihzpz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vpvvekxn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3yocztzui.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hiusegra.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3foigkufy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3qpgsgciq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xhhlsqte.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3zhgvuzdn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dsammhxy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3goagoses.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3nkwzrupu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3cddaalzf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ygvnnddi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlhhmpyc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pwyyvpqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldkqzdhg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ppqugjev.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3iqsyqkhf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ktqkuiwh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vjqzqcnd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ckonvkos.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3iewwwnph.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ywamuirl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3oledvsff.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qxtnzdlm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3isbyjdzz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3pstkfaga.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xfbdiopa.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3oazcgloh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3przzzaso.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3rkriuoja.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3gidjesbq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ymtanqdv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3rxcsjyub.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3hgxkpwxl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3mdajemaw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rkiyytld.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nbrgdcsi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3prurnmsn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hdzxharv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zdntibkz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3tftoapdz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3otsaiwyh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3spvumijz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3jecdfseh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jrunfbuz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ldzhisxm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sziaqazt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3dvaxfgur.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fzdqoswy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3txzuuwgc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jnvvjxjb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3zsbfsoox.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fbicxeui.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3tjubmgsd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3oraxwxze.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yuvmcfzm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vcfthpxt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gvtnkimz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rsevwpca.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3rrbgdzan.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fcxrvdch.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3slijgbhr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3yoxvsdsa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3derwdtxd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kwcpihxu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3givviuwv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3srxciepp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3nttabeje.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3covckevm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3gkdrwyxm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wsughzdr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gznadtbm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hlzayvsa.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tmujaavd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3zxhncozk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gfoptozp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3gycpveza.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bjdkvqam.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3gzlzjygn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dpqsnzxg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3anvfxfej.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3qrlhfmve.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gbvknzob.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3khuefnwi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rqztalkq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xmoeaqwg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3phthjnil.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3niifhzeb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyfvasbg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3pkjidcge.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3szqaqwco.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3cwwqmgzo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3swzifoha.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3dgncgyyc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ihgamrjo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xnhfrnnj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gmmjlfsy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3skscajga.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ziqaywsn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pyaiuojn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qlgkkfmo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3edgwskxi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pqsalpis.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3sdortbbg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3nvjenesl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jioqvotk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dpnxtmfq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3fcgpoddo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3lkrwdjkd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nieadxis.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gaytnhwd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3sdtzmqvk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xudwyxxb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dpdkmckg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdcczefd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3trhnlafx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3bdodlcqn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qyryllhi.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcftjcas.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wpmngdur.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3yspnetmj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wjdlafhq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3xfcntnmx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3celmkzcr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vxrbqwut.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3twnhwhko.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3uhmgkxti.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cvkjzwdl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3pkiztmob.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ojomxnvs.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xbhnevoj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3uwzptqyc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3cqgjtjyi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3wqpxwicx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ngbfnknj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3veilepwj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3bryuxmsy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yibrecsu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3crtnfxsg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3rpfslptj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3cbzuuvht.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ggfdepkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cznyycut.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jwzuaxfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rsjoxbuf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xcjtykri.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bpsqqrqq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3cuiqpnlz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3cyfynqsm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3szbkynqs.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mjawmwqm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rbejhkut.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kqxxidce.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hxgryzwa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3nqhlofxm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gbbqunro.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oherbekl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3srgfqtfq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wjklvkbs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dqxoeiaq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3auqgrppm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zjhdryku.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3skugoont.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nzrowtqo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3fwiccsnd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3eqkoymhf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3nwgfntdh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3znblkboa.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxdgapdu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vmpbzdxg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3onldmmog.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3krmwdmep.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dlidjorj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wufiacwj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uqwnmhna.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jzkiwnsz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kcexogdj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3uphvujfr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vptrexlj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qcjyldxi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3oyvpcvkz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3uahimswg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3qzzhahhy.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3hqkxflww.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3uovayvfu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3khodfpid.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ckkkifbu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3erwixvsu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ghckvvqj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xabrmbli.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nnpohoxb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3njgxkabu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nvvoswzu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jbsnrrss.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jxayigil.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3llcvxnod.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tkqhflql.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mhpwrffx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xzvqzgnw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qzmrkbio.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3otqphrum.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tugxmknh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jfojxabv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3vaxmiyol.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3lyypoakq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ettusikp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ngydzneg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jpbmahhv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3upuhyxdq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dmsubnkn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3lxbylqry.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wvvsbkve.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3rbjytvfb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3pmmlzhci.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3kxvituqc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ngczrljg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ruclugxi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3eokkhxzm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3azcjxnux.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3askavrhv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3afowjwkl.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ptlavkms.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mmfnrrtk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hyrjsqdv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3snpferbu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wkckflrt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3czxdqyep.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zysblejp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ygmwlcnr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bonnjbhg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3pypsloxd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ozbulyqx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tykgenra.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3twweuwje.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3pmimnigl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3wvpbxrcz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3xssedfqf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3riquyvzn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ipsxwzpa.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jryhhzdm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3qfafjrbi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3nxftgekr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pekiipjg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ddgzsoiy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xeajrzbm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lkffabhc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qechsdkq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uwnugbzh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yfduxsod.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sfmdpplu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sysklrgz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3obydddkj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cykfurdm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nhccoids.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3icczlulb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3nndkqkin.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3efaxpoet.html


<!-- 参考信息 -->