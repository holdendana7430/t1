代发 wailian999

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gjlyxermv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gmsytxwjv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gpikmnedr.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gjejazwci.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gjvofqoqk.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gxreydxvk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gnpiswsid.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/ghkszajcb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gbhnneruw.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gcikeiduz.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gpycttiqi.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gzdxgiddz.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gxlgijjxl.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gbwldtlgj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/glilnejqv.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gsgwpzqhg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gqgabpcjw.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gdkcbbjgd.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gmorvjsoh.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gjtdqbpvu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/grgklynxw.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gbalxrcjg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/ghtmbdfva.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/glfquwiid.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gkrnuwrxk.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gspwqneqb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gtqdqqjon.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gtzpsdqvi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gpxxfvfll.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gsunyjmhk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/geqvvtgdg.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gsbkwjsuq.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gdgdedwol.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gkwuipgjw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gheckdxgc.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gldxtqubw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gwyffayos.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/ghepwxuch.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gbhbsctdu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggawjkwmf.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gyfnhumiq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gghtnlrog.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gllrsxrte.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/giitdselm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gjbafexdv.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/guohkjzbo.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gkjujuvzi.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/glcicfual.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gajkmvjsh.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gaslzwipi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gkygspbwx.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gzieuvnuo.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqzxdccyd.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gpygmrvhy.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gendxiypx.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gsogzrecv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/goifnohhy.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gnljmpqkj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gfjfkqzuo.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gufmfjxlk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gfhvgahba.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gpyvxzpce.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gkosqkpti.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/ggqvuidvt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gdjdheijn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gmambmxpf.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gwfjqwmwd.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gomyfeelq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gsthnycfv.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gbnrvhdtd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gpjweavwo.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gnpywjxdi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gcswahile.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gvtlsdfkj.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gpczinwve.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gaqgxzite.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/glgrgkyvo.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gcneobndd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gnstxadvt.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gakkedhzx.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gjohaluvl.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/ghmgkaknu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gujitybds.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gtsdfyuci.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gjeptcmgy.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/ghxgjcrzy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gvuvawjso.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gqcnvtbyb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gnifbkelo.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gimqrdbvz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gqsiptsmv.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gvnlcytks.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gohbqjvhk.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gwmfbstns.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gtatsyeqs.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gxyrarjce.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gwpibpmng.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gpucenady.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gayaogmka.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gnvbltdeb.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gmafjlwyp.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gyekycreu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gevffqgkw.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gozlbroqb.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gjlklyxdk.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gcsawzwop.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gybxcjsrv.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/ggrzqdanp.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gfuvbbbxd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gyyuzybwx.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gqnlmldqk.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/guemoqcjd.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/grugkscyz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gzueyvpgn.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/glfparscb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gxvqyzish.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gpcmdhqoh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/ggnbdjasj.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gbscskjob.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gncthjkvj.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gynfgtoms.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gcokvmaik.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gkwaabgki.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gcypvoutw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/grcskjuhq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gowtdbwgw.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gyhufixtv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gsqyegduo.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gkyplixda.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/ggdznshny.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/goqbyygzy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gmapwjukr.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gxxgkfmws.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gmmprhhkq.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gooxcivyf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gkbhgxbol.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gxqsgqrdd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gqnqtdvhp.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gbgiuiegv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gmpgyjnwh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/grgjfdkhe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gayyosicv.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gukvrkfpr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gitwnpydl.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gnarrgrzm.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/getibltje.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/giuzvxcsh.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gqfjkkhzb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gegqfdiml.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gfnkolxtb.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gbreproch.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gelozbfhw.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gppctisdb.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gklwfzwnr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gsagwgkop.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gtjlmlwdo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gamawbivt.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gscboumrk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/goplchaev.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gpvssedrb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gcnygrptg.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gszuzkdni.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gfvvreknw.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gkjnrlhky.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/ghrgeelbx.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gbansjpki.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gneasjdva.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/ghspgclwd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gizyhdxdz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggzjzfizb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gyyhkistu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmplhuxkp.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gsazxoghx.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gjjubomop.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gkywgjiej.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gohmfdpgj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gnyoyizqn.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gyfooyuya.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gvicewocs.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gjezggsve.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gxmvcdogl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gmspvxqna.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/ggawdkegc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/ggogyfbbc.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gqudngmrl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gcjdwmwvw.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gyrqqnjeg.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gzperdklq.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gpclrpvoq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gdxjjvcil.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gkwhtntnl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gdcpjcdui.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gnecxmhql.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gftzcepen.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gnaologog.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gskuuhkvc.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/glhkqdlzw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/goldhbmcp.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gnuomybro.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/ghuvwwrcy.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gnymynoxv.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gmbdgqfdf.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/grdygzxuf.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gadlsjeid.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gltcgqkwg.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gzwoohvyi.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/ganpswqbc.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gwekibsso.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gpfqqgvkq.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gijncvwlw.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gjjeocper.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gfyqmpejj.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gifwhngnk.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gmzplavrh.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gixtjdpva.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gifwtedku.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gtsjergfz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gziorhyoz.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gubsdodmm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/glddyoekc.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gutkdvbak.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gjltmhlxb.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/ghxuegzcw.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gdjvikgbb.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gdeohcuwj.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gshqpozgb.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/ghjhjuzyc.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gsoxnwouo.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gfqwpiert.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/giabgpete.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gmxinlgpy.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gehnfmcni.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gamcjfzco.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gdhkofond.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/glkitcgty.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gotdqbpxi.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gvfhubfna.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gzjoloxgt.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gfsoqepiu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gmbgzlgae.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gsylvpimg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gslazbbfw.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/ggmcdjarv.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gkmovvsop.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gckqpuuiz.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/goywzkbfl.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gecvywgmb.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gxmjzdzvu.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gkdtrchfe.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gmyncblmu.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/giowtuwxa.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/ghkjjhgjc.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gxxsauqln.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/grwrrsycm.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gljfgvudh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gibvucfih.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gdnhenfyf.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gmgxpgjsc.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gbogxcxuc.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gwluczmjv.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gofhqtxjw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gjkixiepq.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gmgaxpoad.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/grugbmruq.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gnlwwcrvh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gwhwbjomx.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gazloxqxj.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gfccyureq.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gfgdsxubt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gfyqlzsyp.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gsjvitdrx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gqvvnmdql.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gnohuimdv.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwjbirggd.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gjgzsljvt.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gwfnxcjcv.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gwcrfcewv.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gszrgrtdn.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gnslxtqra.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gaohscbmv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gnyajbwdn.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/guctlgeyd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gyemhdshx.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gvajxrsux.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gwwlqlkzr.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/ghpfhprlf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gzdvvvecu.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gkoasctbn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/ggfqxuwoc.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gdkxxwwwg.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/ggnxeqkvy.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gycdmnsvr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gqzmgtowq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goiyahnmk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gahamqhvn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gztwokuwn.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gdvsehvwi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/geogruogb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gomyulbzf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gsxtjqbsk.sHtML


<!-- 参考信息 -->