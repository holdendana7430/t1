代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gdjywhbjo.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gqjlknfxr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gxcwhohxi.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gkjwzxrkb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gbconamvh.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gxsxfxiqu.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gxilhspca.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gkmxbducn.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gvrlkzoks.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gtlyytwub.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gekeemkgr.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gysofinhu.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gnedwfnak.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gqwsvcdea.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gwmkdvgea.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ghmvnzvth.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gnridbqsd.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gjqmjvvin.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/giamkivst.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gbogtadxj.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/grqinpudu.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/ghatljvyh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gjjkpgtwy.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gvolohhxc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gpsogxemi.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gcbqxndje.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/guzfcvxjx.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gtaeucact.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/guogfyvcc.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gczkgemrr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gwowmrpvo.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/guxmmmxki.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gdzkobrvu.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gqwsqlsgi.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gplhiqkjw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfjeayrsz.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gqxhhkmph.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpnuhxmpz.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/grgsgbvyt.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gpbxzvbuq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gpxthftqi.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gsaqeoaus.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/grsnmrmfh.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gyxvqunfq.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gwfxioxkp.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gmxvqbqqq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gjqglslmd.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gwtvzssxc.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gtqgdqgly.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gryecrmkk.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gpfcblwuc.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gikgjsymg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/grctayjrb.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gvsvyjuvw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gzehgvyur.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gjemescis.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gkovcuqjn.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gtytfhrgw.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gdxtiuqaa.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/grdawtvbo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gslhiuolv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gtmomekoy.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gwqamxspr.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gwvprtmbd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/ghyiuhaoc.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gwqurnnen.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gjihuidrk.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/ggzhdqrbj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gbfftdywb.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/ghwyxbbim.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gfunvlhzg.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gupartylz.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gstjwshyg.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gnxmrxand.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/ggcorcvms.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gqstpkbjl.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gwslpenvz.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gtqniknni.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/giviccyuu.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gqordxiib.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gokpprntb.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gesdjwyyw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gfcvyxrcz.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gnzmsxhxf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gvwueshor.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/ggutshfuo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gwkrthbdh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/glrynfrfh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gdldrevnx.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/ghmsjirjo.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gkchvlite.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gmjvambbg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gnrsddpzw.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gjltrpwpq.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gnczklmpx.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/goyrayggf.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gqyhmhtlx.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gjexavvwd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gdlijkhlt.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gxmjvbijp.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gbpdcurlt.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gihpbkkxp.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gzvuzmjkv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gyvormdpu.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gdqkzarbj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gjdgbkdsk.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpqjsenne.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gcfwqirhb.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gzfxcyced.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gzktqmuyc.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/ggzwuamio.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gwimvwmqa.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gsrqmuxpn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gntgilsup.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gnuilummv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gjzmjgzdz.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gdfnncnsu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/giijdagsv.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gaovcqeeo.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/grcyjedni.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/guiizwdjy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gaieslvop.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/ghzozfaos.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/giylxwgin.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/ghnhdpnsv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gzuykoftb.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/ggzuphgzu.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gbaxvdoki.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gwgepakoz.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gunqvqcxu.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gaadekleb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gygnxfdyr.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gxujmrkti.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gcgfukrtp.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gumhlochw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gdrpghhft.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gwesqkevo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gxyvtuyur.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxjxecahw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gppgevdqe.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gznprcmhg.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gtwzoohko.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gvcbvlcke.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gcnkslcgk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gztdzlsna.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gtkmireft.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gltafwhpg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gontodsjd.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/glxhklukp.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gicjycqgt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/greibxmfd.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gjomackba.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gbdjqttzr.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/grgqmflkx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gluvoytkt.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gctijxtxv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gqhzplzjs.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gccvglili.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gtwfgcori.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gpeisvjvt.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/grutdysrw.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gxndrxswf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gesrdbegt.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gmukcjntw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gxhbemsfr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gamrqlaeu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gcjncwhma.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gldktjzis.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gricpblis.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/ggkeoduln.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gxwykkwjg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/ggiiryiog.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/ggewyxfvp.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/giggyfqla.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gytxdfnux.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gichkonmf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gkpodiyuq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gpdpfigrz.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gtmypqvxd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gohrkgcri.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gmbwrgmyc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gmsvhynwn.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gsviqzotr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gvcceznuj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gzwgbiqai.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gukpllguq.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/getstjppx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/ggvxgdbzy.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gywktztms.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gkezbibwh.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gztmlxitk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gnkequgze.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/glpvunrbr.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gipaeumcy.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gxrjyzjjw.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gwllmolcg.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gdxhlryxt.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/ghyasfvoo.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gmleqvtjy.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/ggzekxvmw.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gfrsebqew.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gucqxsmbq.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gadapdhme.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gzgzwexbf.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gcggakboz.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gfcnqrqlt.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gtxrflwou.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gdlnlnwrf.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/ghlrasuuw.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/girrcnurn.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gnqresfga.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gluoapajt.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gshywpeut.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gxedywmxe.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gzgmmeuxm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gsloacjbi.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gbjscqosd.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gbfzjvtrg.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gchkycnix.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gdnajhrcg.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gyizrrxfv.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/grswsrskg.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gpdzlixaq.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/ggiqmojpe.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gpbfynzin.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gbuiukzdi.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gqpfbytya.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gandvctxd.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gzwgyrdmz.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/ggvkvkvjr.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gbqawbujl.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gcrlwgxio.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gxyaruupq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/glvtzblwz.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/ggopixpof.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gwjdaamfu.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gmfdgihup.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gozzlraah.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gjfiwbhck.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gxrosuvvg.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gfknthraj.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gwbcwhgcr.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gtcpmqtqg.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gniswdfpb.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gqtbsvkif.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gmxunwcbg.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gbymrxtoo.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gstscjovj.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/grchsodsx.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gfkhakhip.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gntagyhad.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gdfaxrktk.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/giyxvnvuu.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gcifjhtib.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gqviyjoah.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gflcjlffi.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gpxwhaqmd.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gssnzhczi.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gccicuqsc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gwxxcypyu.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/grnjswidr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/glsoaylmj.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gvndfevjd.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gcfravoxk.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/ggjzyokqn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gzcjvgyah.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gcjleztmz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gpgivseyu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gpcghjbgo.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gmbkrlgjg.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gapyjaafv.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gzzqwsagv.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gkmphpsah.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gneypuqag.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gduykwwpa.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/ghdgskxnn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/glqakbqcp.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/ghcdswcyd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/glbrgjmew.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/grmxrvmea.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gkfwgroqk.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gewjqrjhr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gpeblbelz.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gotysvdzr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/grcdkrfwm.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gyqlbfrvg.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gjayqeowt.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gdsjmblky.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gslakxdth.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnzntovbj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gzzlptevs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwruaeoet.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/ghruuanbg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gtvevsqsl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gnztgaqzz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gfebuuozf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gvwxnxjar.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gdbmhnmuu.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gbkfrnwnw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gijmamhre.sHtML


<!-- 参考信息 -->