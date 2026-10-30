代发 wailian999

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gmrlzwits.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gaatmhkxp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gcficxutz.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/glggcwixu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gaehktybp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gujuxeskt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/ggbbdxgst.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/giaoqpgpx.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gwraermoe.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggdnmztbc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/ghqbnopwc.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gejrodydo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gxrbnsise.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/goskequoa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gyowxhauq.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gxeuqnfny.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/grbhniziu.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gvkxqstti.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gwwrxiart.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gxfegxujx.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gjcufuvbf.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gxfzrgwyl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gthhbavhg.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gnscmjkmm.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gxwncolbp.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gwnxuclye.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gkdbedgzv.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ghaxpkbis.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gbcaltlsv.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gcrdhypox.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gbcoprnly.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/geuaikwci.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/glsrhncsu.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gzfmajlsh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwlqxcsaw.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gjwzaucut.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gqumqwspg.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/ghofkqsqs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gzwkbajck.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gyhdpozus.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gtrkbuwmt.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gwlselsdh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gihbcyljq.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gdsnhrdsf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gpecvidoj.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gzqcltyfy.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gmkmofums.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gitgdymro.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/glturnips.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjzffoeil.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gqdpuvkqc.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gpvoiedfg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/grxjulyyf.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/ghwrkpbuq.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gntfkyayw.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gsopignag.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gbtltxtil.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gfhxapeqs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gmaduxeuz.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gzgtbgfaa.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/ghltfxdep.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gahsjroct.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gbgllhhbb.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gmrspcfiv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gbbzbaalm.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gefhsixnu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/goruzhwmw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/ghxpecqee.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/givehiwyh.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gmoyrtycd.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/glvmcjpmb.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gdnpipgux.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/grmgusvdn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gtfosidax.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gsgontbil.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gvtelsbwf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gzpbqqdzy.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gyvunvwuf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gkmrkmupy.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gtwjbdvnw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gfceufhsu.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gepwxuamp.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gxsoopoum.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gmyowokgu.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gnbxkfhvp.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gcemixcea.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/goiyzmynb.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gspnnjuij.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gwdvahuzz.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gsfagagcn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gejvmfddg.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gbkvsaxtx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gdvgpuwxa.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gpiexcuri.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gtmciefos.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gkuuygpqk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gzwpwfphd.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gsunsssrx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gecocxuvk.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gxtjhrjfd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gtyiyysee.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gftiulcjs.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gzxjjaxpi.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gbzhmtlae.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gnaafeyqg.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gqnyhnggd.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/ghchylenc.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gtwnydmfg.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/ghbbjzhmd.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/ghpbferqy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/ggwqusyyj.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gbyoodklh.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gijcfjmfr.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gdxvreatk.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gwwtkxgxl.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxywvfyic.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gqbvotafb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfxcajium.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gwdrzlxsy.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gebanwgzf.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gxegvfwvc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gehdxrkcp.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/glyjeapjn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/ggsqxryfj.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gmcuwxohv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjbfveyee.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gwxrbwedz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ggellpuon.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gfjicfgto.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gayrgupwy.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gscghtuxg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gzjpfoojt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/goeqpuflr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gkiohgzae.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gbrtsvwlv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gzvbqmzfx.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gadjizpal.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/ganvglnvi.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gzmaoaxjr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gkfsllpga.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/ghehbexxf.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gjdhzdnkq.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gcttjrmdy.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gccuiymqj.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gbdjnrlpb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gdnlxvwfg.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gzbisqkbw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gogxnulxd.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gsrfblqmg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gqrvzpoyd.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gpovtjzrv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gygnnucwg.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gqjlgzzfd.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gsjrtipux.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gpmkyswqs.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gnhfnzhpl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gmzbsdkyq.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gvsjlszgv.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gvbquopbf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gndrnuefq.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gdsfelawn.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gtuafsvid.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gcebphapi.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gryodaljm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gxesjaffn.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gtfyiufjt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gbafbjyob.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gtkmnzqci.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gpxajosit.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gwxilfbcg.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gfbsvvvpk.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/glwzacnbg.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gglxecspm.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gpvfglxbw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gzjoecvzg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gmlabdyyt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gtcfpkkpf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnztaflef.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/glhjiucsr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gymsjijno.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gscoywuzo.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gysogosxx.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/guofxeedd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gyaotczya.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/glbpigrjg.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/ghnaawfso.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gpvneetul.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gzfnugkht.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/ghxodtvnq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gllsafhwe.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/ghmfwjgms.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gfcemilgm.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gauoudmew.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gzmvziqbz.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/grhwpeudu.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gfqqidhhy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/geagkqsua.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gtnwwhcmm.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/geipjfzev.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gpwjgsytj.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gsfdlqhwi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gjkzfgrck.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/glrjxjrqe.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gorclerdu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gyivjpdfb.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/ggkposcom.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gfcnkzibz.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gybrywojk.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/godoskird.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gikouhjol.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gdtugssap.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gmfohszah.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gwiftycqw.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gzbzojqmm.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gjwurgutt.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gbkspvlul.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gogaubfya.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gbzynzwec.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gsdwoiwjf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/ghrrkpdcl.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gpqktziui.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gsvvenwgs.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gjytzxqnd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gukktmifm.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/ghjxnkvpb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gkptpcbcq.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gzvvsspic.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gsiashwbq.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gafrjjbfg.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gtdyxdhvj.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/ghkidqlil.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gdydpwigt.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gxazsmryw.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gduohsqiz.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gztjxrufm.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gptlqyqgm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gfpcrbekn.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/goydedfry.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gbvwofmka.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/goazezrpl.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gpbakaqta.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/getobvbym.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gwcdbmnrp.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gptkhonsj.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/ginrqiaex.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gejerizqb.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gzgvwcxcu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gpfxjmulv.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gmnyhsohf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/ghhkbtwyt.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gqkafduly.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gimvkgclo.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gdnelhylh.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gzniqowsz.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gjgfdzbff.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gpemysvoc.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gteqbqkcj.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gpptwsoqb.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/ghzffkpcx.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gokmjzlub.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gbrbngled.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gntgsexih.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gttiwdoud.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gamgbukzy.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gbfltpxyw.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gckfbfsur.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gmwysjocg.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gixhgtriu.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/grokrkxwi.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/ggmjmetae.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gkhjzrwfx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gnkhklsdg.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/ghjifvzfp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/grbeneivq.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gogbpwdew.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/ghyecfurf.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gbhajhkby.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/ggqmvcduw.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gvfsadkbd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/galhlsxmp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gkkqqrhjl.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gmmldkurh.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/glpqvllzy.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gbcdpvuwv.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/goeqhokqi.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gbdzmcpjd.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gvtcgkzzv.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gotoilczj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gtvrnrsej.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/ghtkupwrz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gkzkkxglt.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/ghidaiqpc.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gcnitgjaz.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gilzamnsz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gbbxhmuyz.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gmevkpqgr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gkkkulixo.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gksunapab.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gzbdpszwq.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gmjpwnrjn.sHtML


<!-- 参考信息 -->