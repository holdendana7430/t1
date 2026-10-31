代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://xl.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lz.haigaiapp.cn

fclose(f);
来源：http://pw.haigaiapp.cn

[S12] C：写文件
来源：http://th.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sx.shtwfgs.cn

[S13] C：宏定义
来源：http://sz.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zh.bjjhwx.cn

[S14] C：枚举
来源：http://xr.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://xw.chemitech.net.cn

[S15] C：类型转换
来源：http://ip.panjiajie.cn

(double) a / b
来源：http://sc.panjiajie.cn

[S16] C：位操作置位
来源：http://nx.bookmarksfly.cn

x |= (1 << 3);
来源：http://qr.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://ux.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sd.521024.cn

[S18] C：命令行参数
来源：http://fr.bjjhwx.cn

int main(int argc, char **argv)
来源：http://jw.shxzukj.cn

[S19] C：快速排序
来源：http://wt.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://og.chemitech.net.cn

[S20] C：二分查找
来源：http://ql.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xk.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://sx.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tn.yuexingan06.cn

[S22] C：字符串转数字
来源：http://ui.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dc.colortex.cn

[S23] C：随机数
来源：http://ln.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ne.wgjwhj.cn

[S24] C：获取本地时间
来源：http://lu.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xi.shtwfgs.cn

[S25] C：内存拷贝
来源：http://nv.wgjwhj.cn

memcpy(dst, src, n);
来源：http://dy.bjjhwx.cn

[S26] C：内存清零
来源：http://ft.asd995.cn

memset(a, 0, sizeof a);
来源：http://rm.haigaiapp.cn

[S27] C：定义常量
来源：http://me.muxihuayi.cn

const double PI = 3.14159;
来源：http://hq.wgjwhj.cn

[S28] C：静态变量
来源：http://ln.521024.cn

static int counter = 0;
来源：http://un.521024.cn

[S29] C：变参函数
来源：http://jb.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dm.nszjky.cn

[S30] C：头文件保护
来源：http://yx.521024.cn

#ifndef X_H
来源：http://qk.chemitech.net.cn

#define X_H
来源：http://ka.newstarts.cn

#endif
来源：http://sf.huanxung.cn

[S31] C++：Hello World
来源：http://lt.szxytkj.cn

#include <iostream>
来源：http://sa.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://mw.521024.cn

[S32] C++：字符串
来源：http://bu.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://fb.panjiajie.cn

[S33] C++：vector 增删
来源：http://od.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://md.hahajie.cn

[S34] C++：遍历 vector
来源：http://tr.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://jx.yuexingan06.cn

[S35] C++：map
来源：http://pv.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aa.chemitech.net.cn

[S36] C++：unordered_map
来源：http://zc.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://we.wgjwhj.cn

[S37] C++：set
来源：http://pq.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sr.huixinmuqiang.cn

[S38] C++：排序
来源：http://xf.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://ky.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://la.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ea.huixiangedu.cn

[S40] C++：查找元素
来源：http://wk.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kp.hahajie.cn

[S41] C++：类与构造函数
来源：http://rb.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nk.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://bk.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://sf.gzmigu.cn

[S43] C++：智能指针
来源：http://ek.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://uc.huixiangedu.cn

[S44] C++：引用传参
来源：http://tw.szsharing.cn

void inc(int &x) { ++x; }
来源：http://bq.asd995.cn

[S45] C++：lambda
来源：http://ib.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yd.wgjwhj.cn

[S46] C++：函数模板
来源：http://am.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cr.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://tv.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nl.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://gc.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pn.hahajie.cn

while (std::getline(in, line)) { }
来源：http://ww.szsharing.cn

[S49] C++：写文件
来源：http://do.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cd.panjiajie.cn

[S50] C++：格式化数字
来源：http://dt.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kh.newstarts.cn

[S51] C++：显式类型转换
来源：http://rm.chemitech.net.cn

static_cast<double>(a) / b
来源：http://dg.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://aq.hahajie.cn

int size() const noexcept { return n_; }
来源：http://pa.asd995.cn

[S53] C++：移动语义
来源：http://tf.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://gn.newstarts.cn

[S54] C++：异常处理
来源：http://aj.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uf.newstarts.cn

[S55] C++：结构化绑定
来源：http://hh.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fz.shxzskj.cn

