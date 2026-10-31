代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://cj.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yv.yuntaijiaju.cn

fclose(f);
来源：http://yd.521024.cn

[S12] C：写文件
来源：http://vh.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://al.haigaiapp.cn

[S13] C：宏定义
来源：http://jm.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bs.chemitech.net.cn

[S14] C：枚举
来源：http://av.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://vo.gzmigu.cn

[S15] C：类型转换
来源：http://ez.wgjwhj.cn

(double) a / b
来源：http://xp.asd995.cn

[S16] C：位操作置位
来源：http://zs.shxzukj.cn

x |= (1 << 3);
来源：http://aw.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://nk.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tw.nicolike.cn

[S18] C：命令行参数
来源：http://mx.nicolike.cn

int main(int argc, char **argv)
来源：http://au.bjjhwx.cn

[S19] C：快速排序
来源：http://mv.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://su.szsharing.cn

[S20] C：二分查找
来源：http://qa.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sl.9csxet.cn

[S21] C：字符类别判断
来源：http://qp.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fa.yuexingan06.cn

[S22] C：字符串转数字
来源：http://oi.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://el.huixiangedu.cn

[S23] C：随机数
来源：http://rh.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gv.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://od.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zb.colortex.cn

[S25] C：内存拷贝
来源：http://si.shxzskj.cn

memcpy(dst, src, n);
来源：http://es.yuntaijiaju.cn

[S26] C：内存清零
来源：http://qd.hahajie.cn

memset(a, 0, sizeof a);
来源：http://lz.szsharing.cn

[S27] C：定义常量
来源：http://qy.muxihuayi.cn

const double PI = 3.14159;
来源：http://re.chemitech.net.cn

[S28] C：静态变量
来源：http://gv.szsharing.cn

static int counter = 0;
来源：http://hk.shtwfgs.cn

[S29] C：变参函数
来源：http://nr.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dp.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://da.chemitech.net.cn

#ifndef X_H
来源：http://as.huanxung.cn

#define X_H
来源：http://vc.hahajie.cn

#endif
来源：http://if.huixiangedu.cn

[S31] C++：Hello World
来源：http://lu.nszjky.cn

#include <iostream>
来源：http://zq.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://vj.9csxet.cn

[S32] C++：字符串
来源：http://dy.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://ay.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://jf.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jr.asd995.cn

[S34] C++：遍历 vector
来源：http://nd.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://dx.jctech888.com.cn

[S35] C++：map
来源：http://um.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zr.szsharing.cn

[S36] C++：unordered_map
来源：http://qw.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jv.bookmarksfly.cn

[S37] C++：set
来源：http://sm.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cb.nszjky.cn

[S38] C++：排序
来源：http://wi.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://ly.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://nx.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uz.colortex.cn

[S40] C++：查找元素
来源：http://vt.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tc.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://se.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://po.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://rq.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://lf.huixiangedu.cn

[S43] C++：智能指针
来源：http://ku.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://pe.hahajie.cn

[S44] C++：引用传参
来源：http://js.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://ag.jctech888.com.cn

[S45] C++：lambda
来源：http://dj.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fn.shxzskj.cn

[S46] C++：函数模板
来源：http://gn.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zf.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://jm.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vd.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://ia.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fx.nicolike.cn

while (std::getline(in, line)) { }
来源：http://gz.bjjhwx.cn

[S49] C++：写文件
来源：http://jv.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hb.hahajie.cn

[S50] C++：格式化数字
来源：http://yf.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qd.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://zb.nicolike.cn

static_cast<double>(a) / b
来源：http://nm.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://ny.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://nm.colortex.cn

[S53] C++：移动语义
来源：http://cu.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://vy.asd995.cn

[S54] C++：异常处理
来源：http://rv.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gu.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://qe.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://br.jctech888.com.cn

[S56] C++：optional
来源：http://bt.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jc.gzmigu.cn

[S57] C++：编译期常量
来源：http://iw.521024.cn

constexpr int N = 10;
来源：http://ac.haigaiapp.cn

[S58] C++：命名空间
来源：http://sn.521024.cn

namespace ns { int f() { return 1; } }
来源：http://vj.wgjwhj.cn

[S59] C++：静态断言
来源：http://ga.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yf.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://lo.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yw.9csxet.cn

================================================================================
来源：http://iy.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://db.521024.cn

