代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://kc.huanxung.cn

[S02] C：变量与格式化输出
来源：http://uy.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://so.9csxet.cn

[S03] C：读入整数
来源：http://wo.newstarts.cn

int x; scanf("%d", &x);
来源：http://vc.muxihuayi.cn

[S04] C：字符串复制
来源：http://pz.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nt.bookmarksfly.cn

[S05] C：字符串长度
来源：http://ag.shxzskj.cn

strlen(s)
来源：http://ff.hahajie.cn

[S06] C：字符串比较
来源：http://eh.shtwfgs.cn

strcmp(a, b) == 0
来源：http://oa.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://bo.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xe.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://ea.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ca.asd995.cn

[S09] C：结构体定义与初始化
来源：http://gr.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mc.szsharing.cn

[S10] C：指针与解引用
来源：http://zq.colortex.cn

int *p = &a;  *p = 5;
来源：http://ba.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://qx.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://ck.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gk.muxihuayi.cn

fclose(f);
来源：http://uy.shtwfgs.cn

[S12] C：写文件
来源：http://xs.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dx.lnxyls.cn

[S13] C：宏定义
来源：http://ip.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ro.gzmigu.cn

[S14] C：枚举
来源：http://on.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://gd.9csxet.cn

[S15] C：类型转换
来源：http://nw.hahajie.cn

(double) a / b
来源：http://yd.szxytkj.cn

[S16] C：位操作置位
来源：http://wv.jctech888.com.cn

x |= (1 << 3);
来源：http://xh.hahajie.cn

[S17] C：安全拼接字符串
来源：http://qm.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sb.yuexingan06.cn

[S18] C：命令行参数
来源：http://qd.muxihuayi.cn

int main(int argc, char **argv)
来源：http://fv.hnjuh.cn

[S19] C：快速排序
来源：http://ck.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rn.szxytkj.cn

[S20] C：二分查找
来源：http://da.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ev.newstarts.cn

[S21] C：字符类别判断
来源：http://lc.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jq.hahajie.cn

[S22] C：字符串转数字
来源：http://id.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pp.bjjhwx.cn

[S23] C：随机数
来源：http://bp.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pa.szsharing.cn

[S24] C：获取本地时间
来源：http://fc.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lg.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://em.shxzukj.cn

memcpy(dst, src, n);
来源：http://jy.chemitech.net.cn

[S26] C：内存清零
来源：http://nc.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://vh.huixinmuqiang.cn

[S27] C：定义常量
来源：http://xf.gzmigu.cn

const double PI = 3.14159;
来源：http://dp.shxzskj.cn

[S28] C：静态变量
来源：http://hz.szxytkj.cn

static int counter = 0;
来源：http://ot.lnxyls.cn

[S29] C：变参函数
来源：http://iy.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kr.szxytkj.cn

[S30] C：头文件保护
来源：http://vr.colortex.cn

#ifndef X_H
来源：http://wr.521024.cn

#define X_H
来源：http://ei.huixinmuqiang.cn

#endif
来源：http://ws.szsharing.cn

[S31] C++：Hello World
来源：http://wk.huanxung.cn

#include <iostream>
来源：http://yj.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://mn.hnjuh.cn

[S32] C++：字符串
来源：http://hr.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://gj.hnjuh.cn

[S33] C++：vector 增删
来源：http://os.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ka.nicolike.cn

[S34] C++：遍历 vector
来源：http://is.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://wi.bjjhwx.cn

[S35] C++：map
来源：http://kz.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yt.9csxet.cn

[S36] C++：unordered_map
来源：http://ly.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vm.bjjhwx.cn

[S37] C++：set
来源：http://mk.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jt.szsharing.cn

[S38] C++：排序
来源：http://qs.asd995.cn

std::sort(v.begin(), v.end());
来源：http://wj.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://cc.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.lnxyls.cn

[S40] C++：查找元素
来源：http://yc.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://go.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://yv.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rh.huanxung.cn

[S42] C++：继承与虚函数
来源：http://nh.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://sb.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://bb.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://pn.muxihuayi.cn

[S44] C++：引用传参
来源：http://ei.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://tl.panjiajie.cn

[S45] C++：lambda
来源：http://sw.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ii.nicolike.cn

