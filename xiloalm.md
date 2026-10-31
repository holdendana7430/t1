代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://bz.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qx.jctech888.com.cn

fclose(f);
来源：http://se.panjiajie.cn

[S12] C：写文件
来源：http://pg.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gr.yuntaijiaju.cn

[S13] C：宏定义
来源：http://lx.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zi.muxihuayi.cn

[S14] C：枚举
来源：http://gs.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://xo.szsharing.cn

[S15] C：类型转换
来源：http://hb.nszjky.cn

(double) a / b
来源：http://xi.nicolike.cn

[S16] C：位操作置位
来源：http://wk.shtwfgs.cn

x |= (1 << 3);
来源：http://oy.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://kd.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ew.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://zn.nszjky.cn

int main(int argc, char **argv)
来源：http://pd.hahajie.cn

[S19] C：快速排序
来源：http://my.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qk.huanxung.cn

[S20] C：二分查找
来源：http://ke.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gv.shxzukj.cn

[S21] C：字符类别判断
来源：http://be.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xz.lnxyls.cn

[S22] C：字符串转数字
来源：http://bi.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yp.hahajie.cn

[S23] C：随机数
来源：http://dv.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uf.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://eq.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://la.jctech888.com.cn

[S25] C：内存拷贝
来源：http://ek.lnxyls.cn

memcpy(dst, src, n);
来源：http://se.521024.cn

[S26] C：内存清零
来源：http://ro.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://jg.shtwfgs.cn

[S27] C：定义常量
来源：http://pf.newstarts.cn

const double PI = 3.14159;
来源：http://pb.shxzukj.cn

[S28] C：静态变量
来源：http://cd.bjjhwx.cn

static int counter = 0;
来源：http://ur.bookmarksfly.cn

[S29] C：变参函数
来源：http://vl.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nh.nicolike.cn

[S30] C：头文件保护
来源：http://eo.shtwfgs.cn

#ifndef X_H
来源：http://kk.521024.cn

#define X_H
来源：http://qz.huanxung.cn

#endif
来源：http://lf.huanxung.cn

[S31] C++：Hello World
来源：http://ju.nszjky.cn

#include <iostream>
来源：http://zq.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://xw.nszjky.cn

[S32] C++：字符串
来源：http://uz.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://vz.shxzukj.cn

[S33] C++：vector 增删
来源：http://vt.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://it.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://qb.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://bf.lnxyls.cn

[S35] C++：map
来源：http://kn.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://my.asd995.cn

[S36] C++：unordered_map
来源：http://zy.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ez.lnxyls.cn

[S37] C++：set
来源：http://vr.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ot.szxytkj.cn

[S38] C++：排序
来源：http://qk.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://ol.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://rl.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gm.asd995.cn

[S40] C++：查找元素
来源：http://zq.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jb.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://vl.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yk.colortex.cn

[S42] C++：继承与虚函数
来源：http://hz.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://fc.shxzukj.cn

[S43] C++：智能指针
来源：http://in.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://dm.haigaiapp.cn

[S44] C++：引用传参
来源：http://ag.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://ve.newstarts.cn

[S45] C++：lambda
来源：http://xc.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pa.colortex.cn

[S46] C++：函数模板
来源：http://za.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kz.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://xp.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nx.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://cq.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gb.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://gn.9csxet.cn

[S49] C++：写文件
来源：http://ny.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xu.shtwfgs.cn

[S50] C++：格式化数字
来源：http://kx.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wj.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://hz.hnjuh.cn

static_cast<double>(a) / b
来源：http://gw.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://bv.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://xv.haigaiapp.cn

[S53] C++：移动语义
来源：http://tz.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://xa.nicolike.cn

[S54] C++：异常处理
来源：http://ci.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://em.panjiajie.cn

[S55] C++：结构化绑定
来源：http://uj.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ud.bookmarksfly.cn

[S56] C++：optional
来源：http://mi.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nh.muxihuayi.cn

[S57] C++：编译期常量
来源：http://jc.chemitech.net.cn

constexpr int N = 10;
来源：http://qz.chemitech.net.cn

[S58] C++：命名空间
来源：http://zj.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://dc.huixiangedu.cn

[S59] C++：静态断言
来源：http://cm.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nm.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://au.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lf.gzmigu.cn