================================================================================
来源：http://nc.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://fp.szxytkj.cn

println("Hello")
来源：http://ab.nszjky.cn

[T02] Kotlin：变量
来源：http://hv.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fl.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://cq.9csxet.cn

"值: $b"
来源：http://gk.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://zd.asd995.cn

val n: String? = null;  n?.length
来源：http://so.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://zs.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://me.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://wk.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://md.521024.cn

[T07] Kotlin：集合过滤
来源：http://qh.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kv.hahajie.cn

[T08] Kotlin：数据类
来源：http://of.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://wa.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://wa.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://nn.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://ls.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bf.yuexingan06.cn

[T11] Kotlin：协程
来源：http://xn.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yu.hahajie.cn

[T12] Kotlin：解构声明
来源：http://xg.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://jj.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://md.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://ho.hnjuh.cn

[T14] Kotlin：循环
来源：http://fw.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://mr.lnxyls.cn

[T15] Kotlin：接口
来源：http://np.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://ku.haigaiapp.cn

[T16] Swift：Hello World
来源：http://qr.huanxung.cn

print("Hello")
来源：http://wh.szxytkj.cn

[T17] Swift：变量与常量
来源：http://we.huanxung.cn

var a = 1;  let b = 2
来源：http://wu.szsharing.cn

[T18] Swift：字符串插值
来源：http://rw.colortex.cn

"值: \(b)"
来源：http://xk.colortex.cn

[T19] Swift：可选绑定
来源：http://by.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://yo.huanxung.cn

[T20] Swift：数组操作
来源：http://bm.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://st.newstarts.cn

[T21] Swift：遍历
来源：http://vm.521024.cn

for x in a { print(x) }
来源：http://wr.lnxyls.cn

[T22] Swift：字典
来源：http://ao.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hv.panjiajie.cn

[T23] Swift：函数
来源：http://fn.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tl.nicolike.cn

[T24] Swift：闭包
来源：http://sv.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xp.szxytkj.cn

[T25] Swift：结构体
来源：http://sp.9csxet.cn

struct P { var x: Int }
来源：http://ng.panjiajie.cn

[T26] Swift：类与重写
来源：http://kg.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://xc.shxzukj.cn

[T27] Swift：错误处理
来源：http://iv.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://nm.wgjwhj.cn

[T28] Swift：枚举
来源：http://wp.9csxet.cn

enum Color { case red, green }
来源：http://kh.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://cl.bookmarksfly.cn

guard let x = opt else { return }
来源：http://in.lnxyls.cn

[T30] Swift：协议
来源：http://wf.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://kp.colortex.cn

[T31] Lua：Hello World
来源：http://hx.muxihuayi.cn

print("Hello")
来源：http://dh.shtwfgs.cn

[T32] Lua：局部变量
来源：http://ll.wgjwhj.cn

local a = 1
来源：http://ns.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://hi.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wr.szxytkj.cn

[T34] Lua：遍历表
来源：http://hr.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uh.bookmarksfly.cn

[T35] Lua：字典表
来源：http://kr.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://oa.szsharing.cn

[T36] Lua：函数
来源：http://xh.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://nk.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://gn.huixinmuqiang.cn

"a" .. "b"
来源：http://hg.nszjky.cn

[T38] Lua：条件
来源：http://uz.szxytkj.cn

if x > 0 then print("正") end
来源：http://if.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://io.shxzskj.cn

string.find(s, "%d+")
来源：http://hd.shtwfgs.cn

[T40] Lua：元表
来源：http://vm.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://nz.panjiajie.cn

[T41] Perl：Hello World
来源：http://kn.huixiangedu.cn

print "Hello\n";
来源：http://gy.szsharing.cn

[T42] Perl：变量类型
来源：http://ux.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cx.nszjky.cn

[T43] Perl：字符串插值
来源：http://vy.huixinmuqiang.cn

"值: $a"
来源：http://ak.huixinmuqiang.cn

[T44] Perl：条件
来源：http://to.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://dc.newstarts.cn

[T45] Perl：数组遍历
来源：http://ab.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://gm.colortex.cn

[T46] Perl：哈希操作
来源：http://kr.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sy.shxzukj.cn

[T47] Perl：正则捕获
来源：http://vo.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rv.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://oy.shxzukj.cn

$s =~ s/old/new/g;
来源：http://my.szxytkj.cn

