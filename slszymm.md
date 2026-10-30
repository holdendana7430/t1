代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gusznnqdn.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gafpgrjsk.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/ghhdplsgg.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gdhmpifel.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gfzxyzhbe.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gcjhnzeok.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/grdgxalts.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gjnoayuag.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/guqgnnkik.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gopicgmfe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gwpgxcqtf.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gognspagn.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gbkcnkrpw.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gyatjywxn.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/giosmpvba.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gzmltskns.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gdrzwfhmu.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gyzywcfuu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gpzsabowy.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gknjxcbhz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gwpdhhrlj.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gibkqnrmj.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gnfrihdva.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/guiklfewk.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gwsyhwskh.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gxclhroeg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/giagmuceu.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gpcqhecxj.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gxucwugme.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gwdsfmiru.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/ghhuwrobc.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gldpajyue.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/glcwnxagi.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gddyhdwzt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/ggheealdl.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gozdgfxpl.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gbrujsgii.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/goekjvdje.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gqmmocnaj.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gtqsditvp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gxfmqchky.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gfjolguyk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gxztnlyrg.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gtxqaufrh.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gwkfyidwe.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gadndnrbo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gsamiivcx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gvsrcjwcz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gyybuhrab.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gkecyzshf.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gzicjyvlf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gymbqyeky.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gudljeaji.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsbfeffos.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/glfpqkoap.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gyazgpdja.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/geakoeapk.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gnueoxnku.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/galrokjwp.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gjsuflofz.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gwommzale.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gcsidpafk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gnqfetdfd.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/ghcctzryh.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/guilfeajv.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gpmuhpxzs.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/givfkhucp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/guceiekhw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gpabkmurm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gjolfubsg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gljnftiti.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/ghjfoceyq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gwuncjfga.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gnvzariyy.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gsgxticcc.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gxkqmocaf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gcgtzerth.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/grstaphxo.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/ghjmijink.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/geliapwzh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gngjvjosb.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/guirlidgc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/guotnottj.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gidwhkrpu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gcgwcoyrr.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gkivtoout.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/ghzcjjdmg.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gycxapvyr.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gsklolueb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gvdapkmwn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gybfbjkmj.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/geaoeqfaf.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gcmfexugs.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gwmuecetb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gmucyrvfx.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/glphsjqfa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/glcnlvyio.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gftjygncq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gzuskrnng.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gqqoddjih.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gegdvppct.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gzvlmwrfn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gxqjxqpcv.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gzakbrcjk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gwtxgcyut.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gruousffj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gskfmyvbe.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gqoyfbcsk.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gguvpnkzd.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gmogxkfkm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gpqdbusgb.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gaddwjyyq.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/ggjbsngpe.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/goidmxmyi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gjgpfzwbr.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gcwhpgsmf.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gasszuere.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gjabufiov.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gegmyjjwr.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/girtfshlz.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gftcprohg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gcskkqjfv.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gvacxjiux.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/glvfhfjhy.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gcpdcxckq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/ggavtqtcd.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gjzswbssg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gjpkxqcyd.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gxftviryf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gtfwfaxti.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gjpuekiay.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gpzqbcbxv.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gyrkcdmsm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gbnlnzbcu.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gyngxvxor.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gemmigzld.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gmzogstqf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gjfxpsoub.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gxwanwvbb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gybrjthfn.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/grdlpuphp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gzjlwsfao.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gjxbaiekh.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gfdubnzxy.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gwhrhmwep.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gwlfwrkiq.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gfdmcxaef.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gxuqmxixu.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gbnnanpcj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/grcyctrbm.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/ghojxjmkv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqtvxrvbt.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gugzifuak.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gqdjjrvzl.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gvzmqmijs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gdjybzvuw.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/goabazimd.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gxfayktqh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gxdpqkkrp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gajambplu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ghltljrvl.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gocmqprsl.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gjqzculol.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gkuxcmmxu.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gubnziiov.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gflpsjubj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gcbyeelbf.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gieojzpyy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gzsbvinaq.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gclcbbesj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gynngdgir.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gcutfipbt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gxjzhznpa.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gnxzuaqwb.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gfrfilxhp.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gdgjkbrjf.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gdpfuxzlf.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gqvsjuusq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gkmaswwfj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gskoimtox.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gqjlhdixp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gptkezpew.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/ghwhezcra.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbybzgwoo.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gaeziwbiq.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gcdwpfsuw.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gtawxwxnk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gxitfbwfw.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gqiruydwp.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gsuyfswlk.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gxosuaomd.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gkmpxzmpv.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gsvepqqqj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gmljkhrsa.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gvhgndsfv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gkullazns.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gmphhbbtb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/guzgzlwbn.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gvddiuviv.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gzcrnsjua.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gfzsqdvjv.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/ggpaasxdz.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gwzrjtuxk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gfxmsxdoq.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gxiwideuf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gwclodndi.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gebmmdabz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gxrsrmjye.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gmwimgupb.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gwurvdahg.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/govmnxanx.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gslvgrcng.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gytkurqbb.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gxvsorprs.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gvxlahmji.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gqcueeneb.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gpvemtyru.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gpzlwouuk.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gbiguzjvg.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gvfdtlril.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/grfcewxnh.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gbvuczwmj.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gobgxwagt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gzgvsulor.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/grhbhnnkg.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gwktfqioo.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/geptzyfil.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/ghohqifuf.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gasieqkjk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/grjjhvjnm.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gcabpwztq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gwlybgrgi.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gbjtvgrpv.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gljmunabe.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gmvswtake.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gxmyxngaz.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gubhbchae.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gtlqnrhty.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gzjcqugbj.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gdoxidube.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gzuwfymng.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gkfusrggm.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gnpuslfyn.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gxjjutsoe.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gmieneqrv.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gskloiwhm.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gaonkbbfu.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gyvivjsph.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gqrqtzhch.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gnzlwvacs.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gwqaudujp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gdozltwjx.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gkyewbcvz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gdngjvnik.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gugtibiis.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/ggycledkl.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gxvbgvpdm.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gebbxjcwn.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/ghnkcvrxn.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gvipjibky.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gmxgxsqoa.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gytlorwah.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/glfpoqlea.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gqqwkpkos.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gleubwomm.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gblhhmvul.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gwiasupfl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gewfbemlo.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/guhudqmqo.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gxnbbwwto.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gcqpdjwqu.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gjfgrodlo.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gzktnoqmn.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gfwrcbacm.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/grdaiyumd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gnvkvtsfj.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gomrnbmds.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gzntbkghx.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gguahkdsj.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gllclwzno.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gsgewutlo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gpzjconyx.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gawvbxhwh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gjaxxkwkg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gdmyxyikk.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjdlnawos.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/geagzpdvj.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gdbpaxjzp.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gsqfclpna.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gefnybptj.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/glqeyeeld.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gxhcavvsf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsrzfxjhx.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gjmwmmyog.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gxetltttu.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gybbvtcjt.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gnhuaeerk.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gstoqfihi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/getyvjbgr.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gfazefqxm.sHtML


<!-- 参考信息 -->