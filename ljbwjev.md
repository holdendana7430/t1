代发 wailian999

strlen(s)
来源：http://nv.nicolike.cn

[S06] C：字符串比较
来源：http://qo.521024.cn

strcmp(a, b) == 0
来源：http://fr.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://dd.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zk.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://xt.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rh.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://fc.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jx.wgjwhj.cn

[S10] C：指针与解引用
来源：http://gk.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://uf.huixiangedu.cn

[S11] C：逐行读文件
来源：http://gr.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://rb.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://si.huixinmuqiang.cn

fclose(f);
来源：http://gq.szsharing.cn

[S12] C：写文件
来源：http://iw.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pf.chemitech.net.cn

[S13] C：宏定义
来源：http://tx.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dk.521024.cn

[S14] C：枚举
来源：http://eb.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://zc.muxihuayi.cn

[S15] C：类型转换
来源：http://wq.muxihuayi.cn

(double) a / b
来源：http://dt.szsharing.cn

[S16] C：位操作置位
来源：http://qt.huanxung.cn

x |= (1 << 3);
来源：http://en.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://rl.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zv.yuexingan06.cn

[S18] C：命令行参数
来源：http://kd.panjiajie.cn

int main(int argc, char **argv)
来源：http://hf.yuntaijiaju.cn

[S19] C：快速排序
来源：http://ki.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ml.haigaiapp.cn

[S20] C：二分查找
来源：http://eu.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aw.panjiajie.cn

[S21] C：字符类别判断
来源：http://xu.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cb.jctech888.com.cn

[S22] C：字符串转数字
来源：http://sp.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gs.szxytkj.cn

[S23] C：随机数
来源：http://id.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wn.panjiajie.cn

[S24] C：获取本地时间
来源：http://xr.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pq.asd995.cn

[S25] C：内存拷贝
来源：http://iw.bjjhwx.cn

memcpy(dst, src, n);
来源：http://tj.newstarts.cn

[S26] C：内存清零
来源：http://vl.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://xg.szsharing.cn

[S27] C：定义常量
来源：http://rh.hnjuh.cn

const double PI = 3.14159;
来源：http://xj.yuexingan06.cn

[S28] C：静态变量
来源：http://ur.colortex.cn

static int counter = 0;
来源：http://jf.huanxung.cn

[S29] C：变参函数
来源：http://qh.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ji.szxytkj.cn

[S30] C：头文件保护
来源：http://uh.hnjuh.cn

#ifndef X_H
来源：http://xr.yuexingan06.cn

#define X_H
来源：http://ug.wgjwhj.cn

#endif
来源：http://ti.521024.cn

[S31] C++：Hello World
来源：http://hj.9csxet.cn

#include <iostream>
来源：http://ka.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ep.gzmigu.cn

[S32] C++：字符串
来源：http://iq.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://it.wgjwhj.cn

[S33] C++：vector 增删
来源：http://ol.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hp.gzmigu.cn

[S34] C++：遍历 vector
来源：http://co.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://vz.hnjuh.cn

[S35] C++：map
来源：http://lo.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://el.gzmigu.cn

[S36] C++：unordered_map
来源：http://zi.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fx.huanxung.cn

[S37] C++：set
来源：http://cm.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xe.hnjuh.cn

[S38] C++：排序
来源：http://oh.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://fk.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://lj.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tc.huixiangedu.cn

[S40] C++：查找元素
来源：http://ke.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kq.shxzskj.cn

[S41] C++：类与构造函数
来源：http://vn.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cq.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://ib.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://kj.szxytkj.cn

[S43] C++：智能指针
来源：http://sr.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://av.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://oq.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://zd.wgjwhj.cn

[S45] C++：lambda
来源：http://ns.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gc.shtwfgs.cn

[S46] C++：函数模板
来源：http://ow.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cx.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://ni.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sa.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://jn.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zs.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://fv.shxzukj.cn

[S49] C++：写文件
来源：http://cz.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://js.lnxyls.cn

[S50] C++：格式化数字
来源：http://ha.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gd.panjiajie.cn

[S51] C++：显式类型转换
来源：http://mw.gzmigu.cn

static_cast<double>(a) / b
来源：http://ia.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://mj.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://ec.bjjhwx.cn

