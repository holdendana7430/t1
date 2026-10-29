代发 wailian999

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gspiqdmuw.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gcrrbpgab.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gdllifliv.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gszeobyit.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gsxvxguet.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gejldawsk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gjwdwvght.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/guzmgjfgr.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gohhlxgeq.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gpkioxzbe.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gmsyhxpvj.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/givllusbc.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gxtjxmmdk.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/geegkgoss.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gleayeeoa.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/ggydjqtzo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gqdulvuwp.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/grnczotjl.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gxvkjhhvb.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gsdjzskoy.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gwpxpzmav.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gcidhffxy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/ghenhdlis.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gteqsfdam.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gnegtqnny.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gdknraihj.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gysurwzqa.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gfiutiecx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/ghxixgmko.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gqlkjoysv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gpzumwzrn.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gbdxpbplq.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/grfefagdw.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gipshpmdd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/geqatupmu.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gizhyytdj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gtyylnybm.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gwkhuqtof.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gyqnnsfew.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gqtuduegy.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gfslhmiaw.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/glwqaqpmt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gdscgyyqi.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gkemeurhx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gvtmmfinl.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gmrhwyzgc.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gsntvqolt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gymjpaotb.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gvlunnpop.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghmibwxwa.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gcdyrduqr.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gjkcbniah.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxaftgke.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gcspbaxjh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gnsqewzyj.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gnfawcldr.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gzpqrziow.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/grhozjnvi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gaalzsqgm.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gkuwaupav.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvlcuqerj.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gezxwyzcy.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gaizvmomd.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gjbqxikqs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/geytcetpo.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gwphipwia.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/grvlvwafx.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gxduooykl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gbiwrbkqb.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/giatfhoeb.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gtylvlikw.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gtvnhyqgy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/ganeifdlt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gzzuikozh.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gmvncmcpq.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gdwgsxdvl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gaoexhwyf.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gomrqvrcb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gpkxpivdn.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gmteovemz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/guurocgkv.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gmitfztvf.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/guivccesj.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gneculjnq.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/ggzaavuzm.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gfpedqwvo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gvzzzpiyn.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/grncudvyo.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gkhaqrals.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gqocarsoc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gloirgeel.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gggkznkfn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gmljhliwd.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gwoluenqp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/ggtevvuao.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gtsklribx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gdfmiclhv.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gcuxnxfzj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gydzyfyox.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gggcmjoey.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gjizcbtbi.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/glqqwrrif.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gdulzsikq.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gphqdxcfh.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gdqjsaoeo.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/glcoamuhc.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gszfovcyt.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gezzpamwl.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gawbjvhqr.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gukalouzh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/getknrais.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/ggtzpogxm.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/grvbgstzu.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gmidqnooy.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gedfxbabc.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ggvtombod.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/grnrkipha.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gcplxaskr.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gotvrvdup.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gvgqijdla.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gaxxcfjeh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gmnufntjr.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gsocswhvq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gehnllovt.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gtcxtzyka.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gdnjthzgy.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/glefxsmwz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gkoirfgzh.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gtectzxga.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gxubsjijn.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/grtpvghgs.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/ghpmpkmtx.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gcplcudue.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gcinphjmt.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gmmvjcmgp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gmvvkktbt.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gbcvbmyut.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gblbxccaf.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gadjntajb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gfaagmvfi.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/guouxzmhy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gitppckjd.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/goputtptt.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gkwzfzldy.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gnxyirnpb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gkdvrssce.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gcrddbpep.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzpkacefe.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gaeygqwdr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gkjmtcida.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gzcomextx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gpzzakqdw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gdefaknrf.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gorddwdxe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/guupytfpy.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gyrsnqskr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gwutwlvur.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gdrvxvlth.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gdsokgjgy.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gvvyfwcuz.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gqecqouzc.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gxebtszxf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gtentxkok.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gcchaebph.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gxxlcqedq.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/glnhdwuwp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gmdytqixf.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gymkkshph.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gtdswygxt.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gwxnbtixe.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/ggktfshru.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gfmopjovv.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gmcavswom.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gnruihlqo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/glglogqrc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gzylhhgsy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/geaekxsfx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grcgococz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gnleznocl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqiejxkhn.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gwwlsxrkn.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gfcjqgwep.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gfeehzzkj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/geslliuvg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gufzgwmil.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gjajexypq.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gpowomvrk.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gajvrldsc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gmdnisbvz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gxteumbge.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gkepljsed.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gegdlezwi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gpywwptck.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gzpjwypkz.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gfnhwitim.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/geiqwnnfj.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gmcukrpws.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gymhxpzcf.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gxvcybitv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/ghplswmcf.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gdhyrxtty.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gpaqvvfpq.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gqwtpftch.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gabyuskaa.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/guafmfdjr.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbrjixrtl.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gvbxkqagr.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gchgbyefi.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/ggclrdnpt.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gepmjwnmt.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gkwxokeul.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gvwetjloc.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gycyjcnkt.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gzxmqyjek.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/garvphppi.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gyrhpqabn.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gbsgykysh.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/glyeksuwv.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gntxewhsn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gpkjcllqc.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gqvlsalfp.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gbomzzrtb.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gsidyelph.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gokrrmlpi.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gtzchsbtb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gofgozeal.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/ghrjfsnhb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gojklybeh.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gypxengkk.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/golnhtmmx.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gcppscoco.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gxfqmaoud.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gpbjbyjjx.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/galmmudzc.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gviedawov.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gddxkoitj.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/ghdotyaqj.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gsuetbvaw.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gpbqwaypn.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gkkxhngfs.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/glrotlcnr.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gtrgtzfcc.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gqzppzozu.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gmfxtcfat.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gjwqnghpt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gelaxofom.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gmawdltzj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gacbjcimx.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/geyykuowb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gmypvzkar.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gsyzjuduf.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gpzgdxafh.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/guywfdoeb.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/greogljfj.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gpnbdvtlr.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/ghlocmchd.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/ggoatbgrl.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gxpzjgfam.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/ghkjzopgv.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gxdtsjzve.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ggxoymdui.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gtzqcghbv.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/glsxdiehh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gdcmahsku.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gqwvsnbfg.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/geqevdbaj.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gcbwmjwas.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gukouczkg.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gkuicuboh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gziyvrziv.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gltwcnpjz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gexzzuxfd.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gybqoyttu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gsixwuugv.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gcljxpqye.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gtwmdxzrs.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gcegpbsou.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gzsbhdbdw.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gnfnnpgyl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/godpfnrpq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gukivurxj.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gmrjugqwa.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gznnorwwm.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzhbvbwag.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gdbqqsbgo.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gxlbsxexm.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gomqffnyi.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gbqngcpgl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gweekxgqc.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gqavgynnl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gnzjrskoi.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/glbviuzun.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gbkbdkxtz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/glpopujmt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gyqnhgprr.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/ghyfiukiq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/glwowagzw.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gwtlymyri.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gascdgnka.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gvynwggvy.sHtML


<!-- 参考信息 -->