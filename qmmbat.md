代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2igkgitgi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2sjauvzmy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2cjowdxed.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2itbjvdon.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2gquqynhk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ennsdeuj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qgfotuar.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2hfqwjjht.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2cpifwszx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lvfwrazz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2vpnemjbc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2oqilfhyw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zheakzwp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ruroiunj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2kpexxnnc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ofyqbjsi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2sppqtcil.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hmbsmnmc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nnshrzeb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2kvwwjwpw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2qchoptyo.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2iortditb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qfdlyuse.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2oufgrpdn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hxjulyqn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2oiwspbjx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2mywwmyxh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2vuxfleju.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2duzatsnj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yovbruin.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ydlyxeac.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2utviclzn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2epvxvbhq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2zhfhqfgs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jmjudkev.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2guptswcj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wihxxtgd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2zjuhddgi.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2kmgddlbg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2axpdcztf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2tokoabui.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tkgyfvfo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lgabpihf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2akgulrcb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2fwapbukm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ygmzzltg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pmdabuzk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ojacdgzo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wphhfzme.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2yqgjhygm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lhdtcign.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2upbgjtsg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ffecumhc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2peijxcje.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xswpkgxz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2heyiysvk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2sjqhfejg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ykodxyyg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mvevtlnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnqrvwek.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zkntaqzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldzfhpwd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oiglvypb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2tnfmdgqe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2vflzqhnk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nyimhbqu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wnvnyhbd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vpzmojcv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ctsdmotf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2pioifwil.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zitbmulq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2apwzlgau.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xheapvku.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ejjwgdvg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2cjgzncvs.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ueillplc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2nzwuhfpn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2kvfuzwsk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2rmwkyuhc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2smzwxwvq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jtzwuhed.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2kphblqsx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2byutyfgr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2whtmrnlc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gukugawn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2lwtjqbmy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lhfwokzf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fdtfmxbz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ekwiyjlu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2czsbowvb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2tetvnfzu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hzhjxbpk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hoipvbub.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ujmlphxh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vpujrxlz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2hpivlpye.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jkebljsz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2irhvwitk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lvujfnuu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2smmosrsg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ftvofgbr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2wavutuom.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2awreqide.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2gsjhhkvq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kojhafwa.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kfmmxrna.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2khkpzyog.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jessjokv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2izndyjhj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xdzrjaqr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hfucrenc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2oljpoptl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2esumgquc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nevhmumy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2sqwplajq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kdxgrsgp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2eacixegy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wjwtoecl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iftsjotk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2dywycyxl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yazkdvbz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kunzvzsh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2yiljbdaj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2bnximbna.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2behowidh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zhbdzaxf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zrhvqmok.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wafjkbhu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qdmikkzr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2glvrdgfq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jjwxgtyp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mvropcgh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2fwqhckoc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2buftpnbv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ypdwnsex.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tobowryr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2kavgnunl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sifjewgc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lptdabph.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uuqbyaul.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2mpgomlne.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2dlivoukh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ilpujyic.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2niefnekv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2qnpnkygr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2itsondcp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2roqsidhe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rrrsquci.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jfrmhhfi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2cvsofmtj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dmnxdytl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gordhceb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2vylqskuw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2medhciyo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2khuwmulf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ywxcqycd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2iejcaelg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2adlwefoi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2kkscrihj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvbesidb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oheugltn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsnojtxa.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2myhnudfb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ihiudwwu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2xsdakyqz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wgmadfgj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ckvlobhi.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2veembtis.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2veuiflzv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2dwstatbc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wrmcqmyd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ftturgfo.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhcyvgtl.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2enzmmuqp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2nnkjgolj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2xmawjrdh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fyctrzev.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2dwgouacl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2azvycnum.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2soidecec.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fmwmbifc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kpyrkrzr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2znxjlgko.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nhlsxwus.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2yeciltpr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2cechrdue.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2leyokgee.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2zoknmzwy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jcvhmyif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywzscjmd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pzaowayb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrcdvwsq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bnadkxfa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eivkshin.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pylgyrcm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2adezdwdg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2grellhai.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yisrbvfl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2qugyuxtz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2qqbsmmnk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jgzvzwpi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cjmnllgj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tabhobxd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dotujutr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2btkrgcyu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pymykxbm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kmnwdhso.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vtepqlvz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2xpkzoxrx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2qrshtiyu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2srhywwwl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2aijqttry.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2vzltkxmy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2mefbocww.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2mudmsjiu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sagscjbj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vlaziycd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qwkgaslr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2svqbrbqq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tngsbpwr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qehdavmi.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2skiclahv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2smcpbkpc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fdpswkqt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2kxnhadwl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2uhivikyb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kpzhhqsh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2fddhdafv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2turfpuxm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2sibtyenu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jjnaolfz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2praodgaj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yqzkxwoy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2slukeebu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2qytydrat.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2vtiwugui.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2emrneenl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2pentskxw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2gzvietng.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yowqglrk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2adcahavx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dbjhdbvp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2uyjuohii.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vsxxdtdi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2shyivkbp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ephqbjuu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2adtxojku.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2pjclvfxl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qoumvaef.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2nbhbkqbj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ijgbzdew.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2vgoznxje.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uxiwsyki.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mvpdiapx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2isidaxhu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zxunsfzz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bxkzljer.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wbkplhnz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ezhfvdeu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wicyltjy.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2vofqnsyc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kwhkumva.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2zmxpowgv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2znpnvbnp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xupwqppv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2dvwuxxov.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gpdximdy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2fofbqipm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wuszuzhp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vggdhius.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2kzcymqpm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2zknpyvbd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sqradfbx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xnsxitah.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2auoujwyr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yfqxpibt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dntscham.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2avptlyld.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2opvmlylk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmtnzlck.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mfccdpcw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2bjdkapfc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2labjvnev.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2aphasdfh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2zgkvjvxn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ejlespxi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2cywsoosa.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2zkiqatjd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2pjihvfuh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2maiucvil.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lqqmyghy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2eefhmbov.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2tbfgaqmp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2haniqovl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qhhtxhlt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2lgklpudf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ggtqhzdb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ynwzryjv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ebablakt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ozudxubg.html


<!-- 参考信息 -->