[S53] C++：移动语义
来源：http://ml.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://wd.panjiajie.cn

[S54] C++：异常处理
来源：http://jn.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://db.521024.cn

[S55] C++：结构化绑定
来源：http://vn.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://io.gzmigu.cn

[S56] C++：optional
来源：http://pi.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ir.hahajie.cn

[S57] C++：编译期常量
来源：http://si.hnjuh.cn

constexpr int N = 10;
来源：http://xj.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://xe.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://jq.huixiangedu.cn

[S59] C++：静态断言
来源：http://ys.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qu.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://ic.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rp.shxzukj.cn

================================================================================
来源：http://al.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rh.bjjhwx.cn

================================================================================
来源：http://ap.nszjky.cn

[T01] Kotlin：Hello World
来源：http://tu.hnjuh.cn

println("Hello")
来源：http://mu.9csxet.cn

[T02] Kotlin：变量
来源：http://um.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jw.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://ik.shtwfgs.cn

"值: $b"
来源：http://lw.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://ue.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://dm.asd995.cn

[T05] Kotlin：when 表达式
来源：http://bx.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pm.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://jr.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://or.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://io.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://me.nszjky.cn

[T08] Kotlin：数据类
来源：http://aw.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://co.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://wg.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://hg.szsharing.cn

[T10] Kotlin：默认参数
来源：http://kt.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tt.yuexingan06.cn

[T11] Kotlin：协程
来源：http://qd.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uu.huanxung.cn

[T12] Kotlin：解构声明
来源：http://hf.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://fu.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://ag.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://cb.jctech888.com.cn

[T14] Kotlin：循环
来源：http://wy.hahajie.cn

for (i in 1..10) println(i)
来源：http://yw.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://mx.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://tz.bjjhwx.cn

[T16] Swift：Hello World
来源：http://tv.bookmarksfly.cn

print("Hello")
来源：http://rx.colortex.cn

[T17] Swift：变量与常量
来源：http://kr.bjjhwx.cn

var a = 1;  let b = 2
来源：http://qc.szsharing.cn

[T18] Swift：字符串插值
来源：http://it.newstarts.cn

"值: \(b)"
来源：http://mh.huanxung.cn

[T19] Swift：可选绑定
来源：http://vv.szsharing.cn

if let n = opt { print(n) }
来源：http://zu.9csxet.cn

[T20] Swift：数组操作
来源：http://tm.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tu.9csxet.cn

[T21] Swift：遍历
来源：http://hg.huanxung.cn

for x in a { print(x) }
来源：http://vu.nszjky.cn

[T22] Swift：字典
来源：http://ul.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cb.hnjuh.cn

[T23] Swift：函数
来源：http://ds.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nv.hahajie.cn

[T24] Swift：闭包
来源：http://kl.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fw.wgjwhj.cn

[T25] Swift：结构体
来源：http://gl.yuexingan06.cn

struct P { var x: Int }
来源：http://ve.huixiangedu.cn

[T26] Swift：类与重写
来源：http://tk.szsharing.cn

class A: Base { override func f() {} }
来源：http://td.asd995.cn

[T27] Swift：错误处理
来源：http://qr.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://uv.lnxyls.cn

[T28] Swift：枚举
来源：http://ll.szsharing.cn

enum Color { case red, green }
来源：http://xr.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://qh.asd995.cn

guard let x = opt else { return }
来源：http://sx.bjjhwx.cn

[T30] Swift：协议
来源：http://pa.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://kv.panjiajie.cn

[T31] Lua：Hello World
来源：http://tb.jctech888.com.cn

print("Hello")
来源：http://mv.chemitech.net.cn

[T32] Lua：局部变量
来源：http://pf.jianghongdianzi.cn

local a = 1
来源：http://kf.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://go.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ex.bjjhwx.cn

[T34] Lua：遍历表
来源：http://qd.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ng.wgjwhj.cn

[T35] Lua：字典表
来源：http://qg.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://tj.nszjky.cn

[T36] Lua：函数
来源：http://qh.jctech888.com.cn

function add(a, b) return a + b end
来源：http://ig.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://zo.shxzskj.cn

"a" .. "b"
来源：http://br.jctech888.com.cn

[T38] Lua：条件
来源：http://vq.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://ql.newstarts.cn