[S46] C++：函数模板
来源：http://tv.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tj.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://sk.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gf.hnjuh.cn

[S48] C++：逐行读文件
来源：http://eu.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wx.newstarts.cn

while (std::getline(in, line)) { }
来源：http://bx.jianghongdianzi.cn

[S49] C++：写文件
来源：http://mq.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qp.yuexingan06.cn

[S50] C++：格式化数字
来源：http://op.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ki.huanxung.cn

[S51] C++：显式类型转换
来源：http://vs.shxzskj.cn

static_cast<double>(a) / b
来源：http://ua.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://gl.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://ah.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://pt.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://nb.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://ks.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dn.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://rr.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sw.wgjwhj.cn

[S56] C++：optional
来源：http://wg.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hp.yuexingan06.cn

[S57] C++：编译期常量
来源：http://vy.lnxyls.cn

constexpr int N = 10;
来源：http://fs.shxzukj.cn

[S58] C++：命名空间
来源：http://hr.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://so.jctech888.com.cn

[S59] C++：静态断言
来源：http://ky.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://et.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://nk.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ef.gzmigu.cn

================================================================================
来源：http://kh.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wy.jctech888.com.cn

================================================================================
来源：http://qe.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://tl.newstarts.cn

println("Hello")
来源：http://ik.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://qy.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gp.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://an.muxihuayi.cn

"值: $b"
来源：http://ck.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://xm.shxzukj.cn

val n: String? = null;  n?.length
来源：http://ht.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://lm.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pm.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://do.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vr.521024.cn

[T07] Kotlin：集合过滤
来源：http://nk.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ow.nicolike.cn

[T08] Kotlin：数据类
来源：http://yh.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://sb.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://kj.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://nf.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://ei.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fs.yuexingan06.cn

[T11] Kotlin：协程
来源：http://dd.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fn.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://yq.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://sd.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://rw.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://ro.haigaiapp.cn

[T14] Kotlin：循环
来源：http://jj.szsharing.cn

for (i in 1..10) println(i)
来源：http://up.yuexingan06.cn

[T15] Kotlin：接口
来源：http://nw.nszjky.cn

interface Shape { fun area(): Double }
来源：http://xr.9csxet.cn

[T16] Swift：Hello World
来源：http://ok.yuntaijiaju.cn

print("Hello")
来源：http://rj.asd995.cn

[T17] Swift：变量与常量
来源：http://zc.nicolike.cn

var a = 1;  let b = 2
来源：http://xm.szxytkj.cn

[T18] Swift：字符串插值
来源：http://vr.shxzukj.cn

"值: \(b)"
来源：http://dm.9csxet.cn

[T19] Swift：可选绑定
来源：http://mw.nszjky.cn

if let n = opt { print(n) }
来源：http://fg.yuexingan06.cn

[T20] Swift：数组操作
来源：http://cg.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jy.gzmigu.cn

[T21] Swift：遍历
来源：http://ls.huanxung.cn

for x in a { print(x) }
来源：http://cy.yuexingan06.cn

[T22] Swift：字典
来源：http://ub.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bn.yuexingan06.cn

[T23] Swift：函数
来源：http://ux.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mx.yuexingan06.cn

[T24] Swift：闭包
来源：http://bk.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qy.hahajie.cn

[T25] Swift：结构体
来源：http://zm.nszjky.cn

struct P { var x: Int }
来源：http://vz.lnxyls.cn

[T26] Swift：类与重写
来源：http://zx.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://zn.lnxyls.cn

[T27] Swift：错误处理
来源：http://fh.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://nv.521024.cn

[T28] Swift：枚举
来源：http://ci.huixiangedu.cn

enum Color { case red, green }
来源：http://xy.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://vd.521024.cn

guard let x = opt else { return }
来源：http://yz.chemitech.net.cn

[T30] Swift：协议
来源：http://xd.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://jr.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://un.newstarts.cn

print("Hello")
来源：http://wq.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://zm.shxzskj.cn

local a = 1
来源：http://pd.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://se.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ce.panjiajie.cn

[T34] Lua：遍历表
来源：http://xr.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ef.jctech888.com.cn

[T35] Lua：字典表
来源：http://ah.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://fw.yuexingan06.cn

[T36] Lua：函数
来源：http://fg.jctech888.com.cn

