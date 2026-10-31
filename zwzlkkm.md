代发 wailian999

strlen(s)
来源：http://gj.muxihuayi.cn

[S06] C：字符串比较
来源：http://om.asd995.cn

strcmp(a, b) == 0
来源：http://vj.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://eg.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zr.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://tq.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lh.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://kz.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ct.jctech888.com.cn

[S10] C：指针与解引用
来源：http://yh.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://yt.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://hx.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://ee.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gt.gzmigu.cn

fclose(f);
来源：http://se.nszjky.cn

[S12] C：写文件
来源：http://wi.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oq.jctech888.com.cn

[S13] C：宏定义
来源：http://ut.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zn.yuntaijiaju.cn

[S14] C：枚举
来源：http://qx.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://mk.huanxung.cn

[S15] C：类型转换
来源：http://cg.newstarts.cn

(double) a / b
来源：http://ol.chemitech.net.cn

[S16] C：位操作置位
来源：http://aq.bjjhwx.cn

x |= (1 << 3);
来源：http://oj.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://ru.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fx.bookmarksfly.cn

[S18] C：命令行参数
来源：http://kv.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://wm.lnxyls.cn

[S19] C：快速排序
来源：http://ut.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ty.szxytkj.cn

[S20] C：二分查找
来源：http://we.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jr.huanxung.cn

[S21] C：字符类别判断
来源：http://oc.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gh.nszjky.cn

[S22] C：字符串转数字
来源：http://zo.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://or.shtwfgs.cn

[S23] C：随机数
来源：http://av.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cr.newstarts.cn

[S24] C：获取本地时间
来源：http://rq.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wu.muxihuayi.cn

[S25] C：内存拷贝
来源：http://az.szsharing.cn

memcpy(dst, src, n);
来源：http://ri.shtwfgs.cn

[S26] C：内存清零
来源：http://if.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://id.yuntaijiaju.cn

[S27] C：定义常量
来源：http://pi.wgjwhj.cn

const double PI = 3.14159;
来源：http://xl.wgjwhj.cn

[S28] C：静态变量
来源：http://gz.jctech888.com.cn

static int counter = 0;
来源：http://ru.szsharing.cn

[S29] C：变参函数
来源：http://lh.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fz.bookmarksfly.cn

[S30] C：头文件保护
来源：http://jb.hnjuh.cn

#ifndef X_H
来源：http://od.bookmarksfly.cn

#define X_H
来源：http://iz.szsharing.cn

#endif
来源：http://vm.panjiajie.cn

[S31] C++：Hello World
来源：http://ll.panjiajie.cn

#include <iostream>
来源：http://xx.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://gw.huixiangedu.cn

[S32] C++：字符串
来源：http://ix.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://dz.shxzukj.cn

[S33] C++：vector 增删
来源：http://je.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jy.9csxet.cn

[S34] C++：遍历 vector
来源：http://xf.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://wc.newstarts.cn

[S35] C++：map
来源：http://rd.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sd.hahajie.cn

[S36] C++：unordered_map
来源：http://vd.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xi.huanxung.cn

[S37] C++：set
来源：http://lx.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wf.huixiangedu.cn

[S38] C++：排序
来源：http://ea.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://sb.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://ir.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mp.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://pa.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eb.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://ww.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qm.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://xv.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://yi.muxihuayi.cn

[S43] C++：智能指针
来源：http://of.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://an.jctech888.com.cn

[S44] C++：引用传参
来源：http://ul.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://oa.521024.cn

[S45] C++：lambda
来源：http://nq.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gm.521024.cn

[S46] C++：函数模板
来源：http://xh.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nm.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://lz.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qe.shxzukj.cn

[S48] C++：逐行读文件
来源：http://ik.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ct.hahajie.cn

while (std::getline(in, line)) { }
来源：http://za.newstarts.cn

[S49] C++：写文件
来源：http://tc.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lc.haigaiapp.cn

[S50] C++：格式化数字
来源：http://dp.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ue.nszjky.cn

[S51] C++：显式类型转换
来源：http://he.asd995.cn

static_cast<double>(a) / b
来源：http://fm.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://my.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://ma.asd995.cn