[S56] C++：optional
来源：http://gf.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xj.yuexingan06.cn

[S57] C++：编译期常量
来源：http://id.huixiangedu.cn

constexpr int N = 10;
来源：http://xh.shxzukj.cn

[S58] C++：命名空间
来源：http://lo.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://yg.521024.cn

[S59] C++：静态断言
来源：http://ys.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zg.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://jo.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://li.jianghongdianzi.cn

================================================================================
来源：http://vq.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dn.bjjhwx.cn

================================================================================
来源：http://fe.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://uw.521024.cn

println("Hello")
来源：http://xq.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://ct.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ba.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://ta.nszjky.cn

"值: $b"
来源：http://jf.shxzukj.cn

[T04] Kotlin：空安全
来源：http://cq.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://sj.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://zc.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hm.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://is.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zv.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://nf.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jy.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://fg.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://od.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://po.521024.cn

fun String.exclaim() = this + "!"
来源：http://kh.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://hy.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fm.panjiajie.cn

[T11] Kotlin：协程
来源：http://nb.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mb.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://ab.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://fn.asd995.cn

[T13] Kotlin：只读 Map
来源：http://sx.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://gm.shtwfgs.cn

[T14] Kotlin：循环
来源：http://au.9csxet.cn

for (i in 1..10) println(i)
来源：http://ui.nicolike.cn

[T15] Kotlin：接口
来源：http://fs.szsharing.cn

interface Shape { fun area(): Double }
来源：http://yu.521024.cn

[T16] Swift：Hello World
来源：http://uc.bjjhwx.cn

print("Hello")
来源：http://lr.shxzskj.cn

[T17] Swift：变量与常量
来源：http://xz.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://vd.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://ss.nicolike.cn

"值: \(b)"
来源：http://ny.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://sa.nszjky.cn

if let n = opt { print(n) }
来源：http://lo.9csxet.cn

[T20] Swift：数组操作
来源：http://bw.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sm.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://qp.colortex.cn

for x in a { print(x) }
来源：http://en.huanxung.cn

[T22] Swift：字典
来源：http://vr.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kk.newstarts.cn

[T23] Swift：函数
来源：http://xt.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vq.huanxung.cn

[T24] Swift：闭包
来源：http://jr.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cm.colortex.cn

[T25] Swift：结构体
来源：http://uw.szxytkj.cn

struct P { var x: Int }
来源：http://ml.bjjhwx.cn

[T26] Swift：类与重写
来源：http://dd.newstarts.cn

class A: Base { override func f() {} }
来源：http://au.hnjuh.cn

[T27] Swift：错误处理
来源：http://ti.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://xr.huixiangedu.cn

[T28] Swift：枚举
来源：http://ae.521024.cn

enum Color { case red, green }
来源：http://kz.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://si.muxihuayi.cn

guard let x = opt else { return }
来源：http://fm.huixinmuqiang.cn

[T30] Swift：协议
来源：http://oq.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://oe.nszjky.cn

[T31] Lua：Hello World
来源：http://oq.haigaiapp.cn

print("Hello")
来源：http://fp.9csxet.cn

[T32] Lua：局部变量
来源：http://az.shxzskj.cn

local a = 1
来源：http://su.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://xw.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wi.newstarts.cn

[T34] Lua：遍历表
来源：http://kj.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://og.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://ys.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://wc.muxihuayi.cn

[T36] Lua：函数
来源：http://sf.huixiangedu.cn

function add(a, b) return a + b end
来源：http://wl.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://ts.nszjky.cn

"a" .. "b"
来源：http://ir.bookmarksfly.cn

[T38] Lua：条件
来源：http://zv.panjiajie.cn

if x > 0 then print("正") end
来源：http://hg.lnxyls.cn

[T39] Lua：模式匹配
来源：http://na.jctech888.com.cn

string.find(s, "%d+")
来源：http://is.bjjhwx.cn

[T40] Lua：元表
来源：http://bx.newstarts.cn

setmetatable({}, { __index = base })
来源：http://ut.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://ke.szxytkj.cn

print "Hello\n";
来源：http://pr.lnxyls.cn

[T42] Perl：变量类型
来源：http://vf.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://od.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://zh.9csxet.cn

"值: $a"
来源：http://vn.huixiangedu.cn