function add(a, b) return a + b end
来源：http://dt.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://mn.chemitech.net.cn

"a" .. "b"
来源：http://oz.szxytkj.cn

[T38] Lua：条件
来源：http://ug.lnxyls.cn

if x > 0 then print("正") end
来源：http://hb.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://oo.shtwfgs.cn

string.find(s, "%d+")
来源：http://wf.jianghongdianzi.cn

[T40] Lua：元表
来源：http://sq.nicolike.cn

setmetatable({}, { __index = base })
来源：http://pj.gzmigu.cn

[T41] Perl：Hello World
来源：http://nb.gzmigu.cn

print "Hello\n";
来源：http://df.szxytkj.cn

[T42] Perl：变量类型
来源：http://eb.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fo.gzmigu.cn

[T43] Perl：字符串插值
来源：http://ek.szxytkj.cn

"值: $a"
来源：http://kh.521024.cn

[T44] Perl：条件
来源：http://up.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://so.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://cx.jianghongdianzi.cn

for my $x (@arr) { print $x; }
来源：http://jx.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://tw.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zf.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://wd.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kn.bjjhwx.cn

[T48] Perl：正则替换
来源：http://vy.shxzukj.cn

$s =~ s/old/new/g;
来源：http://on.chemitech.net.cn

[T49] Perl：函数
来源：http://we.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vz.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://mv.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jk.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://jx.521024.cn

[T51] Scala：Hello World
来源：http://vh.muxihuayi.cn

println("Hello")
来源：http://kn.haigaiapp.cn

[T52] Scala：变量
来源：http://jq.gzmigu.cn

val a = 1;  var b = 2
来源：http://cz.lnxyls.cn

[T53] Scala：字符串插值
来源：http://dy.muxihuayi.cn

s"值: $b"
来源：http://fl.lnxyls.cn

[T54] Scala：集合映射
来源：http://re.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://fc.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://ac.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zs.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://bv.panjiajie.cn

case class User(name: String, age: Int)
来源：http://an.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://iz.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xa.hnjuh.cn

[T58] Scala：函数定义
来源：http://tz.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zy.szxytkj.cn

[T59] Scala：循环
来源：http://gn.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://ll.szxytkj.cn

[T60] Scala：折叠
来源：http://cd.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zy.shxzukj.cn

================================================================================
来源：http://qi.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cj.yuntaijiaju.cn

================================================================================
来源：http://bk.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://tn.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uc.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://nv.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jw.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://gu.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zu.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://ay.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mt.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://hs.huanxung.cn

list(dict.fromkeys(arr))
来源：http://ul.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://sn.huixinmuqiang.cn

{**a, **b}
来源：http://gk.hahajie.cn

[U07] Py：反转字典键值
来源：http://mk.9csxet.cn

{v: k for k, v in d.items()}
来源：http://as.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://zy.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://dl.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://ua.chemitech.net.cn

max(d, key=d.get)
来源：http://wd.panjiajie.cn

[U10] Py：按值排序字典
来源：http://bg.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yx.9csxet.cn

[U11] Py：生成器表达式
来源：http://pp.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://jw.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jm.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://gu.panjiajie.cn

[U13] Py：固定长度队列
来源：http://xd.huanxung.cn

deque(maxlen=10)
来源：http://ey.9csxet.cn

[U14] Py：分组收集到列表
来源：http://bl.huixinmuqiang.cn

defaultdict(list)
来源：http://jt.yuexingan06.cn

[U15] Py：高精度计时
来源：http://gg.chemitech.net.cn

t = time.perf_counter()
来源：http://rz.521024.cn

[U16] Py：命令行参数解析
来源：http://yf.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gp.huanxung.cn

[U17] Py：初始化日志
来源：http://cy.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://lb.szxytkj.cn

[U18] Py：预编译正则
来源：http://yd.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://dr.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://xk.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rm.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://vc.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://zw.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://fc.shtwfgs.cn

@contextlib.contextmanager
来源：http://pt.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://nm.bjjhwx.cn

list(zip(*m))
来源：http://cn.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://ti.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jj.wgjwhj.cn

[U24] Py：路径操作
来源：http://du.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tj.panjiajie.cn


<!-- 参考信息 -->