================================================================================
来源：http://ug.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gn.huanxung.cn

================================================================================
来源：http://ls.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://yo.szxytkj.cn

println("Hello")
来源：http://gs.hnjuh.cn

[T02] Kotlin：变量
来源：http://xw.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dx.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://at.jctech888.com.cn

"值: $b"
来源：http://uv.hnjuh.cn

[T04] Kotlin：空安全
来源：http://se.shxzukj.cn

val n: String? = null;  n?.length
来源：http://tl.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://gk.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zd.521024.cn

[T06] Kotlin：集合映射
来源：http://fe.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://me.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://ri.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nn.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://dd.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://di.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://aq.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://se.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://jx.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tx.huixiangedu.cn

[T11] Kotlin：协程
来源：http://xi.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://db.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://bg.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://cm.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://vt.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://gc.gzmigu.cn

[T14] Kotlin：循环
来源：http://ns.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://kg.nicolike.cn

[T15] Kotlin：接口
来源：http://sc.nszjky.cn

interface Shape { fun area(): Double }
来源：http://qq.nszjky.cn

[T16] Swift：Hello World
来源：http://hr.bjjhwx.cn

print("Hello")
来源：http://in.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://qj.shtwfgs.cn

var a = 1;  let b = 2
来源：http://qy.nicolike.cn

[T18] Swift：字符串插值
来源：http://lc.shxzukj.cn

"值: \(b)"
来源：http://to.hahajie.cn

[T19] Swift：可选绑定
来源：http://rl.shxzukj.cn

if let n = opt { print(n) }
来源：http://bb.huanxung.cn

[T20] Swift：数组操作
来源：http://am.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ym.wgjwhj.cn

[T21] Swift：遍历
来源：http://yz.yuntaijiaju.cn

for x in a { print(x) }
来源：http://bb.shxzukj.cn

[T22] Swift：字典
来源：http://yj.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uk.nszjky.cn

[T23] Swift：函数
来源：http://zq.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ul.lnxyls.cn

[T24] Swift：闭包
来源：http://bx.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iy.hnjuh.cn

[T25] Swift：结构体
来源：http://cd.colortex.cn

struct P { var x: Int }
来源：http://dh.yuexingan06.cn

[T26] Swift：类与重写
来源：http://is.huanxung.cn

class A: Base { override func f() {} }
来源：http://he.shtwfgs.cn

[T27] Swift：错误处理
来源：http://wm.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://dc.szxytkj.cn

[T28] Swift：枚举
来源：http://hh.shtwfgs.cn

enum Color { case red, green }
来源：http://en.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://eq.chemitech.net.cn

guard let x = opt else { return }
来源：http://dn.huixiangedu.cn

[T30] Swift：协议
来源：http://rq.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://uy.9csxet.cn

[T31] Lua：Hello World
来源：http://iv.lnxyls.cn

print("Hello")
来源：http://xe.yuexingan06.cn

[T32] Lua：局部变量
来源：http://hz.szxytkj.cn

local a = 1
来源：http://xk.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://vi.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fc.newstarts.cn

[T34] Lua：遍历表
来源：http://zi.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ot.bjjhwx.cn

[T35] Lua：字典表
来源：http://oi.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://oz.nszjky.cn

[T36] Lua：函数
来源：http://gt.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://jp.521024.cn

[T37] Lua：字符串拼接
来源：http://lm.haigaiapp.cn

"a" .. "b"
来源：http://jo.9csxet.cn

[T38] Lua：条件
来源：http://ml.huixiangedu.cn

if x > 0 then print("正") end
来源：http://mn.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://rs.huanxung.cn

string.find(s, "%d+")
来源：http://oe.lnxyls.cn

[T40] Lua：元表
来源：http://tu.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://oy.szsharing.cn

[T41] Perl：Hello World
来源：http://fe.9csxet.cn

print "Hello\n";
来源：http://vn.hahajie.cn

[T42] Perl：变量类型
来源：http://yd.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://al.szsharing.cn

[T43] Perl：字符串插值
来源：http://dq.haigaiapp.cn

"值: $a"
来源：http://hw.shxzskj.cn

[T44] Perl：条件
来源：http://th.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://zl.shxzskj.cn

