代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://af.shxzskj.cn

[S10] C：指针与解引用
来源：http://zv.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://fl.jctech888.com.cn

[S11] C：逐行读文件
来源：http://hx.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://mq.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bz.bookmarksfly.cn

fclose(f);
来源：http://sr.asd995.cn

[S12] C：写文件
来源：http://db.szxytkj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ve.yuntaijiaju.cn

[S13] C：宏定义
来源：http://lh.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tw.shxzukj.cn

[S14] C：枚举
来源：http://kd.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://pn.bjjhwx.cn

[S15] C：类型转换
来源：http://kk.lnxyls.cn

(double) a / b
来源：http://uf.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://ub.bjjhwx.cn

x |= (1 << 3);
来源：http://ev.nicolike.cn

[S17] C：安全拼接字符串
来源：http://io.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kj.shtwfgs.cn

[S18] C：命令行参数
来源：http://nd.shxzskj.cn

int main(int argc, char **argv)
来源：http://yr.wgjwhj.cn

[S19] C：快速排序
来源：http://xn.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tt.shtwfgs.cn

[S20] C：二分查找
来源：http://gs.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cs.shxzskj.cn

[S21] C：字符类别判断
来源：http://ta.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wv.bjjhwx.cn

[S22] C：字符串转数字
来源：http://je.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fx.lnxyls.cn

[S23] C：随机数
来源：http://wa.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pc.9csxet.cn

[S24] C：获取本地时间
来源：http://au.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dz.jctech888.com.cn

[S25] C：内存拷贝
来源：http://aa.colortex.cn

memcpy(dst, src, n);
来源：http://uo.shxzukj.cn

[S26] C：内存清零
来源：http://hx.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://fl.gzmigu.cn

[S27] C：定义常量
来源：http://ws.bjjhwx.cn

const double PI = 3.14159;
来源：http://cj.nszjky.cn

[S28] C：静态变量
来源：http://cr.jianghongdianzi.cn

static int counter = 0;
来源：http://gq.nicolike.cn

[S29] C：变参函数
来源：http://gh.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://os.asd995.cn

[S30] C：头文件保护
来源：http://mc.panjiajie.cn

#ifndef X_H
来源：http://eq.bjjhwx.cn

#define X_H
来源：http://si.nicolike.cn

#endif
来源：http://yi.newstarts.cn

[S31] C++：Hello World
来源：http://je.gzmigu.cn

#include <iostream>
来源：http://wa.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://ia.gzmigu.cn

[S32] C++：字符串
来源：http://hq.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://lj.szxytkj.cn

[S33] C++：vector 增删
来源：http://ul.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ns.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://fn.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://wi.wgjwhj.cn

[S35] C++：map
来源：http://tu.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jv.panjiajie.cn

[S36] C++：unordered_map
来源：http://kp.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nc.bookmarksfly.cn

[S37] C++：set
来源：http://et.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zv.gzmigu.cn

[S38] C++：排序
来源：http://ib.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://iv.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://wf.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ko.muxihuayi.cn

[S40] C++：查找元素
来源：http://bx.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zw.9csxet.cn

[S41] C++：类与构造函数
来源：http://mg.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cg.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://mw.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://ps.muxihuayi.cn

[S43] C++：智能指针
来源：http://zx.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://ug.nicolike.cn

[S44] C++：引用传参
来源：http://is.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://kw.huixinmuqiang.cn

[S45] C++：lambda
来源：http://wy.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tn.shtwfgs.cn

[S46] C++：函数模板
来源：http://bj.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nx.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://fv.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rl.szxytkj.cn

[S48] C++：逐行读文件
来源：http://jx.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ps.newstarts.cn

while (std::getline(in, line)) { }
来源：http://if.nszjky.cn

[S49] C++：写文件
来源：http://xg.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lm.lnxyls.cn

[S50] C++：格式化数字
来源：http://vv.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zo.gzmigu.cn

[S51] C++：显式类型转换
来源：http://wk.szxytkj.cn

static_cast<double>(a) / b
来源：http://xz.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://rs.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://wv.szsharing.cn

[S53] C++：移动语义
来源：http://on.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://tj.shxzskj.cn

[S54] C++：异常处理
来源：http://xr.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cy.szsharing.cn

[S55] C++：结构化绑定
来源：http://gr.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wg.gzmigu.cn

[S56] C++：optional
来源：http://cq.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://et.panjiajie.cn

