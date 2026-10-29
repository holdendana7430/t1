代发 wailian999

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gdlowogpm.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gphpwnnnp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/glhmejjjw.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gmxuzflxy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/ggijmqzka.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gmzijasiu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gejgzlvdn.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gbsacdyab.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/grwsmcekq.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gpfuqtjkj.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gawlzhzps.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gldjurcym.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gimvqgmqg.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gbsnlkwzk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gtilylkcc.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/geueioduu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gcrggskao.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gplvzdblx.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gwbwsnpey.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gfqpzdbyt.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/ghkaiasli.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gaoajzrbh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gnrrdmpwg.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/guggomdfe.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gfaptkbej.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gisglvhrj.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gtiyjcoky.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gebrpublt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gmxiqetmd.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gemjhbxmm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gjhtanzjb.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gtxdtnola.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gdiaouabb.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gnftoknxh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/glmakmktp.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gzolnkjqd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gynhqwicr.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/guhziwltz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gajeyppbo.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gcslzqlcb.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gjlsioena.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gbdzlvbmd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/glbjprhcs.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gpodfujkr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxwrpnrbt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/ggwjeacgj.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gnwvqiijv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gumqijjhj.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gdiyqdika.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gctzvfogc.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gjzugzdgw.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/grdejyvhv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gdavuppxa.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/grcwztueu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gbphfklsv.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gsbgizixn.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/ggpybhkta.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gythehjjz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gdbmfzznt.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/giyxgtczi.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcgfofkwk.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gycccqwkg.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gutpgcyce.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gjpnmagqt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gloedsafs.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gnhthzkby.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gnmoxmeyr.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gcvbflrae.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gqdedtrlc.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/giknhklpn.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gbebkhoyy.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gyqvdwiha.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gqqlwlpri.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gvxwioxbx.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gmylgctib.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gweeaevwq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gaopewyru.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gshbdwnxy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gcmfqigmf.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gvepmwjvv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gaqhmaptn.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gshstilxp.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gmzkgsoys.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gyccgtmeo.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gfrfcolfa.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gpjczipgh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gmltslwlo.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gviplbqrm.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gmxaeuqqi.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gsarfuiye.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gobmyhptv.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gkckzeiiq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gdpbuurfp.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gvdtmmwaq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gbzngyozy.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gknaofzet.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/ghdeprrwj.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gqndbsrqq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gzulpywvv.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gugouzabh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gnlxolboo.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gawhnfnwr.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gyxgmqpdy.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gqsgodakv.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gabyrlgkn.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gbdjenwza.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gxzqfviwq.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/glkitsmzq.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gekpkivyt.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gffzmqgyk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/ggbrmpopn.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gjbsbpsod.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/goskrofkt.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gwuloungt.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/groiuifwq.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvjwmhslk.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/guzhhodea.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gvzeenxwp.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/ghkfmqjxm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/guphhvpcu.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/grlftbtpy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gpwwsyogm.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gmflnhbhh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/glpdxpsyj.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gzygbvtcu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gczwkovcw.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gfzrdvemm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gpvueunun.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/guyvdqdcy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gtohndxyw.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gkjujltzh.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gesbmvrye.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gfvnulrao.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gguneajno.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gjdjcmgjm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gefylhuih.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/giqopzbvz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/grozpntby.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/geotjsvjd.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gzkztcjsm.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gkfwydlfj.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gqiumdrhs.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gkdcexdwu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gwlxifuwt.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/goqgxmdds.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gtcixjqtv.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gdptucvex.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/grvpwjrnr.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gkvwipiqx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gkmafimkv.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gcywpvqfw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gwyyzamzx.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gwkvihbst.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gwtqbsoey.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gqxkpikdi.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gpnxtmfid.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gsyerdxhl.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/geodpkuwt.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/ggjojvgro.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gaiqkxvwu.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/grbfmmgib.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gwmugpdtb.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gkvtjqgdw.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gohpmonrl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gwyjulbln.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gmjymjjhj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/glyguxkfg.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gfvmibgpp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gxrpcxddw.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gkgbeuibu.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gankozxdw.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gcpfjlcti.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gskvugaah.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/garofqkux.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gaxmrjmqq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gdgaistzp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gwimhtxvb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsfjrcrku.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gqessgsjm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggdaktugo.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gzqmmxozn.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gogvezidn.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/giypojcws.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/grpgzqxyb.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/grgbqxtaz.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gyhsotfpj.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gcufuklny.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gwwgkmjwb.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gxhlyracn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gxpnumcsb.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gutolblim.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gvmyjtfau.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gtjqdorhc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gqoznjktz.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gsmoqdcuf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gdyggqlxl.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gupvxssxn.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gqebkcmad.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/geblhiegz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/glntxehse.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gviqorsea.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gdwtupswx.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/ganiojdzn.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/ghvxmvqow.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gtzcasqpx.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gyacwuwzp.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gecltxctz.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/ghakzdcik.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/goovsezla.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/grlggjbtx.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gpmtrmgcm.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gwrurjrfq.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gojesprii.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/glwijalcr.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gzczdaezc.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gqvezawts.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gmrmgjvem.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gqywnkjvj.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gfyodfomf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gvrpcmcqi.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/ggyhdrvdx.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/ggvjxsnpf.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gwppeyohk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gdhlfonbh.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gibaxwpoy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gynhddxko.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gldktouqj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gmdxbnxxr.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gjyqcmjhv.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gabbitric.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gfoolblnn.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/ginxsdamm.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gvbjcfbex.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gdrgceilx.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gtbicpuuq.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/grherynlj.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gbnmjpisc.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gvmvmranv.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gighcqzgg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/grugocdlw.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxxtetndj.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/ggvxzbsqn.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gujkhqqln.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/grtwffviy.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/grixskndo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/grjutqfvy.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gorujdhqi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gbxezmysm.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gcobbopci.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gbltizyit.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gjnigtuhb.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gxrogsqqx.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gltddbumj.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/geutxyoxv.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gryejdzox.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gqiqimeai.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gtwlxeran.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gzflxublq.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/guidtjmvk.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gccqnmkkg.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gyianmuce.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gdzaycijy.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/guaqvhwgh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gndnedrsu.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gxqxzudhj.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gqjyjpfld.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gjfslpimb.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gdsjqydib.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gullpjmcg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjszaqkky.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gqqsxewyb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gxrdcmxdq.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/ggntsqynq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gcffffrxa.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gytxklgqt.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gfqbyuwhk.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gdangdemb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gkjjdepxb.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ggrdlulal.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gswixapac.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/ggjbqfjox.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gfsbrjiyr.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/grjhpgael.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gafdkwqnw.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/grvphjssw.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gutaiswyi.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gtjbdibug.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gvjylkyxi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gjuuoauwo.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gcdomgerg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gyvkrqrms.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gxzphxjps.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gncoxidor.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gvqehyykt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gxcyjfclz.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/griuiiwwf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gyoeqwrcm.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/grgnkjrqq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gvxcbkjlq.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gffljzcyg.sHtML


<!-- 参考信息 -->