[S53] C++：移动语义
来源：http://rj.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://ru.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://yh.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zd.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://ek.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hd.yuntaijiaju.cn

[S56] C++：optional
来源：http://qk.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dl.shxzskj.cn

[S57] C++：编译期常量
来源：http://yk.shxzukj.cn

constexpr int N = 10;
来源：http://df.muxihuayi.cn

[S58] C++：命名空间
来源：http://ht.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://wm.shxzskj.cn

[S59] C++：静态断言
来源：http://gf.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yb.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://uh.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cb.huixinmuqiang.cn

================================================================================
来源：http://xx.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jb.lnxyls.cn

================================================================================
来源：http://hy.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://jq.newstarts.cn

println("Hello")
来源：http://gu.yuexingan06.cn

[T02] Kotlin：变量
来源：http://ib.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yx.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://uc.haigaiapp.cn

"值: $b"
来源：http://nk.asd995.cn

[T04] Kotlin：空安全
来源：http://ay.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://wv.asd995.cn

[T05] Kotlin：when 表达式
来源：http://wo.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vg.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://yf.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lh.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://uz.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pb.hahajie.cn

[T08] Kotlin：数据类
来源：http://ca.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://er.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://dk.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://qt.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://us.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dc.jctech888.com.cn

[T11] Kotlin：协程
来源：http://zd.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dd.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://zo.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://jv.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://ou.9csxet.cn

val m = mapOf("a" to 1)
来源：http://lp.wgjwhj.cn

[T14] Kotlin：循环
来源：http://rr.huanxung.cn

for (i in 1..10) println(i)
来源：http://da.nszjky.cn

[T15] Kotlin：接口
来源：http://gm.huanxung.cn

interface Shape { fun area(): Double }
来源：http://if.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://sl.haigaiapp.cn

print("Hello")
来源：http://tt.colortex.cn

[T17] Swift：变量与常量
来源：http://oh.chemitech.net.cn

var a = 1;  let b = 2
来源：http://ot.hahajie.cn

[T18] Swift：字符串插值
来源：http://ec.shtwfgs.cn

"值: \(b)"
来源：http://ru.gzmigu.cn

[T19] Swift：可选绑定
来源：http://pk.gzmigu.cn

if let n = opt { print(n) }
来源：http://ua.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://cz.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vd.hnjuh.cn

[T21] Swift：遍历
来源：http://qo.shxzukj.cn

for x in a { print(x) }
来源：http://gq.haigaiapp.cn

[T22] Swift：字典
来源：http://bp.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ku.szxytkj.cn

[T23] Swift：函数
来源：http://xm.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cz.asd995.cn

[T24] Swift：闭包
来源：http://le.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kj.wgjwhj.cn

[T25] Swift：结构体
来源：http://ai.gzmigu.cn

struct P { var x: Int }
来源：http://jy.chemitech.net.cn

[T26] Swift：类与重写
来源：http://tk.newstarts.cn

class A: Base { override func f() {} }
来源：http://gm.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://op.nicolike.cn

do { try f() } catch { print(error) }
来源：http://lf.szxytkj.cn

[T28] Swift：枚举
来源：http://jx.asd995.cn

enum Color { case red, green }
来源：http://hy.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://uq.panjiajie.cn

guard let x = opt else { return }
来源：http://lp.hahajie.cn

[T30] Swift：协议
来源：http://ew.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://tw.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://td.muxihuayi.cn

print("Hello")
来源：http://kj.chemitech.net.cn

[T32] Lua：局部变量
来源：http://mr.newstarts.cn

local a = 1
来源：http://wx.lnxyls.cn

[T33] Lua：表（数组）
来源：http://gh.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kv.haigaiapp.cn

[T34] Lua：遍历表
来源：http://ha.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zl.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://mi.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://qf.9csxet.cn

[T36] Lua：函数
来源：http://gx.asd995.cn

function add(a, b) return a + b end
来源：http://yi.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://tg.shtwfgs.cn

"a" .. "b"
来源：http://vr.shxzukj.cn

[T38] Lua：条件
来源：http://bk.colortex.cn

if x > 0 then print("正") end
来源：http://ca.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://es.huanxung.cn