[T39] Lua：模式匹配
来源：http://sm.wgjwhj.cn

string.find(s, "%d+")
来源：http://bm.chemitech.net.cn

[T40] Lua：元表
来源：http://gm.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://wh.wgjwhj.cn

[T41] Perl：Hello World
来源：http://mk.521024.cn

print "Hello\n";
来源：http://fn.huixiangedu.cn

[T42] Perl：变量类型
来源：http://iw.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bj.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://mc.huanxung.cn

"值: $a"
来源：http://mk.hnjuh.cn

[T44] Perl：条件
来源：http://fw.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://rx.nicolike.cn

[T45] Perl：数组遍历
来源：http://mr.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://hu.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://ub.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fp.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://mv.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ll.asd995.cn

[T48] Perl：正则替换
来源：http://yb.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://hy.bjjhwx.cn

[T49] Perl：函数
来源：http://fq.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://no.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://pr.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ka.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://ps.shxzskj.cn

[T51] Scala：Hello World
来源：http://kl.huixiangedu.cn

println("Hello")
来源：http://wr.yuntaijiaju.cn

[T52] Scala：变量
来源：http://wi.nicolike.cn

val a = 1;  var b = 2
来源：http://xj.shxzskj.cn

[T53] Scala：字符串插值
来源：http://fl.huixiangedu.cn

s"值: $b"
来源：http://yj.huixiangedu.cn

[T54] Scala：集合映射
来源：http://oe.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://po.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://xc.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ts.shxzukj.cn

[T56] Scala：样例类
来源：http://ty.huanxung.cn

case class User(name: String, age: Int)
来源：http://ef.hnjuh.cn

[T57] Scala：模式匹配
来源：http://cr.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zy.hnjuh.cn

[T58] Scala：函数定义
来源：http://ca.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ft.9csxet.cn

[T59] Scala：循环
来源：http://mu.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://xe.chemitech.net.cn

[T60] Scala：折叠
来源：http://nr.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tm.huixinmuqiang.cn

================================================================================
来源：http://yn.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ho.chemitech.net.cn

================================================================================
来源：http://da.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://tk.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zz.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://ff.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gb.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://fv.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rv.panjiajie.cn

[U04] Py：变量调试打印
来源：http://hu.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ha.521024.cn

[U05] Py：列表去重且保序
来源：http://dy.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://bh.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://ih.nicolike.cn

{**a, **b}
来源：http://jc.huanxung.cn

[U07] Py：反转字典键值
来源：http://ak.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://ze.huanxung.cn

[U08] Py：展平二维列表
来源：http://gh.szsharing.cn

[y for x in nested for y in x]
来源：http://fd.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://ld.wgjwhj.cn

max(d, key=d.get)
来源：http://yv.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://ug.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fq.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://tn.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://ir.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lx.521024.cn

Counter(arr).most_common(3)
来源：http://rh.lnxyls.cn

[U13] Py：固定长度队列
来源：http://go.yuntaijiaju.cn

deque(maxlen=10)
来源：http://kw.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://cr.521024.cn

defaultdict(list)
来源：http://up.szxytkj.cn

[U15] Py：高精度计时
来源：http://sf.huixinmuqiang.cn

t = time.perf_counter()
来源：http://yu.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://wq.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yq.yuexingan06.cn

[U17] Py：初始化日志
来源：http://ka.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://mh.wgjwhj.cn

[U18] Py：预编译正则
来源：http://ri.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://cz.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://fk.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vf.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://wm.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://ay.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://rr.asd995.cn

@contextlib.contextmanager
来源：http://xe.szsharing.cn

[U22] Py：矩阵转置
来源：http://vi.yuntaijiaju.cn

list(zip(*m))
来源：http://fm.newstarts.cn

[U23] Py：分块读取大文件
来源：http://mw.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hs.yuexingan06.cn

[U24] Py：路径操作
来源：http://jt.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ep.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://lq.hnjuh.cn

csv.DictReader(f)
来源：http://ql.shxzukj.cn

[U26] Py：并发下载
来源：http://dk.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hm.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://pj.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://bv.chemitech.net.cn

[U28] Py：类型别名
来源：http://uz.lnxyls.cn

UserId = int
来源：http://si.521024.cn


<!-- 参考信息 -->