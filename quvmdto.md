代发 wailian999

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gwwcvolin.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfucehbem.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseyeidpr.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gjfsaohmr.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gzvzglnch.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/ggbajcaau.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gibqftcbt.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbvcswdn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gmtcnukog.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnquvslen.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/ggaotyqet.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gaatifwzx.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gzegbbgpa.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjehzdkbp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvceyawm.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbwusuwc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdjegqiv.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzfbvasl.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkazmfng.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gydqceqtf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gwcmcedgs.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpxreuak.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmehdqop.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gjhmnpzcy.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvtgwljv.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/giqsicnbi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqasxgoo.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjadoqada.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gnfnqqeng.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsetfnjiw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gachjqrjn.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gqudugfeq.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/grmfclbxs.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gjejrmsxp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/geemyvxdl.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwbskjiu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gebgnkncd.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwemaeal.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvzlidwc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejxtbbdg.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxytajci.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdkmbvvw.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnpnudnmu.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gdxdwptzy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyigdhvjh.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gefajhjqr.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gqeihrxpv.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxeitpoi.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gwoptugog.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gxmrtsrsq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gglffegun.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdevobanv.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gwrmfzjry.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gabduyiog.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmfxrafj.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gnizozjsv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gbmqvugwz.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/ghihoyahf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/ganggmabe.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gvzhyqnjx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gtogcqyhd.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukbdvgoq.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gplqbqpoc.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbxuscju.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gbrsprdms.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gqtzscmkl.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/greiowsdr.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvvaavefd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnrneyqt.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gmonyolzn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdigmild.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gefyvltto.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/guoqfdzrt.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gchnehsza.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpvfpqhx.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/glsdbuplr.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gqpmosfls.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbjztzsp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gcyxawqgk.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkekurbge.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlvuircw.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/ggjsrszrg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/ggpgiamls.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gkmnhizir.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gzrsxjpai.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gkaazrbgd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/galfmbjcz.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gimcwznay.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvbzkiqy.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwbpepmj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/ghwqcjgzl.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gyterbopg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqjjtyqc.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpsrxgwj.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gphgmptuz.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaudxiwif.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcsaqddw.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuxqzino.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/glscumkju.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gavhpkjuz.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvsseymp.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gofutrzyz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghemwxezh.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gpyghzara.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gpevhyehy.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gdklrwuqs.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gsjxonoqf.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gccviaiis.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gtusarmjd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkcnggka.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/guxiwekcr.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gibtnfcix.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gwluasjst.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxktqzfz.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/glxkwmfpz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gahwmroim.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gtideoxkr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghqjcwheo.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyjgbtsp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaactefa.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gblfuvguw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gibtoylcz.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfxzftqe.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gtydewchp.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gbpjvjrtg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxkhwydm.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjaqwilj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gflhsguxr.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvxnlxspu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqeggixw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzdwqnfd.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/ggdibjgog.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/grvrcypkd.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfvwsrlh.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gtjymkpvi.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiosszbl.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/guyjppotl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnhnoxwo.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbihpiaf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkxxukrwc.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gobjcnguq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gspqamwiw.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfehbxrqk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjecdoxo.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjppefmpc.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtylehseq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvtzzycz.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkhlybmo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/geesjxqim.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gebxovcpo.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnseigpa.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/groicyfpv.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwdhlhco.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzuseyxe.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyyatkqw.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikybwlaf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gfzimqnzb.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gatrmmdga.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gxnhrftip.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbhqsphe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuyccukm.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gxkdnmook.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/guqqwminb.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsysbixn.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gkomqbvqo.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/guyacfoqw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gswhbigyv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gexyzumlj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gieqhqwao.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfreechb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gcqdpxcer.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkahovrzb.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwkrsabg.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyponoafw.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyjinpmx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/geqguhfuq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbeavdkc.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gehhfolhr.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqctwznq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpjafedx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpavtgwk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/grspeydog.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhyzhzcy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxjenunk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhpdfdpw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/grdlugkuf.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gcigesqdp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwbpyimr.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gybzyorxr.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpftuirez.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/goupmcdkk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gjjfiiwrt.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxqlwstf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/glwfnwcxq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gedekpvlj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifgzubbm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbppiuia.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdgsuquv.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggdfqheh.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gonptamfm.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gslhoqpcg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvsncylx.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gpqwkdxdi.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsukszaso.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/ggkrjbjhf.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyuiroxv.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmwqjerk.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzkmuogm.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexszsder.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzgnolxl.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gbptmlwus.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonrobtxu.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gotwtjtam.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzgyyauy.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gxzcwdyua.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcvfbnpa.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/glagfnbqp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gkljpubdj.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gtifayxvl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfoxxywp.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/guhzxsmlx.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnzyzzva.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgyhgqlk.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuhzjyrp.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gnriwlaat.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnjrkyjm.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/glattnyju.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gfeokdisr.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gaqcaikqi.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gdsrxybek.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozxqqzay.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjregwee.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gggcqduzh.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjtsnunp.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgqhrtyn.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gkqydwvxh.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gikqxyeiv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gxffbcpyb.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/grtkqgdhq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnigqikqb.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gavtwurnb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcdnahnq.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkxovzlh.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/giihqnjzu.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gukjjttke.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtkbjffv.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnshgtbgu.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxypwdbrf.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gjdoeljkd.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmdowayd.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheuixoru.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gywdsfvpz.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxpslpstm.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gpathdkvm.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gorymrhtf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkasgxkwr.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gezfwhqos.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gumndvuso.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/govblgcvr.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkraqoild.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtkzjhsw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmduckbio.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gagpovptv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibhjzutk.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gschjhkpb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyjuhlby.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyaxcqck.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gwiotjztp.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxclkknfe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqqtlxjbx.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtughabvt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/ghqulsawq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gccjhjcwk.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gcodsojzo.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnzulzse.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsjasxoe.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gejgvhuqf.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gkrwvxegb.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/ghsavfauw.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjcrczlt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gciyxcywt.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnmntshx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthgptnzj.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmwcncjp.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxobpcmvu.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/guknwfvyt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtxlvnpf.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/giqdhdfpj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsvvuown.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gxlnfiztd.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gwjobkfho.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gprurjpgy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gewqidvhy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcirgham.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gejwsjdip.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gyxjhoygn.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gchmndscw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gfenefbkx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzyjfnen.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gijlyzbxa.sHtML


<!-- 参考信息 -->