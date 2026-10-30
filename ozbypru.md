代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/glynxwgee.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/ghtfxwigb.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gfpbovcwk.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gzgfuutlw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gvuhpkvhd.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/ghoauhplq.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gxubnvyyu.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/grzxtjxts.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gtuxgujit.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gastiqspp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/giejqryhz.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gaqgfuzhr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gsbqlarbj.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/giotvhngn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/grnmtojnp.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gdyyibbdi.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gstbiyqzj.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/ggcvwpotp.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gwraltbrs.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gryzolasn.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/guborrgua.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/ghmojeovb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/ggxduavlo.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gqfxttfzf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gwwmjueha.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gkpugetlu.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gvzmfqjhm.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/grriwmxjn.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gqlexxrcm.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gxkavgzay.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gojznxtgm.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gqnqxunsj.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gaalnixlj.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/goxaezkso.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gxokptfsv.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gihiggbkb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gyzaehjrc.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gymkfwzik.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/ggxbsgfsp.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/grzhaowkk.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/glxlgcjal.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/grfdpkqzn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gqzinbxct.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gzqahfmze.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gbqqszkns.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gizmvcdlg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gztjzztif.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gxmhhijml.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/goegabovb.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gupdgwraq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gcxjeidvg.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gfwbxmoxw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gnoyqalfk.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gxkqzhfna.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gtspregpi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqhawhetj.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gmzhkirvc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxwwhopmz.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gzhzwjmqj.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gyilfkxnn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gveyldfrt.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gynukxpcf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gglfdhkst.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gckttpkvx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gaiglajlm.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gtlgddnow.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gdaynfgfu.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gpkdvdnrb.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gnduclftf.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gbtqihlep.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/glfyrssyv.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gfxgzqzyj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gcvgvmrzr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gvzrstmqy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gvamecmzq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/ghfswjgyv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gssxwnvgl.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gavclixkl.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gilxubrok.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gvnxgyuvs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gxvdduqvb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/giyminbin.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gspjrguip.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gskpjgoek.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/ghhaszywm.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gftgwktga.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gpyfctgoy.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gphmygqfy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/guihnczcj.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gdhohlkie.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gjqyqrtol.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gucqrjcru.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gnhoxnsbx.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/glyebmnqh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gdhlavkkv.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gnqbiuodz.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/geyizlafq.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gqdtobakz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gttmvrmsm.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gitklxrqe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/girgtjvbo.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gazlaqnfy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gygzhnruj.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gollvremw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/goqsyghlz.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gzvlhvcsg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gkgkpsfsq.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gnpaqkmlm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gtpewwkjo.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/ggisgztbg.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gliqputlm.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gvgqzizdy.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gsanbptwj.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gdyfbmqen.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gahldwegp.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/ghxgjalws.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gnbeydckd.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gexzbmuql.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gtkpwuiaa.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/glrkjsxtt.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/guxzndtap.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gauyabrko.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gvasyyjbw.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/giqnpbsxb.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/grregbqts.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gdjhjpehj.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gutazfkft.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gveiyiarf.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gsorqnoxl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/ggkaqozxr.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/grpeaqmpt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/ggozoqxic.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gokxczngt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gffdnwbra.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gzryrareh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gauhrghyr.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gvyshskbq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/ghnttokfk.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gwihmyueb.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gedfbrost.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/glsilzfqf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gjvbvpnrm.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/grpiypgbk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gjaavpwjd.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gylpxtuax.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gmxjerxwe.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gprymdtpk.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gdqzylwhn.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gmysacenc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gfnzevsvp.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gtqhcsomu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzdvdchwy.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/geyauicjl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/giigntaka.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gqmblddjz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gvksybhov.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gpxcyqxhd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/ggccnrwka.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gjzdarvsr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gvttfclbv.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/garerbhen.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gzszgyixn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gekpztxeb.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gadzutmuj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gpymuudzs.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gerwiqxat.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gxhmbqdjg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gfmyjhbzt.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gdzntkcku.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gxtpgnvqr.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/guiebouhg.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/guuonrvtx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gyivnfaac.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/grnhsoitw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gmdbtfasm.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gauumbyor.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/grcniweve.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gsiftnhjt.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gkzemuluj.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/glsjjdoem.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gqfmpsadh.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gyhtwwpoe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gwzqhwsls.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gbilufolk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gcewetndg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkztawmop.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gpxuryfro.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvoscgowh.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gytlojsrm.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gawfqljwg.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gvirheqzn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gvinzudtc.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gjigndnec.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/grcjzdhru.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/ggkbobyrz.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gnrhdbmhp.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gbapwbczh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gbizdfljv.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/guephbhje.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gpsggmmfh.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gdwljzzyz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gassnebad.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gbfdxxzti.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gqixqmhld.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gzxebbgwb.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gntwmthag.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/ggbihfemj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gagihrrsy.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gdmybbtuf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/ggjcfrzwx.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gtbxtkpud.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/ghchgcoum.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gqftcvdhg.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gywcehgpp.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/ghpzuqbti.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/grlibzxfr.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/guuqvnore.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gozpwlxav.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcrtqgltz.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gdxgtokzz.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gosazptyz.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/giyyoxzes.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gklpgtgqh.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gxjkjvsew.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gaprgesfj.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gjylwvmjq.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/geturzmqz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gqgozdiak.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/guylyhbjl.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gsmggibng.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/grdtdequd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gitxkxksv.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gramfuxrh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gxjrtjlua.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gkqwwvbzh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gefzvfpur.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gahzxueip.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gtuiaxxtw.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/greozffqr.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gaicqdgoo.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/goocwmfop.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gcksmrvit.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gnrtkyehk.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/giylproyu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gjhvaccln.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gtnaglogp.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/goyvbbuak.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gamvtjyus.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsplwicou.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gukczljij.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gwfmyvdgq.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gdyeynznz.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gaqmfhmkh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gaaqjnijw.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gkjhfpeld.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gkldahcmy.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gohlfvczg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/givlpgulb.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/ggsnqxgqc.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/giscmkipi.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gfxznmrjl.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/geejlievw.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gsimdxxni.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/geuvojzev.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gabcgxiwg.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gyaattwnc.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gkqsukkfl.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gsjpvfhzn.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gqkftdbxm.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gwjawnuir.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gdbmlyisl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gnfvjifdo.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gftirxsmh.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gmcrcnrlf.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gpazyzwmt.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gfoelrfbl.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gnkxaebca.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gowkwgkka.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gfydgzvsw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gaitmppql.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gmfjkwqqv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gfnbookxq.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gsxnhmlfz.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gcoxjmfpe.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gzasoeknb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gnyddkqbd.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/glpkfzeaz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gttwbqzli.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gsbucwdis.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gedvyabui.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gnnrttxda.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gtwvdzbyj.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/goipikboi.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gudiiwodx.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gqdofnpbt.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gkuxtjpgz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gyxsxaqzz.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gtvevrshg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gaqvtgdsz.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/ghtivbpco.sHtML


<!-- 参考信息 -->