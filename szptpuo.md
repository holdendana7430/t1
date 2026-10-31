代发 wailian999

int x; scanf("%d", &x);
来源：http://br.hahajie.cn

[S04] C：字符串复制
来源：http://vn.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fi.hahajie.cn

[S05] C：字符串长度
来源：http://vr.hnjuh.cn

strlen(s)
来源：http://zu.hahajie.cn

[S06] C：字符串比较
来源：http://ns.muxihuayi.cn

strcmp(a, b) == 0
来源：http://it.shxzukj.cn

[S07] C：数组遍历求和
来源：http://ah.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jr.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://ko.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sj.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://rf.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aq.huanxung.cn

[S10] C：指针与解引用
来源：http://gm.nicolike.cn

int *p = &a;  *p = 5;
来源：http://go.521024.cn

[S11] C：逐行读文件
来源：http://zf.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://ye.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hh.huanxung.cn

fclose(f);
来源：http://ws.hnjuh.cn

[S12] C：写文件
来源：http://nf.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mx.huanxung.cn

[S13] C：宏定义
来源：http://ns.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oj.shtwfgs.cn

[S14] C：枚举
来源：http://eu.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://pz.lnxyls.cn

[S15] C：类型转换
来源：http://yv.szxytkj.cn

(double) a / b
来源：http://vr.nicolike.cn

[S16] C：位操作置位
来源：http://yn.panjiajie.cn

x |= (1 << 3);
来源：http://kd.asd995.cn

[S17] C：安全拼接字符串
来源：http://ih.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rv.asd995.cn

[S18] C：命令行参数
来源：http://dg.asd995.cn

int main(int argc, char **argv)
来源：http://jr.hahajie.cn

[S19] C：快速排序
来源：http://ps.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ly.muxihuayi.cn

[S20] C：二分查找
来源：http://wb.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tz.hnjuh.cn

[S21] C：字符类别判断
来源：http://rc.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cq.huanxung.cn

[S22] C：字符串转数字
来源：http://ba.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fp.szxytkj.cn

[S23] C：随机数
来源：http://gy.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pj.wgjwhj.cn

[S24] C：获取本地时间
来源：http://be.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wk.szsharing.cn

[S25] C：内存拷贝
来源：http://is.panjiajie.cn

memcpy(dst, src, n);
来源：http://qu.shxzukj.cn

[S26] C：内存清零
来源：http://ht.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://qg.panjiajie.cn

[S27] C：定义常量
来源：http://mm.panjiajie.cn

const double PI = 3.14159;
来源：http://ko.muxihuayi.cn

[S28] C：静态变量
来源：http://mc.newstarts.cn

static int counter = 0;
来源：http://mg.lnxyls.cn

[S29] C：变参函数
来源：http://od.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cm.nszjky.cn

[S30] C：头文件保护
来源：http://jf.9csxet.cn

#ifndef X_H
来源：http://ot.shxzskj.cn

#define X_H
来源：http://sy.9csxet.cn

#endif
来源：http://id.panjiajie.cn

[S31] C++：Hello World
来源：http://co.shxzukj.cn

#include <iostream>
来源：http://sg.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://qp.lnxyls.cn

[S32] C++：字符串
来源：http://sk.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://mf.shtwfgs.cn

[S33] C++：vector 增删
来源：http://hy.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mo.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://xw.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://ie.huixiangedu.cn

[S35] C++：map
来源：http://pi.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ha.shxzskj.cn

[S36] C++：unordered_map
来源：http://gf.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tk.shxzskj.cn

[S37] C++：set
来源：http://df.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://el.huixinmuqiang.cn

[S38] C++：排序
来源：http://mh.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://he.521024.cn

[S39] C++：自定义比较器排序
来源：http://om.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cg.panjiajie.cn

[S40] C++：查找元素
来源：http://ym.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ak.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://ym.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://on.9csxet.cn

[S42] C++：继承与虚函数
来源：http://on.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://zu.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://fp.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://ug.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://ti.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://fv.shxzskj.cn

[S45] C++：lambda
来源：http://vf.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ok.nszjky.cn

[S46] C++：函数模板
来源：http://yz.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://og.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://bt.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lo.nicolike.cn

[S48] C++：逐行读文件
来源：http://fu.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bl.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://zu.szxytkj.cn