[T49] Perl：函数
来源：http://ta.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ni.asd995.cn

[T50] Perl：逐行读文件
来源：http://zl.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ka.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://cs.newstarts.cn

[T51] Scala：Hello World
来源：http://if.shxzukj.cn

println("Hello")
来源：http://mu.colortex.cn

[T52] Scala：变量
来源：http://ru.colortex.cn

val a = 1;  var b = 2
来源：http://is.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://qs.szxytkj.cn

s"值: $b"
来源：http://fn.9csxet.cn

[T54] Scala：集合映射
来源：http://bu.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://bz.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://nt.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xx.shtwfgs.cn

[T56] Scala：样例类
来源：http://zr.huanxung.cn

case class User(name: String, age: Int)
来源：http://wc.shxzskj.cn

[T57] Scala：模式匹配
来源：http://az.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ox.panjiajie.cn

[T58] Scala：函数定义
来源：http://zr.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://el.colortex.cn

[T59] Scala：循环
来源：http://hq.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://wt.szxytkj.cn

[T60] Scala：折叠
来源：http://tl.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yr.shxzukj.cn

================================================================================
来源：http://fu.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cl.shxzskj.cn

================================================================================
来源：http://zd.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://wc.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ft.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://yi.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wk.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://ox.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rf.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://tp.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rs.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://ku.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://mb.nicolike.cn

[U06] Py：合并两个字典
来源：http://lx.shtwfgs.cn

{**a, **b}
来源：http://qb.colortex.cn

[U07] Py：反转字典键值
来源：http://hu.asd995.cn

{v: k for k, v in d.items()}
来源：http://ct.hahajie.cn

[U08] Py：展平二维列表
来源：http://yj.nszjky.cn

[y for x in nested for y in x]
来源：http://pj.521024.cn

[U09] Py：字典取最大值的键
来源：http://yv.szsharing.cn

max(d, key=d.get)
来源：http://oh.newstarts.cn

[U10] Py：按值排序字典
来源：http://zn.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fz.9csxet.cn

[U11] Py：生成器表达式
来源：http://cu.haigaiapp.cn

(x * 2 for x in arr)
来源：http://uq.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dg.newstarts.cn

Counter(arr).most_common(3)
来源：http://po.lnxyls.cn

[U13] Py：固定长度队列
来源：http://cp.nicolike.cn

deque(maxlen=10)
来源：http://ea.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://xu.shtwfgs.cn

defaultdict(list)
来源：http://ag.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://go.muxihuayi.cn

t = time.perf_counter()
来源：http://kc.szsharing.cn

[U16] Py：命令行参数解析
来源：http://bw.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://od.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://bt.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://yg.gzmigu.cn

[U18] Py：预编译正则
来源：http://vk.szsharing.cn

pat = re.compile(r"\d+")
来源：http://ed.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://kv.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nx.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://al.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://vq.521024.cn

[U21] Py：自定义上下文管理器
来源：http://gi.asd995.cn

@contextlib.contextmanager
来源：http://ic.shxzukj.cn

[U22] Py：矩阵转置
来源：http://gk.lnxyls.cn

list(zip(*m))
来源：http://dv.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://bx.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vd.wgjwhj.cn

[U24] Py：路径操作
来源：http://vh.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vb.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://yq.wgjwhj.cn

csv.DictReader(f)
来源：http://gt.hnjuh.cn

[U26] Py：并发下载
来源：http://na.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bo.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://di.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://cy.haigaiapp.cn

[U28] Py：类型别名
来源：http://cs.shtwfgs.cn

UserId = int
来源：http://ga.shtwfgs.cn

[U29] Py：属性校验
来源：http://sj.szxytkj.cn

@property 与 @x.setter 配合
来源：http://qn.muxihuayi.cn

[U30] Py：数据类
来源：http://gm.bookmarksfly.cn

@dataclass(slots=True)
来源：http://wd.colortex.cn

[U31] Py：单测
来源：http://zu.shtwfgs.cn

python -m pytest -q
来源：http://vl.hahajie.cn

[U32] Py：代码格式化
来源：http://eq.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://fw.shxzukj.cn

[U33] Py：打包发布
来源：http://bv.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://cp.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://yy.panjiajie.cn

chardet.detect(raw)
来源：http://qs.huixiangedu.cn


<!-- 参考信息 -->