[T45] Perl：数组遍历
来源：http://mk.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://jl.huanxung.cn

[T46] Perl：哈希操作
来源：http://tl.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vi.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://hq.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ah.hnjuh.cn

[T48] Perl：正则替换
来源：http://pm.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://ax.jctech888.com.cn

[T49] Perl：函数
来源：http://iy.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lq.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://yh.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://me.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://ys.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://tn.9csxet.cn

println("Hello")
来源：http://fb.wgjwhj.cn

[T52] Scala：变量
来源：http://yy.shxzukj.cn

val a = 1;  var b = 2
来源：http://wj.521024.cn

[T53] Scala：字符串插值
来源：http://zc.hahajie.cn

s"值: $b"
来源：http://sm.muxihuayi.cn

[T54] Scala：集合映射
来源：http://fj.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://vl.shxzukj.cn

[T55] Scala：集合过滤
来源：http://kk.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://np.hahajie.cn

[T56] Scala：样例类
来源：http://aw.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://mf.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://da.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://df.wgjwhj.cn

[T58] Scala：函数定义
来源：http://qx.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xj.shxzskj.cn

[T59] Scala：循环
来源：http://dk.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://gq.shtwfgs.cn

[T60] Scala：折叠
来源：http://st.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ix.huixinmuqiang.cn

================================================================================
来源：http://gf.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://te.huixinmuqiang.cn

================================================================================
来源：http://yj.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://gm.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cv.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://xd.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zl.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://sm.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oc.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://fy.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ra.521024.cn

[U05] Py：列表去重且保序
来源：http://iu.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://vr.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://sh.newstarts.cn

{**a, **b}
来源：http://ih.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://hr.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://ia.panjiajie.cn

[U08] Py：展平二维列表
来源：http://db.shtwfgs.cn

[y for x in nested for y in x]
来源：http://xe.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://wi.bookmarksfly.cn

max(d, key=d.get)
来源：http://tj.hnjuh.cn

[U10] Py：按值排序字典
来源：http://vo.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ql.521024.cn

[U11] Py：生成器表达式
来源：http://bi.huanxung.cn

(x * 2 for x in arr)
来源：http://kb.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nw.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://wk.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://te.szsharing.cn

deque(maxlen=10)
来源：http://no.521024.cn

[U14] Py：分组收集到列表
来源：http://qk.jctech888.com.cn

defaultdict(list)
来源：http://ax.muxihuayi.cn

[U15] Py：高精度计时
来源：http://hv.lnxyls.cn

t = time.perf_counter()
来源：http://om.hahajie.cn

[U16] Py：命令行参数解析
来源：http://sn.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://il.bjjhwx.cn

[U17] Py：初始化日志
来源：http://xw.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://do.szxytkj.cn

[U18] Py：预编译正则
来源：http://fr.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://cp.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://jg.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ju.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://rx.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://as.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://dx.521024.cn

@contextlib.contextmanager
来源：http://hi.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://xq.gzmigu.cn

list(zip(*m))
来源：http://bv.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://pz.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rt.asd995.cn

[U24] Py：路径操作
来源：http://pu.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sc.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://ab.panjiajie.cn

csv.DictReader(f)
来源：http://pl.bjjhwx.cn

[U26] Py：并发下载
来源：http://qo.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bh.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://co.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://rp.wgjwhj.cn

[U28] Py：类型别名
来源：http://fi.9csxet.cn

UserId = int
来源：http://zf.haigaiapp.cn

[U29] Py：属性校验
来源：http://zf.newstarts.cn

@property 与 @x.setter 配合
来源：http://gp.yuexingan06.cn

[U30] Py：数据类
来源：http://nf.gzmigu.cn

@dataclass(slots=True)
来源：http://af.shxzskj.cn

[U31] Py：单测
来源：http://lm.9csxet.cn

python -m pytest -q
来源：http://le.haigaiapp.cn

[U32] Py：代码格式化
来源：http://xf.nicolike.cn

ruff format . && ruff check --fix .
来源：http://fk.shxzukj.cn

[U33] Py：打包发布
来源：http://qh.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://uw.hahajie.cn

[U34] Py：判断编码
来源：http://hz.gzmigu.cn

chardet.detect(raw)
来源：http://jw.9csxet.cn


<!-- 参考信息 -->