代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mq.nszjky.cn

[S13] C：宏定义
来源：http://qa.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pz.lnxyls.cn

[S14] C：枚举
来源：http://bz.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://oi.haigaiapp.cn

[S15] C：类型转换
来源：http://kp.lnxyls.cn

(double) a / b
来源：http://dj.colortex.cn

[S16] C：位操作置位
来源：http://wm.jctech888.com.cn

x |= (1 << 3);
来源：http://ag.nszjky.cn

[S17] C：安全拼接字符串
来源：http://uq.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vc.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://mm.huanxung.cn

int main(int argc, char **argv)
来源：http://kg.shxzskj.cn

[S19] C：快速排序
来源：http://xe.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kn.9csxet.cn

[S20] C：二分查找
来源：http://ge.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sy.bjjhwx.cn

[S21] C：字符类别判断
来源：http://iq.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qe.muxihuayi.cn

[S22] C：字符串转数字
来源：http://ox.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qn.nszjky.cn

[S23] C：随机数
来源：http://fs.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ge.521024.cn

[S24] C：获取本地时间
来源：http://ud.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cp.hnjuh.cn

[S25] C：内存拷贝
来源：http://bg.szsharing.cn

memcpy(dst, src, n);
来源：http://yu.bjjhwx.cn

[S26] C：内存清零
来源：http://qi.521024.cn

memset(a, 0, sizeof a);
来源：http://kr.shtwfgs.cn

[S27] C：定义常量
来源：http://dt.szsharing.cn

const double PI = 3.14159;
来源：http://rk.gzmigu.cn

[S28] C：静态变量
来源：http://ws.chemitech.net.cn

static int counter = 0;
来源：http://tg.nszjky.cn

[S29] C：变参函数
来源：http://rz.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oc.chemitech.net.cn

[S30] C：头文件保护
来源：http://vh.asd995.cn

#ifndef X_H
来源：http://fa.lnxyls.cn

#define X_H
来源：http://jg.huixiangedu.cn

#endif
来源：http://ng.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://ya.szxytkj.cn

#include <iostream>
来源：http://fa.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://rd.huixinmuqiang.cn

[S32] C++：字符串
来源：http://ab.521024.cn

std::string s = "hi";  s += "!";
来源：http://ky.shtwfgs.cn

[S33] C++：vector 增删
来源：http://qs.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uo.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://ma.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://ho.lnxyls.cn

[S35] C++：map
来源：http://ju.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fd.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://vu.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dh.gzmigu.cn

[S37] C++：set
来源：http://oi.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vl.hahajie.cn

[S38] C++：排序
来源：http://kj.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://tn.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://wh.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dj.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://zr.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sf.nicolike.cn

[S41] C++：类与构造函数
来源：http://xg.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vz.nszjky.cn

[S42] C++：继承与虚函数
来源：http://rh.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://dz.huanxung.cn

[S43] C++：智能指针
来源：http://gd.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://ja.szsharing.cn

[S44] C++：引用传参
来源：http://qk.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://qn.shxzukj.cn

[S45] C++：lambda
来源：http://fu.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ib.muxihuayi.cn

[S46] C++：函数模板
来源：http://mt.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gs.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://tp.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ot.gzmigu.cn

[S48] C++：逐行读文件
来源：http://ah.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xq.huanxung.cn

while (std::getline(in, line)) { }
来源：http://pw.jctech888.com.cn

[S49] C++：写文件
来源：http://mn.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kc.chemitech.net.cn

[S50] C++：格式化数字
来源：http://bb.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vt.szsharing.cn

[S51] C++：显式类型转换
来源：http://aa.shxzukj.cn

static_cast<double>(a) / b
来源：http://dw.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://dq.521024.cn

int size() const noexcept { return n_; }
来源：http://go.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://hn.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://ta.colortex.cn

[S54] C++：异常处理
来源：http://dv.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jl.gzmigu.cn

[S55] C++：结构化绑定
来源：http://nb.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cb.hnjuh.cn

[S56] C++：optional
来源：http://ga.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ev.hnjuh.cn

[S57] C++：编译期常量
来源：http://tf.shxzskj.cn

constexpr int N = 10;
来源：http://al.bookmarksfly.cn

[S58] C++：命名空间
来源：http://ce.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://xz.panjiajie.cn

