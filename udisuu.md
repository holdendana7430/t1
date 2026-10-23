代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ccvuemdk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bguacqlr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ajhrmuzw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ssyxewfg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3mgrhbxdj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3bordrksy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tgzpxaob.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3yrfcurry.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3clqrqqug.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3dmjwwxpi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bywkcplg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3tkiownuj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3mgdvkbkv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nxysuvgj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tqxophzy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3rixscnwk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3sujqekax.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tjaecbgz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3dbjedudr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vuctcmnl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3snzxasgc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3dyoybrnx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xcoyzmkr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uyamryex.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3zasjtylm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kxamuvzw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3dkyzyxyn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3yezkoxwh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ujjmcxwr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3mxixvkyy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ccoihbgd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3orclepar.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ccvggnzr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3uixglfpg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kjrxsgkg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3uxeqvofq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ivwjhnlr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mnixbjwu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3rsalzlmx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3yqbdwuyd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kbergjlu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3iavxckax.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3skwlcfwq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3pjyjmojs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rocffzwt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3leomdckr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tmzkzamx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sdyktenu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tllfehxl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3hjorzeba.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3miwgmxbz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3rokjsjqh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3thkifjfn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rtohuopk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bxjmypuk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3lomhdiwu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3riayffli.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3egfywicf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ncrutddm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3uyckfhok.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3evaznsnl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3cboocezv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3puavnlpu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jugtltfx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3sublsgfd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3hihpdfwl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3wceppmmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fygcmppg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3phhbclgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kntitjmz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3meubunmg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3hduwdrjp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fyjsirvu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ujvkwrcc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3suhmdsyb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ibzzyfhh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3njahobvf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3sgioqxou.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ihlqmvrq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3svsvahqz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gbiwrzqg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wtayrlbk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3wbziwdxh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3tnhnwutk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3wymmlkkc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3qjptabms.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3isgxmcwp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ypriszsd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3vukmqvye.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3veeszgpq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ktonrapv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rbvttnwp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3dtdfrlyo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zjrclyrs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ebtotzsr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ymqceath.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ozrkpqdt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3egdxzmml.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3krsoorzy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rxgodnmn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3behmgmbe.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3aqgidesk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bfowxbrt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3kumranpg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ocwbcsmt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xqkrpvyp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ehtmmcgl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bvqfhxfx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3hwouniao.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qwmwcacq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ilcoqznu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3icpwmxai.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3snjhmfft.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hchgjmws.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wiscdlaw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pytzhbcu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3pfptcexx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3qrxmuvis.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uymdlsth.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lzhgkavw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vndoxyew.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3oswspasa.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3deatezzb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zcuzphpz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hmhvjvvi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3rhzvyfed.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oeippwzt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3bamzxbdm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kzvyhnxu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3eiekhqac.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qgzqcikb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hoqqzvgi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3jdorzntz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rpijxegf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3hxnqgwyv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3koyjmfjl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3yooznqkm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3exckfqeg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xhxxrvmy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kjjxwfpq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3cqciqpos.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3gaxdkilv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3hnksopfb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3faxnargp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rskujfyb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3svxsvltf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3owrfxnwb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3znstxteo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3isvhxeho.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3tzdmyunw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3tihijagn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3egafmpkn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3fcehinby.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ixvywcvu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ctitpxtm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3fagakwnr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jyuzhfmd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3woojyqac.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3kryyjaps.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xrdbddmp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zzyjkviq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3avjcaanr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3mqgmmsdy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3oldfckwu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3thvksdxk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3vxnrckbu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3pcxhckao.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3yitphoac.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xzhjpawe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqptjxex.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lqmtuwyv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3eeufwkrz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3htfheuif.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dsuhoevb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3myaapoth.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lqbpvjpr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nlakkyrf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ioysstho.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xmyngqse.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3uckqewua.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ebrhscqk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3pguomwkp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3krgquvra.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3nafoiatu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dalqsuew.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lejbzuwn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aqeddvrp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3kdqnfugf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3gntlanga.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kzfwiqdm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ytvcukas.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3suthkxjy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3gpexkjst.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3icnnoqfy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3pvadfykn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3voxrjqid.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vujyjjiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpqebpzd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3lmevcaqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dydtbqur.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rritvqpl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3amxfikda.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pxgazvjl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3kkygdmqk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3fjsjifdw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qlrafnss.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xxstrcax.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3tnkpajjw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3kbyrgibs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3luxniwje.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lumblean.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3psficpuh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3inkdqdwz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yvxfwngl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ngouqnki.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wytqorou.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mihemxky.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3zkkfquvo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3igbapkny.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3vdbvohov.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ehfstanq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hvvthcwe.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jtdsxysv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eajxbhlt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tzjabwrv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3hgyoubgm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uwuczwwz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3otjxwrae.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3xggoxtnp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3mdxzfwro.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dlywppoj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mteebdlu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3otzihaaq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ppccdcet.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3btvgzmfk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qlubgndz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3klshhtty.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xlgkftip.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zuppmyym.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qqtneahy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nbxhfcwa.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3txqdengj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fqhduihn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hqmkrtrd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3eujpygro.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vsxdcpwb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3lpspohkl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yiyzjezm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ucmuutju.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3xfxuykdt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3axarkhgg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3lyszzcnt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ksmukhms.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3evdqsmne.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3cdfbdohu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jxarffsa.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3veemgefe.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zxapzvin.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3blqdpnkz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ifffawfp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vfiwdwhe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3anzqxicf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vqvbzymy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pdgyxogh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wjkkslgo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3sqmetfwi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ksvtppdd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3arjcutba.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3adaffyhi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rqkjgxuw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3yvbfopfg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xndyrhly.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uxfqpbzv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jscdbenn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pfqxevjs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vfkhlndy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pkivbxqk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3bjcceluh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vmhmcdoh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rjqjoqqu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3envqjumq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rizwqcfy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jvchptae.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3nrhyqjqz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ugltgvgl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3irjsdxqt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kalfwmmb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3zayrrghw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jzwrvvjw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkdmfcrb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3klignepy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3dkihaxfw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3pvpwvtdz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3okvzirho.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tmapmoqb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3hhzhhwrj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ntjkwqww.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bbgjgawv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rhsegyeh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3dybtcncs.html


<!-- 参考信息 -->