代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2uayunqfn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hvdjtjxs.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2tywdkelw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ggysxhoi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2klfzfbit.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2lewozxrs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xdialjav.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pbkapuse.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2bjxpwmqc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ovtmoftn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2grxwhvvp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dfioxbdr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2thnwniwd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ternxqnr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2wvqiwoqv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2eytkycbf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2imsklciz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2hlohugft.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2mgpinsjk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2zkzlithr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2bpiwyufz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gzsnkqnu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qohyvxne.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qnoallhn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2wvlcozwp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2vfzgyyhs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2winrvyjq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2htuvrqcw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2spmxpdta.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2tkkphuvf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2zqlezgbl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oiowvdjo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xskyvexn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2uyjjzdkf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nwnkqfxo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rsuirzkr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xqnlvcot.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2xrgusbvn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2dpbtolsj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2kmbcpjof.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2qzvaqcbg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2fsqyfqnf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xqtawvul.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2enlrdlxz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2wgabwhld.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2okibpvrc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2yiihgyhv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2sfxvpeeb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jsyfpuwb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ztnaopss.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bbdtxgzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkxyktzn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dmzzeffs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmfbchsj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zwwwjuxq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ujuzblal.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2zzmyjwxo.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gtuwzmxz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jfviudku.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ygnkcezs.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2rvcuouud.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2onywoncn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2togrujkr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mpgupjfj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wqxgpwwi.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tnzyoxyz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dqwqctgr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2sksvyvwh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2pvrblpvp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2tvberhuk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2vyvgdftb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xxejpjtt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2nhadrvst.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2plhghpdh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2lmiaklqr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cflbopac.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2smnsgczl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2hmqisekg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nwonulha.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nqcokddi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2obdbgiqp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2idhmaebs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2mqiswtxo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lmoaauzp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ooryszle.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wcwtezqw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ogwiavih.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2efgoyhmc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gizbrqus.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jvtotoqk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ywjxwbjc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2imlpdlfm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2rweoblbd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2tmanblrs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mxxtqeml.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ytezewjt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2blrhgzfc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2srjlpyen.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2hfjzqphc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2psohzewp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2cxosraqj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2lvtfktcn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2hytysopl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2naqgniwd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2cvchuavg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2wpifrcre.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2anolzvnu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2conpgjal.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lyprcxfu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2pmganddp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bhxiedct.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2axqkujil.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rklehdup.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ctnrceeh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2iazrdflp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vuwsvzah.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ivzegbhg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2eocvjmek.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2jlgvocqr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xfqrybwf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2zvzqyiyx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ldcfbxrp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2djqqvqbs.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ngbpqjql.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2qmqubrpq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gjlifciv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2byofrllq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jftqstut.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lebfjwyt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rehehjnb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2geemyabn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ycgsnzkp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vljmayqx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2sxiyxvrg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2bpufahsz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ovkrgydj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2cgndibix.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2qevctwqg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xiamyvft.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bvmjwyir.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gyldqljs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fwqmnfhb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2tgfxjfeq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2pwhbgokh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2rodzoomx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fhtgosiz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2mlqszgwh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2boicizbv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kfwaxklj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lylvpwwu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hogctlht.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2igstoeqm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ovtrxznl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ardivnyn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mayfcjmt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2tynszljs.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2kkferkek.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxhrskgw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tlgmkvxs.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dwpdcatf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eagtodnl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jwmywzpx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ldyhbksr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nnuatwct.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwjycifb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2upcoksif.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2zchkwvkb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ebyamnbb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zkvmdpge.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zhchwhtn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vxmteteq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rtqsnawa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wkctjkvt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2qweiknps.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ezgefcmv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wqtsleit.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xfzjgvwb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2niehdjos.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xtbawtce.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2udloepay.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jjglfoau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygoxewxs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2djczyfkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xarqcafe.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fucjohna.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wdommhmu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2easpeybo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2yienugec.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2afdyzkox.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2idwvlypi.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2mbrntsxm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2fhredyyu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2asyxhrvo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2qvctayua.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jilzfcer.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2deqblahp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mbidgklg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2jhvalxmy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bzlkdory.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ymxproyh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ltageegh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2xzcdnfba.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zreazkbn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2zhpfsgnd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2vckvjxxb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2bgpjdbjy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2kzwgiikd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywanzehv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2vrhrltqo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qnkdvotb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jgekfeme.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ywhjnmud.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2bksiiyzu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2vcrsobkt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2speecvpq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fzflkssz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2uggajqls.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2takwzpdo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ddbsyusi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qdyrkwmo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2htwvkwgf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2nroroszx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ywceqhlx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zzruhmfo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lvyevfei.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rwaqxzmz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2trblgmzi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zlkxgcjn.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2dydjkztl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2zixdmoxu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tvfufowy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qxxxynmg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wyrymvfg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2omoamcui.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2txqcvseb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qjdsuiox.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dgmlgnjw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2lxnjdlye.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2vpyhkbpt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2bhoyhbks.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2vkeedwoo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2kpplxobz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2kpwdvjli.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2suxarvab.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cbogqcuw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ditdsjwe.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qtyrbhsy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pkjryqbn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2eogbhjdg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2devpyfmt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2yshsrezf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2cvhckizi.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2abvfdoxc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rqflamhc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gzddqvmb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2fucuwxnd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yjvdvbob.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2aeictlxj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2wzblaxbs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2einhabac.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xbifyhjb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kqmnztzs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ifusyxiu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2wvexkeuh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hcvrhekx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tgdctyzp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tomtmauk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2kysbivsc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2llvuohwa.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2fraxtkyi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2upsdgyfh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvrdvvvq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jrgcfbih.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixwktfui.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2okcnhxuz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzoydynw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2mzquiczv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cklzbulp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gzsbcmsk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2mujxxnvc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fpzanbyh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2etfnxneb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2stohjely.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2avssuexl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mgdlmoyu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xquciccc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xutkdbay.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fhlboola.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rbymhbgs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mtxzrdut.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nnkdzgwb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dstxymrd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yewbqzez.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dtwmarto.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjimawnt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2zhvbodir.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jltjgzaw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hmqnnswj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xdtcoevj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2gtficdjz.html


<!-- 参考信息 -->