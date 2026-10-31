代发 wailian999

strlen(s)
来源：http://ae.jctech888.com.cn

[S06] C：字符串比较
来源：http://ju.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://nv.szxytkj.cn

[S07] C：数组遍历求和
来源：http://qr.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tt.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://qx.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ei.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://dt.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://we.hnjuh.cn

[S10] C：指针与解引用
来源：http://qg.521024.cn

int *p = &a;  *p = 5;
来源：http://tj.wgjwhj.cn

[S11] C：逐行读文件
来源：http://gv.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://vt.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ko.huixinmuqiang.cn

fclose(f);
来源：http://tf.hahajie.cn

[S12] C：写文件
来源：http://pn.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mn.szsharing.cn

[S13] C：宏定义
来源：http://aj.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wj.lnxyls.cn

[S14] C：枚举
来源：http://zo.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://az.yuntaijiaju.cn

[S15] C：类型转换
来源：http://rn.9csxet.cn

(double) a / b
来源：http://cf.szxytkj.cn

[S16] C：位操作置位
来源：http://jd.521024.cn

x |= (1 << 3);
来源：http://xs.newstarts.cn

[S17] C：安全拼接字符串
来源：http://mn.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dh.huanxung.cn

[S18] C：命令行参数
来源：http://jk.nicolike.cn

int main(int argc, char **argv)
来源：http://ne.wgjwhj.cn

[S19] C：快速排序
来源：http://zr.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pj.szsharing.cn

[S20] C：二分查找
来源：http://fh.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bl.hnjuh.cn

[S21] C：字符类别判断
来源：http://gu.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://au.huixiangedu.cn

[S22] C：字符串转数字
来源：http://uz.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ev.nszjky.cn

[S23] C：随机数
来源：http://gy.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fx.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://ez.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ci.lnxyls.cn

[S25] C：内存拷贝
来源：http://kd.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://aj.hahajie.cn

[S26] C：内存清零
来源：http://ni.newstarts.cn

memset(a, 0, sizeof a);
来源：http://sg.huixinmuqiang.cn

[S27] C：定义常量
来源：http://ro.newstarts.cn

const double PI = 3.14159;
来源：http://ny.lnxyls.cn

[S28] C：静态变量
来源：http://zd.huanxung.cn

static int counter = 0;
来源：http://pi.hahajie.cn

[S29] C：变参函数
来源：http://qk.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hu.huixiangedu.cn

[S30] C：头文件保护
来源：http://ef.yuntaijiaju.cn

#ifndef X_H
来源：http://lq.jctech888.com.cn

#define X_H
来源：http://ru.huanxung.cn

#endif
来源：http://ek.szxytkj.cn

[S31] C++：Hello World
来源：http://ns.huanxung.cn

#include <iostream>
来源：http://kc.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://rj.nszjky.cn

[S32] C++：字符串
来源：http://wx.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://zp.huanxung.cn

[S33] C++：vector 增删
来源：http://ni.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gw.szxytkj.cn

[S34] C++：遍历 vector
来源：http://py.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://xu.bjjhwx.cn

[S35] C++：map
来源：http://lx.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rw.newstarts.cn

[S36] C++：unordered_map
来源：http://rv.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vm.hahajie.cn

[S37] C++：set
来源：http://qd.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://td.hahajie.cn

[S38] C++：排序
来源：http://iq.asd995.cn

std::sort(v.begin(), v.end());
来源：http://zt.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://vf.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cb.shtwfgs.cn

[S40] C++：查找元素
来源：http://np.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://py.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://xg.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tm.huanxung.cn

[S42] C++：继承与虚函数
来源：http://jm.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://lk.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://rx.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://ez.muxihuayi.cn

[S44] C++：引用传参
来源：http://wr.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://qo.chemitech.net.cn

[S45] C++：lambda
来源：http://ry.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qa.bookmarksfly.cn

[S46] C++：函数模板
来源：http://ku.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bt.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://xw.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://me.hnjuh.cn

[S48] C++：逐行读文件
来源：http://pq.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kv.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://uq.lnxyls.cn

[S49] C++：写文件
来源：http://iz.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kc.hahajie.cn

[S50] C++：格式化数字
来源：http://ge.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://po.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://dt.521024.cn

