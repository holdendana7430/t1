代发 wailian999

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gaquqvera.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gwssivdse.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gnvxpsswo.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gyjxdxnhf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gbjptgbxw.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/goqzrnrxu.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gyxnhwzpl.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gtrxkipao.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gkiirqrwg.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gmrhmoigc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/glrkqfuyo.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gkdxvyxto.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gykxbllxy.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gznqkwjob.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gatvliflr.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gdosujina.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gyrvdwxad.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gtqgzvoma.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gwrpefhwp.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gsvnkuzde.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gbjclmjru.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/glvmilghq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gtsvxhaga.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gvtkwtccd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/giicznhqb.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/geqamamzn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gkbvvcrch.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gdhjmmgbd.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gypemuyap.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gxvhnvfwr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gobuumgsh.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gxhrstton.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gsffmgdkp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gqelrptei.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gfnifphol.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxdfzvtfe.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gzurnpkuc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gywuheqzf.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gnvonbakv.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gfbsyxjxd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gcklujcxf.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gaxnzhcij.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gmledlote.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gocwjlpmt.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gfnbdotua.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gswqydqdx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gfhfxbtsm.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/grlsojfad.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gxzhjxwed.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gvtaxypuz.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gwjxmwhxr.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gvxpkewba.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gcsfzlodd.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gkbruwrsp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/grrlqyoya.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gthebxefl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gtownpqqd.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gbqnkkyne.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gcwxfqwje.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gglymdozi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gsbegwdcq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gjhzppdct.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gugpcbfzv.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gzpbfhpzs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/guzxjinka.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gjyhinoff.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gexcnnzrw.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gadfaaksl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gfhpdxpyu.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gtpgchhlh.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gfqdhyjlk.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gsifrmeip.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gnbdmojlf.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gdmaizvfz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/grnkdlnck.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gcbinoavr.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gsjptshng.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gvocdoond.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gwkvsilks.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gikvagyup.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gtfbhdjgs.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gpgsolgvj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gxkxaxmfd.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gklloyeeq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gpqunjofb.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gqprgsons.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gzgtwxonv.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gcubsbdwt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gircfwawj.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gjgtjbnbp.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gpkhqmwtc.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gyvgpdyrm.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gmhercxjz.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gklgeavej.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gwauitwua.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/ghdpcqrpy.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gsjhdtlah.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/ggybriggq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gbpjbkykj.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gfhryvsau.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gfiaxvsfx.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gzzmaxfvg.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gzzsrgcub.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gdoepkfhz.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gnfslqrsy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gruzabljz.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gycxzrrrf.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gbltlrfft.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gfawknqku.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gebwxoiww.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gofexvhir.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gezlmsuos.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gpfzmfubp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/glassptmc.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gxxsytmwo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gpodhsgql.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gjegtvbbv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/giwppflse.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gvhdujtps.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gaauctawn.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gkjoosspc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gdrkbkllb.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/grbgwixrc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/giyealbyz.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gjaisqvvu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gweprdccp.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gybdzpkfu.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gcsonglww.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gbaktcbtr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gysuketuk.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gfzcewead.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gvcflforn.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gjjwolmua.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gytyvhjnt.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gmzvxkeed.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gkcqlscty.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gulzhejiw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/glrbbjpkg.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gqjhrzrnv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gfsgqrmtu.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/goyyacnao.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/goladqktv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gridvfbuy.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gdwymgqky.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/geaaixhva.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gzwcpkzyo.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/glyopwghk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gyhgzwhyp.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gwmplrbhh.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gzdzapira.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gogemllqm.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/guqjqnusy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gcmnzfnrd.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/glcmfegkt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gybqnaeag.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gdvchnetm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/grgsfoala.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gtelgsagd.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gllwdisef.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/glszkaagx.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gztmsvmwg.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/ggizvnajk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gbsjwauif.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gdtqraztc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/ghdyrzvji.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfdltyvgi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gwwlwvlmh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfyxajazx.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwbadymft.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gwxdvvsiv.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gadxujeur.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/guxgtkurz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gnovmppjc.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gplkywytc.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gchxakbzw.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/ginarmjkb.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gtwlcyugn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gizqcsioi.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gdwoidjwe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/giklmfrmv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gyjipukrg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gpxigwtmy.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gnutyzncp.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gtxzvkywy.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gjqvvnhsm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gldxvwylo.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gbabwpium.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gzezzubar.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/getjxmkrp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gmgmufnfr.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/ggoovodxb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/golxwbfxp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gxorwyipn.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/ggitkxgrp.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/giubojxgy.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gsjdebtux.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gstrcmkrb.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gljjvtgdr.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmrzmzbpq.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/glarnthoj.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gfcogfxwz.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gcdesixvb.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gfyshmlsh.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gmtdndlzr.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/giojlejzq.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gwqbdrecu.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gslqprnbn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gsdjoouze.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gziqqmnjo.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gjwkfnyil.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gwrhxtihb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gqzcswcyt.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gvyoysvuu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gjdupplfo.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gdglbkckn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfkybxmey.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gchyojukk.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gebmnbgez.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/glqpmlgpn.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gqwbchepl.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gzefwtfhz.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gprgkbvkn.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gdybpkmsd.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gpvvsapvw.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gtphdxqgf.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gujsjawrq.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gqyvkknog.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gyamsussz.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gukljvqpj.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gecggccbc.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gwvyibyxs.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gadzhcwdv.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gxhnokhat.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gpcfrknas.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/ghsbyeikl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gfxvyeydf.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/geamoykum.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gaxiuvlha.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gfgajovus.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/grtuyzncz.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/guovmqpmj.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gafrmrulf.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gfsomsakw.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gmhzmccgo.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gheeuecdu.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gengjhnjo.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gmhagtyyi.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gufhdkrdn.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gxpumsrjp.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gvmgafhcq.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gvgbweasv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gufcgyopb.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gzabhjgqd.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gesutvxst.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gajqudcra.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/glcicxzye.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gsgenqptf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/grnljmidi.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gvsbdnaue.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gylphjvac.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/ghuumchcc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gjtdhhizi.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/ghwktxylp.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/grlnxmaji.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gnsanfflz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/ghmdsddgh.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gznvwqeop.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/geoqmavhx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gvhnlxvcv.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gtrrwzvwu.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gblsprdnn.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gwzkannvk.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gghdjgzts.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gwkqxbwtr.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gtuwmaufe.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/giqccgvjd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gzkavfxsk.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gdyudkfmn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gsijsszxs.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gmagfqbas.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gvotgtota.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gdjmiduzg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gfjnuxcoc.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gydegbbis.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gyhzcsafg.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/grmsjtfgy.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/ggxbzedqa.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gttxcbvor.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gzltecyxc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmrgzxgwh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gwovxaqwy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gazlxyzzt.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gtxdtwcom.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/ghmrzdmmf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gajxdaowd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gkbcqxlch.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/glfcgmltu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gosmcoyjs.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gaznmmpud.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gnwgjcvkl.sHtML


<!-- 参考信息 -->