[T44] Perl：条件
来源：http://dd.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://tx.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://uo.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://lb.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://om.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rk.shxzskj.cn

[T47] Perl：正则捕获
来源：http://gx.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bg.haigaiapp.cn

[T48] Perl：正则替换
来源：http://gi.521024.cn

$s =~ s/old/new/g;
来源：http://tj.wgjwhj.cn

[T49] Perl：函数
来源：http://jc.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gn.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://qn.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uo.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://yw.muxihuayi.cn

[T51] Scala：Hello World
来源：http://wt.shxzskj.cn

println("Hello")
来源：http://kx.panjiajie.cn

[T52] Scala：变量
来源：http://dv.wgjwhj.cn

val a = 1;  var b = 2
来源：http://mg.hnjuh.cn

[T53] Scala：字符串插值
来源：http://rz.newstarts.cn

s"值: $b"
来源：http://ms.nszjky.cn

[T54] Scala：集合映射
来源：http://se.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://qk.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://yv.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://we.huanxung.cn

[T56] Scala：样例类
来源：http://yw.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://mp.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://hj.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://et.yuexingan06.cn

[T58] Scala：函数定义
来源：http://cv.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yc.9csxet.cn

[T59] Scala：循环
来源：http://qa.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://xg.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://qy.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://os.lnxyls.cn

================================================================================
来源：http://ag.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dc.gzmigu.cn

================================================================================
来源：http://rc.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://sm.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pb.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://zk.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hk.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://gh.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lw.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://ko.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nz.nszjky.cn

[U05] Py：列表去重且保序
来源：http://mz.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://of.colortex.cn

[U06] Py：合并两个字典
来源：http://xf.asd995.cn

{**a, **b}
来源：http://bj.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://te.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://sh.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://aa.hnjuh.cn

[y for x in nested for y in x]
来源：http://pd.colortex.cn

[U09] Py：字典取最大值的键
来源：http://zb.9csxet.cn

max(d, key=d.get)
来源：http://tp.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://he.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qa.shxzskj.cn

[U11] Py：生成器表达式
来源：http://va.shtwfgs.cn

(x * 2 for x in arr)
来源：http://ya.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ds.9csxet.cn

Counter(arr).most_common(3)
来源：http://gy.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://fj.lnxyls.cn

deque(maxlen=10)
来源：http://qt.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://wz.haigaiapp.cn

defaultdict(list)
来源：http://fh.huixiangedu.cn

[U15] Py：高精度计时
来源：http://ey.huanxung.cn

t = time.perf_counter()
来源：http://kh.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://il.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rd.gzmigu.cn

[U17] Py：初始化日志
来源：http://tx.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://ux.nicolike.cn

[U18] Py：预编译正则
来源：http://hz.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://es.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://gk.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bt.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://vh.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://pi.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://ic.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://cw.9csxet.cn

[U22] Py：矩阵转置
来源：http://zx.jctech888.com.cn

list(zip(*m))
来源：http://jt.nicolike.cn

[U23] Py：分块读取大文件
来源：http://sr.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fw.asd995.cn

[U24] Py：路径操作
来源：http://sl.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nm.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://qm.bjjhwx.cn

csv.DictReader(f)
来源：http://ka.shtwfgs.cn

[U26] Py：并发下载
来源：http://bn.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mz.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://wj.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://cv.521024.cn

[U28] Py：类型别名
来源：http://ri.wgjwhj.cn

UserId = int
来源：http://ml.521024.cn

[U29] Py：属性校验
来源：http://ff.colortex.cn

@property 与 @x.setter 配合
来源：http://xs.huanxung.cn

[U30] Py：数据类
来源：http://sn.yuexingan06.cn

@dataclass(slots=True)
来源：http://mi.gzmigu.cn

[U31] Py：单测
来源：http://vf.huanxung.cn

python -m pytest -q
来源：http://cx.bjjhwx.cn

[U32] Py：代码格式化
来源：http://za.521024.cn

ruff format . && ruff check --fix .
来源：http://qh.shxzskj.cn

[U33] Py：打包发布
来源：http://rv.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://kh.bjjhwx.cn

[U34] Py：判断编码
来源：http://xo.wgjwhj.cn

chardet.detect(raw)
来源：http://py.yuntaijiaju.cn


<!-- 参考信息 -->