[S49] C++：写文件
来源：http://gs.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kn.chemitech.net.cn

[S50] C++：格式化数字
来源：http://cl.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pd.asd995.cn

[S51] C++：显式类型转换
来源：http://qg.hahajie.cn

static_cast<double>(a) / b
来源：http://pl.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://sh.9csxet.cn

int size() const noexcept { return n_; }
来源：http://dt.haigaiapp.cn

[S53] C++：移动语义
来源：http://zq.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://if.521024.cn

[S54] C++：异常处理
来源：http://yg.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fl.9csxet.cn

[S55] C++：结构化绑定
来源：http://jk.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gq.panjiajie.cn

[S56] C++：optional
来源：http://vh.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ws.chemitech.net.cn

[S57] C++：编译期常量
来源：http://gm.muxihuayi.cn

constexpr int N = 10;
来源：http://mp.yuexingan06.cn

[S58] C++：命名空间
来源：http://vu.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://el.hahajie.cn

[S59] C++：静态断言
来源：http://vi.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://su.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://tc.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dz.wgjwhj.cn

================================================================================
来源：http://kv.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oh.bookmarksfly.cn

================================================================================
来源：http://yr.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://tg.hahajie.cn

println("Hello")
来源：http://wt.yuexingan06.cn

[T02] Kotlin：变量
来源：http://tj.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oc.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://uf.bjjhwx.cn

"值: $b"
来源：http://cc.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://zw.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://sq.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://ug.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ea.521024.cn

[T06] Kotlin：集合映射
来源：http://ly.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ym.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://cn.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ov.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://ft.asd995.cn

data class User(val name: String, val age: Int)
来源：http://jx.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://yv.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://pn.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://eh.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sj.asd995.cn

[T11] Kotlin：协程
来源：http://yv.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lv.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://bb.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://fv.colortex.cn

[T13] Kotlin：只读 Map
来源：http://au.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://gy.hahajie.cn

[T14] Kotlin：循环
来源：http://tp.szxytkj.cn

for (i in 1..10) println(i)
来源：http://bg.huixiangedu.cn

[T15] Kotlin：接口
来源：http://ig.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://ab.chemitech.net.cn

[T16] Swift：Hello World
来源：http://bs.colortex.cn

print("Hello")
来源：http://bp.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://bm.hnjuh.cn

var a = 1;  let b = 2
来源：http://ya.nszjky.cn

[T18] Swift：字符串插值
来源：http://lw.521024.cn

"值: \(b)"
来源：http://za.colortex.cn

[T19] Swift：可选绑定
来源：http://fm.szxytkj.cn

if let n = opt { print(n) }
来源：http://vr.szxytkj.cn

[T20] Swift：数组操作
来源：http://np.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wi.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://gn.nszjky.cn

for x in a { print(x) }
来源：http://ld.bjjhwx.cn

[T22] Swift：字典
来源：http://lr.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wm.haigaiapp.cn

[T23] Swift：函数
来源：http://vs.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xl.hnjuh.cn

[T24] Swift：闭包
来源：http://mm.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tw.hnjuh.cn

[T25] Swift：结构体
来源：http://jg.asd995.cn

struct P { var x: Int }
来源：http://rc.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://ji.szxytkj.cn

class A: Base { override func f() {} }
来源：http://im.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://dj.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://yi.huanxung.cn

[T28] Swift：枚举
来源：http://bw.huixinmuqiang.cn

enum Color { case red, green }
来源：http://lk.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://fa.asd995.cn

guard let x = opt else { return }
来源：http://zr.nszjky.cn

[T30] Swift：协议
来源：http://zq.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://jt.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://tm.szsharing.cn

print("Hello")
来源：http://ho.wgjwhj.cn

[T32] Lua：局部变量
来源：http://eh.nicolike.cn

local a = 1
来源：http://ya.521024.cn

[T33] Lua：表（数组）
来源：http://sr.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sl.hnjuh.cn

[T34] Lua：遍历表
来源：http://yh.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dy.nszjky.cn

[T35] Lua：字典表
来源：http://gt.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://dt.szsharing.cn

[T36] Lua：函数
来源：http://ah.jctech888.com.cn

function add(a, b) return a + b end
来源：http://dh.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://nj.shtwfgs.cn