static_cast<double>(a) / b
来源：http://sz.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://rv.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://di.wgjwhj.cn

[S53] C++：移动语义
来源：http://gv.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://ne.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://oz.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pi.521024.cn

[S55] C++：结构化绑定
来源：http://kf.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ef.huixiangedu.cn

[S56] C++：optional
来源：http://pu.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yv.szsharing.cn

[S57] C++：编译期常量
来源：http://lo.yuexingan06.cn

constexpr int N = 10;
来源：http://xl.asd995.cn

[S58] C++：命名空间
来源：http://de.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://tu.jctech888.com.cn

[S59] C++：静态断言
来源：http://yo.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zs.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://cc.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vt.bjjhwx.cn

================================================================================
来源：http://uu.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://py.521024.cn

================================================================================
来源：http://tv.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://li.gzmigu.cn

println("Hello")
来源：http://dt.jctech888.com.cn

[T02] Kotlin：变量
来源：http://ya.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tm.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://ms.shtwfgs.cn

"值: $b"
来源：http://jj.hnjuh.cn

[T04] Kotlin：空安全
来源：http://ik.nicolike.cn

val n: String? = null;  n?.length
来源：http://ub.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://lx.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ed.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://dx.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tf.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://ql.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rv.nicolike.cn

[T08] Kotlin：数据类
来源：http://qi.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://em.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://xq.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://wk.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://ab.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uy.szxytkj.cn

[T11] Kotlin：协程
来源：http://yl.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xq.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://ql.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://es.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://na.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://nw.panjiajie.cn

[T14] Kotlin：循环
来源：http://qb.szsharing.cn

for (i in 1..10) println(i)
来源：http://hk.asd995.cn

[T15] Kotlin：接口
来源：http://tp.huanxung.cn

interface Shape { fun area(): Double }
来源：http://xv.nicolike.cn

[T16] Swift：Hello World
来源：http://ku.hahajie.cn

print("Hello")
来源：http://on.gzmigu.cn

[T17] Swift：变量与常量
来源：http://qj.asd995.cn

var a = 1;  let b = 2
来源：http://kc.lnxyls.cn

[T18] Swift：字符串插值
来源：http://ol.shtwfgs.cn

"值: \(b)"
来源：http://uc.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://gb.huanxung.cn

if let n = opt { print(n) }
来源：http://ww.yuexingan06.cn

[T20] Swift：数组操作
来源：http://ys.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uq.chemitech.net.cn

[T21] Swift：遍历
来源：http://in.shxzskj.cn

for x in a { print(x) }
来源：http://ze.jianghongdianzi.cn

[T22] Swift：字典
来源：http://xk.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jq.huixinmuqiang.cn

[T23] Swift：函数
来源：http://dm.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lv.szxytkj.cn

[T24] Swift：闭包
来源：http://ll.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gq.colortex.cn

[T25] Swift：结构体
来源：http://xo.newstarts.cn

struct P { var x: Int }
来源：http://mi.szsharing.cn

[T26] Swift：类与重写
来源：http://kw.521024.cn

class A: Base { override func f() {} }
来源：http://xd.lnxyls.cn

[T27] Swift：错误处理
来源：http://zw.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://kc.panjiajie.cn

[T28] Swift：枚举
来源：http://xa.bookmarksfly.cn

enum Color { case red, green }
来源：http://hw.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://tq.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://it.shxzukj.cn

[T30] Swift：协议
来源：http://ke.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://yn.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://ex.colortex.cn

print("Hello")
来源：http://ul.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://lx.szsharing.cn

local a = 1
来源：http://ls.nicolike.cn

[T33] Lua：表（数组）
来源：http://mj.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ti.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://hg.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hk.bookmarksfly.cn

[T35] Lua：字典表
来源：http://zf.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://sj.huixiangedu.cn

[T36] Lua：函数
来源：http://ur.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://ti.asd995.cn

[T37] Lua：字符串拼接
来源：http://bb.yuexingan06.cn

"a" .. "b"
来源：http://ck.9csxet.cn

[T38] Lua：条件
来源：http://jf.hahajie.cn

if x > 0 then print("正") end
来源：http://sd.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://hy.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://ck.panjiajie.cn

[T40] Lua：元表
来源：http://qa.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://tv.wgjwhj.cn