[S59] C++：静态断言
来源：http://zo.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rv.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://hk.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ul.hnjuh.cn

================================================================================
来源：http://im.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fl.jctech888.com.cn

================================================================================
来源：http://ca.9csxet.cn

[T01] Kotlin：Hello World
来源：http://sx.lnxyls.cn

println("Hello")
来源：http://yy.hahajie.cn

[T02] Kotlin：变量
来源：http://xr.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cz.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://uk.bjjhwx.cn

"值: $b"
来源：http://uz.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://hb.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://ge.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://jd.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://km.521024.cn

[T06] Kotlin：集合映射
来源：http://zl.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tf.huixinmuqiang.cn

[T07] Kotlin：集合过滤
来源：http://qv.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yb.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://ls.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://de.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://gt.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://nv.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://qg.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wt.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://ex.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dz.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://yd.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://tf.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://fr.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://vi.hnjuh.cn

[T14] Kotlin：循环
来源：http://bs.gzmigu.cn

for (i in 1..10) println(i)
来源：http://xm.9csxet.cn

[T15] Kotlin：接口
来源：http://dx.szsharing.cn

interface Shape { fun area(): Double }
来源：http://ti.yuexingan06.cn

[T16] Swift：Hello World
来源：http://zb.9csxet.cn

print("Hello")
来源：http://nh.panjiajie.cn

[T17] Swift：变量与常量
来源：http://xt.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://af.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://ct.asd995.cn

"值: \(b)"
来源：http://zh.huanxung.cn

[T19] Swift：可选绑定
来源：http://gd.newstarts.cn

if let n = opt { print(n) }
来源：http://rp.colortex.cn

[T20] Swift：数组操作
来源：http://mb.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nn.521024.cn

[T21] Swift：遍历
来源：http://fz.chemitech.net.cn

for x in a { print(x) }
来源：http://jp.huanxung.cn

[T22] Swift：字典
来源：http://ve.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rw.wgjwhj.cn

[T23] Swift：函数
来源：http://xi.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oc.521024.cn

[T24] Swift：闭包
来源：http://wj.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bo.szxytkj.cn

[T25] Swift：结构体
来源：http://yv.hahajie.cn

struct P { var x: Int }
来源：http://lw.panjiajie.cn

[T26] Swift：类与重写
来源：http://nh.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://ex.hnjuh.cn

[T27] Swift：错误处理
来源：http://hw.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://qt.hahajie.cn

[T28] Swift：枚举
来源：http://ib.hnjuh.cn

enum Color { case red, green }
来源：http://oi.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://hq.lnxyls.cn

guard let x = opt else { return }
来源：http://cy.shxzskj.cn

[T30] Swift：协议
来源：http://sb.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://tx.huixiangedu.cn

[T31] Lua：Hello World
来源：http://py.shxzukj.cn

print("Hello")
来源：http://ct.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://ik.yuntaijiaju.cn

local a = 1
来源：http://sm.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://vm.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pk.panjiajie.cn

[T34] Lua：遍历表
来源：http://of.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yo.colortex.cn

[T35] Lua：字典表
来源：http://ft.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://tg.9csxet.cn

[T36] Lua：函数
来源：http://ol.yuexingan06.cn

function add(a, b) return a + b end
来源：http://hf.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://dv.521024.cn

"a" .. "b"
来源：http://kf.yuexingan06.cn

[T38] Lua：条件
来源：http://ru.521024.cn

if x > 0 then print("正") end
来源：http://vb.9csxet.cn

[T39] Lua：模式匹配
来源：http://nw.521024.cn

string.find(s, "%d+")
来源：http://rn.panjiajie.cn

[T40] Lua：元表
来源：http://go.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://xm.521024.cn

[T41] Perl：Hello World
来源：http://lt.hahajie.cn

print "Hello\n";
来源：http://cq.jctech888.com.cn

[T42] Perl：变量类型
来源：http://zz.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zk.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://qi.nicolike.cn

"值: $a"
来源：http://bk.bjjhwx.cn

[T44] Perl：条件
来源：http://an.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://jd.gzmigu.cn

[T45] Perl：数组遍历
来源：http://ft.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://vq.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://cp.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://in.gzmigu.cn

[T47] Perl：正则捕获
来源：http://wm.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pq.bjjhwx.cn

[T48] Perl：正则替换
来源：http://fn.hahajie.cn