string.find(s, "%d+")
来源：http://oe.jianghongdianzi.cn

[T40] Lua：元表
来源：http://mr.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://jd.hnjuh.cn

[T41] Perl：Hello World
来源：http://vm.jctech888.com.cn

print "Hello\n";
来源：http://dz.jctech888.com.cn

[T42] Perl：变量类型
来源：http://vj.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lp.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://bg.panjiajie.cn

"值: $a"
来源：http://qk.hnjuh.cn

[T44] Perl：条件
来源：http://kb.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://in.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://pc.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://ix.szxytkj.cn

[T46] Perl：哈希操作
来源：http://eq.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ge.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://pu.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ho.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://zk.shxzukj.cn

$s =~ s/old/new/g;
来源：http://dg.chemitech.net.cn

[T49] Perl：函数
来源：http://al.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ah.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://xm.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ta.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://ug.haigaiapp.cn

[T51] Scala：Hello World
来源：http://cu.bookmarksfly.cn

println("Hello")
来源：http://tn.hnjuh.cn

[T52] Scala：变量
来源：http://be.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://bt.hahajie.cn

[T53] Scala：字符串插值
来源：http://pu.wgjwhj.cn

s"值: $b"
来源：http://fn.shxzukj.cn

[T54] Scala：集合映射
来源：http://xf.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://dh.panjiajie.cn

[T55] Scala：集合过滤
来源：http://cs.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xj.szxytkj.cn

[T56] Scala：样例类
来源：http://km.521024.cn

case class User(name: String, age: Int)
来源：http://cg.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://ee.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ln.shxzukj.cn

[T58] Scala：函数定义
来源：http://re.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cg.hnjuh.cn

[T59] Scala：循环
来源：http://py.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://yf.hnjuh.cn

[T60] Scala：折叠
来源：http://lb.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nw.chemitech.net.cn

================================================================================
来源：http://zb.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ha.shxzskj.cn

================================================================================
来源：http://by.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://zg.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rm.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://ia.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bm.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://hi.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fg.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://dr.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tf.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://qx.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://fa.hahajie.cn

[U06] Py：合并两个字典
来源：http://ti.shxzukj.cn

{**a, **b}
来源：http://nz.hnjuh.cn

[U07] Py：反转字典键值
来源：http://sn.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://aq.hahajie.cn

[U08] Py：展平二维列表
来源：http://cn.wgjwhj.cn

[y for x in nested for y in x]
来源：http://ms.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://ku.wgjwhj.cn

max(d, key=d.get)
来源：http://sd.nszjky.cn

[U10] Py：按值排序字典
来源：http://wj.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vt.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://qn.asd995.cn

(x * 2 for x in arr)
来源：http://yn.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xi.shxzukj.cn

Counter(arr).most_common(3)
来源：http://jv.gzmigu.cn

[U13] Py：固定长度队列
来源：http://rz.bjjhwx.cn

deque(maxlen=10)
来源：http://ul.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://rh.muxihuayi.cn

defaultdict(list)
来源：http://as.szsharing.cn

[U15] Py：高精度计时
来源：http://hq.asd995.cn

t = time.perf_counter()
来源：http://lu.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://is.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dp.newstarts.cn

[U17] Py：初始化日志
来源：http://de.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://pt.huanxung.cn

[U18] Py：预编译正则
来源：http://bq.huanxung.cn

pat = re.compile(r"\d+")
来源：http://gh.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://ym.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kd.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://ds.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://mw.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://hr.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://qt.huanxung.cn

[U22] Py：矩阵转置
来源：http://yg.nszjky.cn

list(zip(*m))
来源：http://nj.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://vq.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sb.bjjhwx.cn

[U24] Py：路径操作
来源：http://ic.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bv.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://as.bookmarksfly.cn

csv.DictReader(f)
来源：http://nz.nszjky.cn

[U26] Py：并发下载
来源：http://gx.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vb.nszjky.cn

[U27] Py：异步 HTTP
来源：http://mj.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://vq.9csxet.cn

[U28] Py：类型别名
来源：http://zj.shxzskj.cn

UserId = int
来源：http://ng.hahajie.cn


<!-- 参考信息 -->