[S57] C++：编译期常量
来源：http://ab.bookmarksfly.cn

constexpr int N = 10;
来源：http://tq.hnjuh.cn

[S58] C++：命名空间
来源：http://li.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://si.9csxet.cn

[S59] C++：静态断言
来源：http://js.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ve.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://fq.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ol.wgjwhj.cn

================================================================================
来源：http://xs.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ye.huixinmuqiang.cn

================================================================================
来源：http://nh.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://hp.szxytkj.cn

println("Hello")
来源：http://xb.hnjuh.cn

[T02] Kotlin：变量
来源：http://yo.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vt.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://mi.bookmarksfly.cn

"值: $b"
来源：http://ve.szxytkj.cn

[T04] Kotlin：空安全
来源：http://kz.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://oy.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://sx.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nl.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://yl.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vg.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://jy.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kg.szsharing.cn

[T08] Kotlin：数据类
来源：http://ak.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://ab.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://hk.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://zq.newstarts.cn

[T10] Kotlin：默认参数
来源：http://mk.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pj.chemitech.net.cn

[T11] Kotlin：协程
来源：http://te.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zx.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://aj.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://kz.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://zp.hahajie.cn

val m = mapOf("a" to 1)
来源：http://ik.panjiajie.cn

[T14] Kotlin：循环
来源：http://cj.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://eg.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://fo.nszjky.cn

interface Shape { fun area(): Double }
来源：http://pq.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://tq.shtwfgs.cn

print("Hello")
来源：http://yp.asd995.cn

[T17] Swift：变量与常量
来源：http://lr.chemitech.net.cn

var a = 1;  let b = 2
来源：http://mp.szxytkj.cn

[T18] Swift：字符串插值
来源：http://uz.szsharing.cn

"值: \(b)"
来源：http://de.panjiajie.cn

[T19] Swift：可选绑定
来源：http://yj.huixiangedu.cn

if let n = opt { print(n) }
来源：http://wk.lnxyls.cn

[T20] Swift：数组操作
来源：http://ux.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pt.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://pi.muxihuayi.cn

for x in a { print(x) }
来源：http://am.lnxyls.cn

[T22] Swift：字典
来源：http://rt.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bt.jctech888.com.cn

[T23] Swift：函数
来源：http://di.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vh.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://go.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://el.gzmigu.cn

[T25] Swift：结构体
来源：http://kc.muxihuayi.cn

struct P { var x: Int }
来源：http://oi.nszjky.cn

[T26] Swift：类与重写
来源：http://vr.lnxyls.cn

class A: Base { override func f() {} }
来源：http://lb.gzmigu.cn

[T27] Swift：错误处理
来源：http://qd.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://pf.jctech888.com.cn

[T28] Swift：枚举
来源：http://rc.nszjky.cn

enum Color { case red, green }
来源：http://bw.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://hn.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://ak.jianghongdianzi.cn

[T30] Swift：协议
来源：http://uw.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://un.shxzskj.cn

[T31] Lua：Hello World
来源：http://bd.gzmigu.cn

print("Hello")
来源：http://hj.haigaiapp.cn

[T32] Lua：局部变量
来源：http://mm.9csxet.cn

local a = 1
来源：http://hf.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://od.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uv.huanxung.cn

[T34] Lua：遍历表
来源：http://xk.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wc.lnxyls.cn

[T35] Lua：字典表
来源：http://bs.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://fs.521024.cn

[T36] Lua：函数
来源：http://ua.huanxung.cn

function add(a, b) return a + b end
来源：http://nc.szsharing.cn

[T37] Lua：字符串拼接
来源：http://qn.hahajie.cn

"a" .. "b"
来源：http://sf.huanxung.cn

[T38] Lua：条件
来源：http://fi.szsharing.cn

if x > 0 then print("正") end
来源：http://pp.lnxyls.cn

[T39] Lua：模式匹配
来源：http://rq.panjiajie.cn

string.find(s, "%d+")
来源：http://as.newstarts.cn

[T40] Lua：元表
来源：http://sb.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://ta.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://nj.shxzukj.cn

print "Hello\n";
来源：http://gi.hnjuh.cn

[T42] Perl：变量类型
来源：http://tt.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ty.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://lm.jianghongdianzi.cn

"值: $a"
来源：http://zm.szsharing.cn

[T44] Perl：条件
来源：http://wy.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://if.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://ki.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://yt.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://kj.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wv.shxzukj.cn

