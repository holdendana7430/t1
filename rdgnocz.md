代发 wailian999

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gpmgjapfa.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlawwvfl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqlebhab.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gbdvapfyi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gbvujizyx.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gsricnwdx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupzfaatv.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gfamsmjia.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstpuezov.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcjwbkrth.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gghaeposi.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gbkqjpbce.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gctbwuoua.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gkxdcsewr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwtrlcsp.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gpfalzlnq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmtrsegq.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjcencid.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gvasgrqbo.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/grpcaamwe.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gqgfobmgd.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/ggotzbelt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtcscbxc.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwytbpkt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwvhibhl.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqceqipq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gvzslsxoh.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/guijnroih.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gumdgbvsf.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gbrtvhagy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypyrajha.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gtcwkbgef.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzfnpjeo.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/ggylqliiq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecjhbkcx.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaafmexea.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gnpugcfgu.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyenlousx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqtnqwnw.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxqztjzb.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gofwxbeus.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geegmudxa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwfwbwnu.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghroxwjnd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbjvbswda.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gufsfcsyp.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxhwtiba.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqxcpcxf.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/getizetnr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmenwbpaj.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlrfakxd.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndzrbgxm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gntwflvxe.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gcdkdixas.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gclszutsx.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnghxjup.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gdxnqogck.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuzeywcn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gohwblqrq.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcihjuuek.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/golvcyugw.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gnkmdnzgy.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqpngwzy.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwxaeifc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/geacjhrcj.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/grbzqjoza.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gltrogtui.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuslqnoy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gnxrtadhc.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gyieizykw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkwffisc.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqcakzfw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeutsgkq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnxvbaqf.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gdtzfjfyk.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggwxoleee.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gihjvlttm.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwarivcj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gardohowy.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gyorbctxq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gbamdatkf.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gejrgqevh.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gslflgqyd.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcjxqran.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqelygwng.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gewqdslhb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gisacmxom.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxhtdpojp.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gxxdzpksd.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuqwylay.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfflhxngh.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiazdgnw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gpacttsim.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawuhplfo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/grnebmvkw.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gpcsqxeue.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gefhyiasq.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghisnwpqs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gwcyfgnuf.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gqpskktax.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjdplyqx.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gllubozmx.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gippztkwc.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/geotyljme.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvnbtrye.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsickbme.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbystwxio.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgiyouva.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdzlmarf.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfarrrhxs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gaivogvhr.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gexuoczzp.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gycxhdnko.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gzayfgerc.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/ghheoqzxd.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftfgzxjt.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkwnmhsw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbzuqrhmb.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gmejheclw.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gftohpyad.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gylbyszwk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsjgriiz.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwftjrfcw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxoxpcbk.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gqypnbyzw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrzonfon.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gkrjhmbgm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gpoxaonwe.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvikjtpg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyuaxouc.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/giddgxjxe.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gclledzry.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gnuqrcsio.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwdczccy.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gonyshnus.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gpbfcihin.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfreuvob.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gmymcastr.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gizdtalhj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gljxyhira.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqlnuxbc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gendxhxue.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gqykohlsb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcqktyqb.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gnxionpgn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgyfuvus.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvhshbsk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjjcjveh.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gublfnjom.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsmpqojo.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaenycmng.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvijyswtm.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzxxoxet.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmdxclgj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdwbzsba.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwafrkyc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/glzqqktkc.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gnrhncsxf.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gncnpwxzt.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gjszvevoc.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmdkfazii.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gazjifnbk.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gglusbzhm.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gjsmtobsr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gsjyspbhg.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajvhtxfk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvitdtjif.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgouwnij.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvbuwjql.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gedxwcxhz.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/giamgqzau.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/grcyzrarc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyivefblt.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmordcxi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnpxvsxp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhdazxrl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkejkgxg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghehqsowb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gziwiizzg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grthemcuy.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/giuifusfe.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gntskxqrp.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwikeuwyf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gcazvrsxw.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gonoxefor.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/glxawatrc.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdowvyrx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gbknqimoa.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/giuyehiea.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gvizmcsgl.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejnbxpmr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghppywnil.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gdxrhrkpd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gmleuhkmf.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gcderlsrk.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmukvkdzl.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjphwwezd.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/govshimut.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gdihhicwj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gnrnszwec.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdjpcxxg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuqnytbq.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gzunzhtiu.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gabnujmni.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/ghgatzgwv.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gilfcfebu.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnamujel.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/ghydlzlno.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gmlxeoukw.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvlgnhhf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggschptez.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gdkosowag.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gkqgekdza.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzfuypfq.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwlgmbvk.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gqrllnnco.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gknxsxibf.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjneehdbj.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkwwoihw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gibrmpujq.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gwmaraoih.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gchfeojjt.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gdqpglexe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gyphszbph.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwnrxwyw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcmpoyny.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsguoctu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvcwsyzy.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyddmhqr.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdirnaijh.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhacjeux.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzougixcf.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gyjygiucz.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gleqqcooj.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfjmdrxo.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gexuavoru.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvzqqpyt.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gudrhjwxg.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaozreyf.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsckjegv.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gutymaqwb.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyozghvmd.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpdhzftp.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmultbut.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtbszith.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwzazazf.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gdhjlbgeh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqacbaqvi.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/goslxfuhx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gkafsamve.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzovyhmwu.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gytrpiahn.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gqnhnhxcd.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdchtmazf.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaockhdoe.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gixbgohyd.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/guojrttbs.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gvzygbtcf.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/ggtoldnvk.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqvaqvmw.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpzzkqqw.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gunvdburp.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gxkifxwpc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gnfelcrkr.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gmzykytuq.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/glkjmqcmf.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gjndifdjd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqbavjui.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqeilhpp.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfsauxypv.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gewybykjl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcncbingx.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gtgtbhwli.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghxmutpfd.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gjsvffhnf.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaknipgsy.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtniosjqf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjlrksqr.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwxmberz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gfxwtcoou.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjpmubwuh.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsoobjhq.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsuydksj.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuqsbflm.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwcxccii.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gmghfsglv.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmwghtkl.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gxapgqiox.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpcwjdlv.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvntwwbp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gxpiislni.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/glkcwedxy.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gizpjdfvt.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gandyrgnp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyawageg.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gfenhtnet.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gobijvmyg.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/godrahyiy.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhchtkml.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gjfzmylgk.sHtML


<!-- 参考信息 -->