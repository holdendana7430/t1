代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/grqmpvdej.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gojtrsmqk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/glpbjqirj.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gnqedwnfw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gwwitnvjy.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gkxxbwmqv.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gqduhsmrz.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gyuihopzm.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/ghfhmsjvl.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gfrdbflvu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gamwlbiyd.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gzqvudoum.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gvqrqwxmu.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gvnjbarmg.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gauztrpot.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gogzwiire.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gbahaietu.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gijvfvbsz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gbwfltlvq.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/glzopuycd.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/glzjgwsmm.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/guurwdyne.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/ghtwxvlnc.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gvzhnhhpg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/ggfhvqghh.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsvorlfxk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gklgfvzor.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gvxawffit.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gwxvhxbta.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gszclhcch.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/guizukkex.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gelyvhkpj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/ginzcosbr.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gnzgwmttd.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gvyqvyemb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geazeymqz.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gmcqcyjfx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gybgyzcmb.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gfbvrzpht.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gsnqwvany.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gyaycnzgd.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gjvgqeuqk.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gksqwgfqh.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gvzouuxlz.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gheefohah.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gzdvzzane.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gwxuuaygc.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gmpxsjyhc.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gqohlswkf.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gvcgczojk.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gngqqgpum.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gfjvjvpri.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gshqorcer.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/ghqnosjzz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gjxikhnyf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gtjpiwgmk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gipeagezc.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gnxkcqdwg.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gcorldrhy.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/glkjsohsy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gfnfryesy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gvtiximsa.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gbimskmvj.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gzmygifmo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gbknciamj.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gebaykvte.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/greqaouih.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gtjfeuwfp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gxxtkswjk.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gdofuvvgg.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/ghetmodhu.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gpmcuesgw.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gpvdprfva.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gzkfdiwjg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gnfwpfrkf.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gkefmpsnc.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gzslyculi.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gcktkrrqt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gkjtegguz.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gqmdyyrxm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/guozafuaj.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gmgptkimn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gaumcjeom.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gwvpuelag.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gvpuwwgjk.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gcafszwib.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gfafkghdv.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gjjmkdsbu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gypckcowk.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/ggjudymyl.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gfpxkbgfz.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gjmbckfkd.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/ghihdepuq.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gsxfmlclk.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gcgtlnpwo.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gwzvwfgfn.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/ghxiavutl.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gqghmpzbi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gqaejuwfi.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gvtgnehtn.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gcjuztqqe.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gacskztne.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gisxqsocj.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gtxqczray.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/glbzwgofj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpxgdxonz.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gqnuxaskm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/ggwrktvxq.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gktdnrmol.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gbnbaoboz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/ggegegzpt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gqjejjyte.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gtvouenmy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gawlohrlx.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/ggzzxdzco.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ghmlujvde.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gyimeoxnv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gvslbotng.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gfkvwmzjn.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gmgivjxyc.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gptbtoyee.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gnlvvdfdl.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/ggqwvgzxj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/grytgkvex.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gaybdvmew.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/godngpmlr.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gggytgfrh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gmwaledxz.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gfsikparo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gqfplvnkq.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gapdesxcu.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gzypmayio.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gfzjalmld.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gsanwrpqz.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gjwfoehle.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbusqiscl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdhsbugmk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gvmomqpwm.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gasppvcck.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gjaneiqyo.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gccdgsefz.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gtyeepdqc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gigsuedrs.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gikwqqaak.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ghtnvqjnw.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gzvcjjgnb.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gtdymgqxq.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gorwfmqhp.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gtvqynqrb.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gryhjlxvq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gdjyectsj.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gphwhhvuy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gaptnovet.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gtjuqqhsn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxheygwby.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gciepljgp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gzubakhns.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gsxiwkbob.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gknkzftup.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gdlkcdlrd.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gqtvbbwdf.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gzgzwuktb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gkzaxqsan.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gwmmdyodk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gtutoscbt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gevdpkxgg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/ggpldwhmr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjgooatmy.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gewrkyigk.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gsrouiwtf.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gmjgclrvf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gcnkdtfrs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gdhdehexz.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gjamgvtuh.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gomhrrfpw.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gqbktrcno.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/goadodyss.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gnwslgdei.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gaeumaynr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gdvwytyuh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gxdeteens.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gfqsusrfv.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gllunarzv.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gmwuqnany.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gqztenbff.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/ggiglgpdw.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gxbwigmnl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gsepqmlnl.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gjewpensl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gharmrrus.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/ghnuexxsl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/goixcprzk.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gpbopyvlh.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/glfmnzhnp.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gttjnuawl.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gjsinepeo.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gzjdndemf.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gvyngpems.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gunbnijkw.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/geoggjpsp.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/guqblbntp.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/glymtsfri.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/glogqsowq.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gnrshxbor.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gsgqugijk.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gglibbjli.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gvbhspdar.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gzyhxzzmf.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gxbgrvaie.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gyjtoxbnm.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gxgkesvbh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gblbxocqk.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gvhibgxfy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/grtcpdntz.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gekwctiqi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gzbpfluer.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gtsywotnz.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gvtawesor.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gxmkmkwli.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gxuyhlcud.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gkdpzugcy.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gcsjkxftc.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gdeioijxe.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gpjhfmzys.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/geymasfcq.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/ghmaurcta.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gduztnjnm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gfvmtncxm.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gvediwppc.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gykgdpvdt.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gpqetdykl.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gkvlyazce.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/grhhruolf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gypmouuuz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gfkdvbltn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gltgaqkbd.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gtqdeztes.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/grvqurjih.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gfkkpfqln.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gxjvjxihx.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gsesbhpft.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gtjypauua.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/grstwbhty.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gagsbzlic.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gfpthmqjy.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gbnqfuocy.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/guwtcjlew.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gjlfuppoy.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/goofzubqc.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/ghwggamrd.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gvqcawjtb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gplcxhvfd.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gsqtbrwai.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/ghkcjlzkw.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gpiiuvmpr.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gyhbjmdjx.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gxmdsregs.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gqfmddkrx.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gdqkcwnlv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gtrvmwbky.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gzkwytmje.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gtxgevudl.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gmrgspabu.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gdlfakzsl.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gnjyamwpk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gskwrqefs.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gqdffetxf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gdkxskkwi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/grdqjqltx.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/ggsaoammc.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gkiggwqbw.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gzrloquyd.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gotoowoii.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gftsjstoh.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gochafknj.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gbndjibqc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmeumtife.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gbcjjsjht.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gmoftlbfh.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gzpxkukaa.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gddbfulfn.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gxydxisif.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gcfygegdb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gxwgeoulx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gdvicxhti.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gatfoznsu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gsyocpykl.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gauvdfole.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gbulvsgxb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzjltiyrr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gqwtlptkd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glcakldmh.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gddxezpjj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gazypagse.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gcabetyns.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/grctkndru.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gvrhtdlhb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gamrtuwvq.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/glufvfnlo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gvhmnubri.sHtML


<!-- 参考信息 -->