[T47] Perl：正则捕获
来源：http://jt.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rz.521024.cn

[T48] Perl：正则替换
来源：http://ss.panjiajie.cn

$s =~ s/old/new/g;
来源：http://na.colortex.cn

[T49] Perl：函数
来源：http://zz.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mc.nicolike.cn

[T50] Perl：逐行读文件
来源：http://hb.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ns.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ok.lnxyls.cn

[T51] Scala：Hello World
来源：http://xk.huixinmuqiang.cn

println("Hello")
来源：http://gk.hnjuh.cn

[T52] Scala：变量
来源：http://uf.shxzukj.cn

val a = 1;  var b = 2
来源：http://tv.521024.cn

[T53] Scala：字符串插值
来源：http://is.muxihuayi.cn

s"值: $b"
来源：http://df.chemitech.net.cn

[T54] Scala：集合映射
来源：http://rr.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://yf.szxytkj.cn

[T55] Scala：集合过滤
来源：http://he.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ur.newstarts.cn

[T56] Scala：样例类
来源：http://ys.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://tc.shxzskj.cn

[T57] Scala：模式匹配
来源：http://sy.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kb.haigaiapp.cn

[T58] Scala：函数定义
来源：http://wr.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qe.nicolike.cn

[T59] Scala：循环
来源：http://um.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://yx.nicolike.cn

[T60] Scala：折叠
来源：http://wp.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qg.9csxet.cn

================================================================================
来源：http://mm.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bs.wgjwhj.cn

================================================================================
来源：http://lu.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://wm.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ii.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://nm.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cf.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://wt.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jo.asd995.cn

[U04] Py：变量调试打印
来源：http://iu.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qg.nszjky.cn

[U05] Py：列表去重且保序
来源：http://mg.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://do.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://rz.panjiajie.cn

{**a, **b}
来源：http://av.521024.cn

[U07] Py：反转字典键值
来源：http://yc.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://sf.huanxung.cn

[U08] Py：展平二维列表
来源：http://vw.panjiajie.cn

[y for x in nested for y in x]
来源：http://nn.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://qq.colortex.cn

max(d, key=d.get)
来源：http://cl.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://sl.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hx.huanxung.cn

[U11] Py：生成器表达式
来源：http://pa.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://zn.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zg.szxytkj.cn

Counter(arr).most_common(3)
来源：http://hr.gzmigu.cn

[U13] Py：固定长度队列
来源：http://nb.huixinmuqiang.cn

deque(maxlen=10)
来源：http://tm.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://ck.gzmigu.cn

defaultdict(list)
来源：http://fa.haigaiapp.cn

[U15] Py：高精度计时
来源：http://es.muxihuayi.cn

t = time.perf_counter()
来源：http://tt.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://rn.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vo.colortex.cn

[U17] Py：初始化日志
来源：http://du.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://yw.shxzskj.cn

[U18] Py：预编译正则
来源：http://gr.newstarts.cn

pat = re.compile(r"\d+")
来源：http://nc.521024.cn

[U19] Py：正则替换带回调
来源：http://qo.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ft.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://he.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://by.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://ns.bookmarksfly.cn

@contextlib.contextmanager
来源：http://ng.colortex.cn

[U22] Py：矩阵转置
来源：http://mj.shtwfgs.cn

list(zip(*m))
来源：http://gi.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://ns.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oa.521024.cn

[U24] Py：路径操作
来源：http://bk.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qj.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://un.muxihuayi.cn

csv.DictReader(f)
来源：http://mh.jctech888.com.cn

[U26] Py：并发下载
来源：http://kr.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ug.9csxet.cn

[U27] Py：异步 HTTP
来源：http://uj.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://oo.jctech888.com.cn

[U28] Py：类型别名
来源：http://lp.hnjuh.cn

UserId = int
来源：http://wo.szsharing.cn

[U29] Py：属性校验
来源：http://ln.shxzskj.cn

@property 与 @x.setter 配合
来源：http://kn.haigaiapp.cn

[U30] Py：数据类
来源：http://hh.szxytkj.cn

@dataclass(slots=True)
来源：http://dj.panjiajie.cn

[U31] Py：单测
来源：http://xu.lnxyls.cn

python -m pytest -q
来源：http://xr.nszjky.cn

[U32] Py：代码格式化
来源：http://dv.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://bu.szxytkj.cn


<!-- 参考信息 -->