$s =~ s/old/new/g;
来源：http://ku.wgjwhj.cn

[T49] Perl：函数
来源：http://hv.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pd.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://ep.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pi.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://aa.szxytkj.cn

[T51] Scala：Hello World
来源：http://ln.asd995.cn

println("Hello")
来源：http://jo.szxytkj.cn

[T52] Scala：变量
来源：http://vm.shtwfgs.cn

val a = 1;  var b = 2
来源：http://xl.colortex.cn

[T53] Scala：字符串插值
来源：http://wy.521024.cn

s"值: $b"
来源：http://ac.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://os.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://db.hnjuh.cn

[T55] Scala：集合过滤
来源：http://it.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ck.newstarts.cn

[T56] Scala：样例类
来源：http://me.hnjuh.cn

case class User(name: String, age: Int)
来源：http://is.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://sk.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gm.panjiajie.cn

[T58] Scala：函数定义
来源：http://ny.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ib.9csxet.cn

[T59] Scala：循环
来源：http://kz.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://lr.bookmarksfly.cn

[T60] Scala：折叠
来源：http://ee.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ly.szxytkj.cn

================================================================================
来源：http://ke.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ft.shxzukj.cn

================================================================================
来源：http://wg.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://gv.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yp.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://dm.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iu.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://ku.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kv.huanxung.cn

[U04] Py：变量调试打印
来源：http://yj.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://is.nszjky.cn

[U05] Py：列表去重且保序
来源：http://hi.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://nr.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://yd.chemitech.net.cn

{**a, **b}
来源：http://sp.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://ey.nszjky.cn

{v: k for k, v in d.items()}
来源：http://lz.panjiajie.cn

[U08] Py：展平二维列表
来源：http://kf.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://yo.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://dl.bookmarksfly.cn

max(d, key=d.get)
来源：http://jz.shxzskj.cn

[U10] Py：按值排序字典
来源：http://xm.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://no.nszjky.cn

[U11] Py：生成器表达式
来源：http://ns.wgjwhj.cn

(x * 2 for x in arr)
来源：http://sy.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hu.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://wg.szsharing.cn

[U13] Py：固定长度队列
来源：http://fd.nicolike.cn

deque(maxlen=10)
来源：http://wv.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://uh.nszjky.cn

defaultdict(list)
来源：http://yi.yuexingan06.cn

[U15] Py：高精度计时
来源：http://sm.chemitech.net.cn

t = time.perf_counter()
来源：http://km.asd995.cn

[U16] Py：命令行参数解析
来源：http://zv.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://us.gzmigu.cn

[U17] Py：初始化日志
来源：http://km.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://tc.colortex.cn

[U18] Py：预编译正则
来源：http://lg.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://md.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://se.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nv.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://gi.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://wv.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://zc.bookmarksfly.cn

@contextlib.contextmanager
来源：http://sk.szxytkj.cn

[U22] Py：矩阵转置
来源：http://tz.bjjhwx.cn

list(zip(*m))
来源：http://op.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://gq.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zy.muxihuayi.cn

[U24] Py：路径操作
来源：http://gj.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gp.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://np.jctech888.com.cn

csv.DictReader(f)
来源：http://mg.colortex.cn

[U26] Py：并发下载
来源：http://kk.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uc.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://hf.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://zn.huanxung.cn

[U28] Py：类型别名
来源：http://qm.newstarts.cn

UserId = int
来源：http://qz.asd995.cn

[U29] Py：属性校验
来源：http://kh.szsharing.cn

@property 与 @x.setter 配合
来源：http://on.huixinmuqiang.cn

[U30] Py：数据类
来源：http://de.panjiajie.cn

@dataclass(slots=True)
来源：http://dg.newstarts.cn

[U31] Py：单测
来源：http://yr.muxihuayi.cn

python -m pytest -q
来源：http://bj.shxzskj.cn

[U32] Py：代码格式化
来源：http://pf.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://qe.shtwfgs.cn

[U33] Py：打包发布
来源：http://mp.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://sn.lnxyls.cn

[U34] Py：判断编码
来源：http://jw.yuexingan06.cn

chardet.detect(raw)
来源：http://ey.wgjwhj.cn

[U35] Py：发送邮件
来源：http://oi.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dc.szxytkj.cn

[U36] Py：定时任务
来源：http://so.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://lr.shxzskj.cn


<!-- 参考信息 -->