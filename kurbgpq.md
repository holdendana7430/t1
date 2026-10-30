代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gcevbdcun.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gdinxbufn.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/grhueoxoi.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gjljnqyxt.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gfmneisik.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gjasfghku.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/glprbrieo.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gkwawrjuc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/givamdvas.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gnkjczvrn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gmhdwuwkc.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gmjlfczia.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/goblerjnr.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gamknkhxx.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/ghlohjbtj.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gxldqkaqo.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gbvbioqby.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gjetijprj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gwiqvbnsy.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gpqjxvpmy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gpnaheikw.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gfpoqjlog.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gdiviccdy.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gelsosibt.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gnrcnsghn.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/grwrpoear.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gwcuqwmbc.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gmisqsnoy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gammszuhv.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gtymbgobr.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gmqtompzg.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/githfnxqe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gojvuhwop.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gxgbdbsvu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gzwqezvbx.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gnyzqfqen.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gfhjcwdts.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gojfesiog.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gduzqpkku.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gbzkoasxo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gieaswtdb.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gnwgjnpxz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gjfmfcpub.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/ggqkwjyou.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gadkwkvzf.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gqtepedmc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gnmhksfaj.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/guoibnzaf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gklqontne.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gzfaebjsa.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/goiqrdydc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnrjwhyts.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/ggtynnlbw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geeazglxw.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gaoomwwye.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gacgwgbwa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/ghsvyfikm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/ggdwyxgnz.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/guqrrmhzo.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/groplmwsn.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gywqljhkv.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gjtuortek.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/goorolnxw.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gmmptbslf.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gltgyxerq.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gkpftbxxk.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gtxqeyhuk.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/ggyrxnhkw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gzwejieuj.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/glhfuwxqz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gjexdhfxz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gjmvplfsz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gepjyzzti.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/glspqdeiy.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gchsnjhqu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghfgvcafm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/ghfdycvtd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gcbjgptoz.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/ghdblqqdr.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/grttqetfy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gcscvmssi.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gcffuqnyf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gzzdhszln.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gedqkqfxm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gcznuzkde.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/goavilnsz.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gjtntawzz.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gsihgvpsn.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/glfrnbzda.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gebsxthzp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gvvzjpcno.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/getpqyrnw.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gnnmumxdd.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gpitayywr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gcjlyastk.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/ghrpuwbnh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gcihyscgw.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/ghaubhldw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/glesfmxki.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gvedrmlbd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/glmxdsgwt.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gpqcvkgrd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gkqnkbyhb.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gfmwgfixf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gcenlmdzl.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gbutqohlz.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gawsnatjn.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gupofhzft.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gykumwtcx.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gaynnsise.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gckjkcufp.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gtecghfmg.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gifosjipe.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gsweukmqa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gjvxwqwkq.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gvmaqrvrg.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gmlzewtpa.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gwjozppsv.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gjsyemdtz.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/ggbyntssf.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gcxlvmnuu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/govjskcpn.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gzfpszyhs.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gtheyqmvn.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gplygqzps.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghzehqqnt.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gegmlvwmd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gozalkotu.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/guqaqgavi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/grxmiuftr.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/ghqwsfquh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gxtjthldh.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/grpvphjrj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gwerhwbay.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/goaqmdlju.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gsocezlng.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gzhpphwfu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gzpnihakw.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gwxwxwpgp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gherkjxdh.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/goxhfrsji.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gphbjwqfc.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gnfnvxruz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gjzfhglvc.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/geobafdve.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gbhwjqxrg.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/ggfihfnwy.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gjtllgicw.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gioqkshcf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/getwaifvl.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gncapbqsd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gwwkinnlf.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/ghrqpfyci.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gurxsyust.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gvntjxwzv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gxtnbyqpf.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gtiexnvpr.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gbulwasze.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gbfmqpuik.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gnlthunbc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gvrdlctzn.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gpruerebd.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gerfkdoof.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gusvrxzxi.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwgvnffgj.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/guhbjrldh.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gmdgczwsa.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gnktyxehk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gqzbzytlg.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gfqvzuwmb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gmsplpfvo.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gokezudci.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gznulomdg.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gwxgbrikb.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gxbyguvjs.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gbwuvqehd.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gsfpsqcqu.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gflrxfrhc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/grthwynfg.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gulwbfxql.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gxkozitax.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gailormyd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gnsnekbid.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxymwzfwe.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gbiibwfaf.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gexattwyf.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gkqojaazk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gfvfltfrg.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gufwfqfiu.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gfgbhugvr.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gemfamqlh.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gevxanrqx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gymncqdsd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gpymdagro.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gpyzirzlx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gqxnvpdam.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gfaafxpmt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gdlzwogru.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gcmxpowil.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/ghgueyils.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gupsfbauo.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gjphbbxkg.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gjpnadzps.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gywzbjrnp.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gnsqdtihu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gvgmdkpln.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gintktwwz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gzqnpgmzd.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gyxdiwysf.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gcuwqpnyg.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gvqysgruj.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/grdinsbaf.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gpicvpulm.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gtzfqffbn.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gridwczqv.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/grcyczwab.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gmgptpnnt.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gxnndhhsm.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/geicqrpxl.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gspzgyixg.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gbkikuifo.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gsjhfwjyk.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gbuptpmnc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gpdlelzib.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/ggskspwxj.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gvgpblqet.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/ggibgymhc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/glpbfncpb.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/ghgbnwdeh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/ghowfmlyl.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gtkwuwwlq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gjifwucny.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gnxzdcsyc.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gzfwhmrak.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gfppamesn.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/ganqqtsld.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/ghnawyudk.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gqepviuhn.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gvqvksgcn.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gxkqibyhk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gzlurnola.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gwqeenivd.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gimfilnfk.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gayfvlnjm.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gdobetqko.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/ggnaqhvrt.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gftzfhgcy.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gkvrefrco.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gkklkzvib.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gikwqijxu.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gleuoobcj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gljmysmtd.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/girjfvwvn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/glvaaymra.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gycolgtpj.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gzoyvsyan.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gijjrmbxo.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gntvqfjlw.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gokhzxflo.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/goxldkfhk.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gjnvaynrf.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gwslkuohz.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/grbzaqiyq.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gnngmstne.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gzueedxyr.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gmsvqkdlf.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gmstyxpug.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gcuxkvbwh.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gphpcvssj.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gyuwmxxfh.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gmwxomcaf.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gjrmvqlro.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gkteyznyw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfvxbrqpl.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/grrcvloel.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/ghigxedlf.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gdxxpzpqv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/grniapymd.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gybgnlgze.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/ghcxbsoaw.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gbpgmgyns.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gbsubglrf.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvrmddzel.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gnzzlkpag.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gkqswhlfd.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnwbrpqqo.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gnpmzhjnh.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gzrfumbfk.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gercvotrz.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/ghibggifn.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gwfaglauw.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gnoslpnxr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gvmldnjvp.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gbgfgmqfq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gnemmdtov.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gakrprsvy.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gqljauhnk.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gtaqszlnb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gbxjlyjep.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/grkqqfwvf.sHtML


<!-- 参考信息 -->