[T41] Perl：Hello World
来源：http://bx.szxytkj.cn

print "Hello\n";
来源：http://at.huixiangedu.cn

[T42] Perl：变量类型
来源：http://my.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mg.9csxet.cn

[T43] Perl：字符串插值
来源：http://qf.yuexingan06.cn

"值: $a"
来源：http://gy.panjiajie.cn

[T44] Perl：条件
来源：http://pl.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://di.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://ed.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://po.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://al.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hj.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://il.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nm.hahajie.cn

[T48] Perl：正则替换
来源：http://ge.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://ef.chemitech.net.cn

[T49] Perl：函数
来源：http://sa.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ez.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://va.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://df.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://dv.haigaiapp.cn

[T51] Scala：Hello World
来源：http://sm.gzmigu.cn

println("Hello")
来源：http://yo.huixiangedu.cn

[T52] Scala：变量
来源：http://ce.yuexingan06.cn

val a = 1;  var b = 2
来源：http://jy.huanxung.cn

[T53] Scala：字符串插值
来源：http://kh.gzmigu.cn

s"值: $b"
来源：http://jf.szsharing.cn

[T54] Scala：集合映射
来源：http://lt.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://gv.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://aq.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tk.yuexingan06.cn

[T56] Scala：样例类
来源：http://cq.hahajie.cn

case class User(name: String, age: Int)
来源：http://gl.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://hf.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mp.huanxung.cn

[T58] Scala：函数定义
来源：http://gj.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://eu.yuntaijiaju.cn

[T59] Scala：循环
来源：http://zw.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://xw.szxytkj.cn

[T60] Scala：折叠
来源：http://yv.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sm.wgjwhj.cn

================================================================================
来源：http://yn.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fs.bjjhwx.cn

================================================================================
来源：http://pp.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://rp.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dz.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://fc.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fx.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://zv.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rz.9csxet.cn

[U04] Py：变量调试打印
来源：http://mz.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://up.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://yl.hnjuh.cn

list(dict.fromkeys(arr))
来源：http://sf.gzmigu.cn

[U06] Py：合并两个字典
来源：http://un.asd995.cn

{**a, **b}
来源：http://sv.shxzukj.cn

[U07] Py：反转字典键值
来源：http://lv.521024.cn

{v: k for k, v in d.items()}
来源：http://ls.hnjuh.cn

[U08] Py：展平二维列表
来源：http://xf.huanxung.cn

[y for x in nested for y in x]
来源：http://th.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://wu.bookmarksfly.cn

max(d, key=d.get)
来源：http://ha.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://tm.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gf.szsharing.cn

[U11] Py：生成器表达式
来源：http://xh.gzmigu.cn

(x * 2 for x in arr)
来源：http://sm.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iv.9csxet.cn

Counter(arr).most_common(3)
来源：http://nr.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://sn.nicolike.cn

deque(maxlen=10)
来源：http://ih.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://xs.jctech888.com.cn

defaultdict(list)
来源：http://tq.nicolike.cn

[U15] Py：高精度计时
来源：http://ky.chemitech.net.cn

t = time.perf_counter()
来源：http://qp.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://xd.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ci.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://um.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://kq.huixiangedu.cn

[U18] Py：预编译正则
来源：http://pa.szsharing.cn

pat = re.compile(r"\d+")
来源：http://io.hahajie.cn

[U19] Py：正则替换带回调
来源：http://ld.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vu.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://vz.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://cr.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://mr.chemitech.net.cn

@contextlib.contextmanager
来源：http://ab.shxzskj.cn

[U22] Py：矩阵转置
来源：http://uo.szxytkj.cn

list(zip(*m))
来源：http://eb.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://ux.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uu.gzmigu.cn

[U24] Py：路径操作
来源：http://qb.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ye.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://yf.521024.cn

csv.DictReader(f)
来源：http://qp.huanxung.cn

[U26] Py：并发下载
来源：http://ki.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nj.hahajie.cn

[U27] Py：异步 HTTP
来源：http://vk.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://ji.521024.cn

[U28] Py：类型别名
来源：http://vc.haigaiapp.cn

UserId = int
来源：http://kr.huixinmuqiang.cn


<!-- 参考信息 -->