"a" .. "b"
来源：http://fi.nszjky.cn

[T38] Lua：条件
来源：http://nf.yuexingan06.cn

if x > 0 then print("正") end
来源：http://se.nicolike.cn

[T39] Lua：模式匹配
来源：http://rq.panjiajie.cn

string.find(s, "%d+")
来源：http://ry.yuexingan06.cn

[T40] Lua：元表
来源：http://px.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://be.huixiangedu.cn

[T41] Perl：Hello World
来源：http://wr.shxzukj.cn

print "Hello\n";
来源：http://bm.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://fz.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iv.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://vm.yuexingan06.cn

"值: $a"
来源：http://yd.szsharing.cn

[T44] Perl：条件
来源：http://aa.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://qa.colortex.cn

[T45] Perl：数组遍历
来源：http://al.521024.cn

for my $x (@arr) { print $x; }
来源：http://ja.shxzukj.cn

[T46] Perl：哈希操作
来源：http://cq.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qd.shxzukj.cn

[T47] Perl：正则捕获
来源：http://kb.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ev.haigaiapp.cn

[T48] Perl：正则替换
来源：http://jn.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://ue.jctech888.com.cn

[T49] Perl：函数
来源：http://cq.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zg.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://qk.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ig.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ww.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://au.9csxet.cn

println("Hello")
来源：http://tu.yuexingan06.cn

[T52] Scala：变量
来源：http://wi.huixiangedu.cn

val a = 1;  var b = 2
来源：http://ve.9csxet.cn

[T53] Scala：字符串插值
来源：http://ld.521024.cn

s"值: $b"
来源：http://es.newstarts.cn

[T54] Scala：集合映射
来源：http://fi.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://ne.asd995.cn

[T55] Scala：集合过滤
来源：http://vf.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nm.shxzskj.cn

[T56] Scala：样例类
来源：http://xk.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://io.huanxung.cn

[T57] Scala：模式匹配
来源：http://em.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://st.shxzukj.cn

[T58] Scala：函数定义
来源：http://zd.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fy.chemitech.net.cn

[T59] Scala：循环
来源：http://ga.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://pi.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://nq.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qm.wgjwhj.cn

================================================================================
来源：http://gw.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ym.szsharing.cn

================================================================================
来源：http://sm.521024.cn

[U01] Py：创建虚拟环境
来源：http://ug.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ge.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://ep.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kt.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://rp.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ew.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://tg.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fb.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://ek.asd995.cn

list(dict.fromkeys(arr))
来源：http://ak.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://tm.shtwfgs.cn

{**a, **b}
来源：http://xo.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://mi.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://mi.colortex.cn

[U08] Py：展平二维列表
来源：http://hd.521024.cn

[y for x in nested for y in x]
来源：http://ri.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://ia.huixinmuqiang.cn

max(d, key=d.get)
来源：http://rg.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://yg.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mc.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://cz.nszjky.cn

(x * 2 for x in arr)
来源：http://jm.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vw.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://zv.szxytkj.cn

[U13] Py：固定长度队列
来源：http://us.shtwfgs.cn

deque(maxlen=10)
来源：http://en.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://sn.shxzukj.cn

defaultdict(list)
来源：http://dv.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://nd.gzmigu.cn

t = time.perf_counter()
来源：http://gm.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://re.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rg.szxytkj.cn

[U17] Py：初始化日志
来源：http://ef.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://ed.shxzukj.cn

[U18] Py：预编译正则
来源：http://fx.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://re.newstarts.cn

[U19] Py：正则替换带回调
来源：http://jq.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oh.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://il.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://kj.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://ov.szsharing.cn

@contextlib.contextmanager
来源：http://tq.newstarts.cn

[U22] Py：矩阵转置
来源：http://vx.chemitech.net.cn

list(zip(*m))
来源：http://iv.huanxung.cn

[U23] Py：分块读取大文件
来源：http://to.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wa.huixiangedu.cn

[U24] Py：路径操作
来源：http://qf.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qa.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://sk.yuexingan06.cn

csv.DictReader(f)
来源：http://kf.yuexingan06.cn

[U26] Py：并发下载
来源：http://xe.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hh.jctech888.com.cn


<!-- 参考信息 -->