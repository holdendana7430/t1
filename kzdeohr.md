代发 wailian999

x |= (1 << 3);
来源：http://ey.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://np.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://du.hnjuh.cn

[S18] C：命令行参数
来源：http://mp.bjjhwx.cn

int main(int argc, char **argv)
来源：http://oo.gzmigu.cn

[S19] C：快速排序
来源：http://wh.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://od.huanxung.cn

[S20] C：二分查找
来源：http://kc.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vc.jctech888.com.cn

[S21] C：字符类别判断
来源：http://wt.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mc.wgjwhj.cn

[S22] C：字符串转数字
来源：http://cq.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ce.colortex.cn

[S23] C：随机数
来源：http://ea.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ck.colortex.cn

[S24] C：获取本地时间
来源：http://bp.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ru.muxihuayi.cn

[S25] C：内存拷贝
来源：http://mf.hnjuh.cn

memcpy(dst, src, n);
来源：http://lz.huanxung.cn

[S26] C：内存清零
来源：http://xx.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://ad.jianghongdianzi.cn

[S27] C：定义常量
来源：http://nr.newstarts.cn

const double PI = 3.14159;
来源：http://qh.huixiangedu.cn

[S28] C：静态变量
来源：http://cx.colortex.cn

static int counter = 0;
来源：http://wv.szxytkj.cn

[S29] C：变参函数
来源：http://id.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zl.bjjhwx.cn

[S30] C：头文件保护
来源：http://qr.521024.cn

#ifndef X_H
来源：http://mm.huanxung.cn

#define X_H
来源：http://qh.hnjuh.cn

#endif
来源：http://wj.muxihuayi.cn

[S31] C++：Hello World
来源：http://jv.newstarts.cn

#include <iostream>
来源：http://nw.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://mh.jianghongdianzi.cn

[S32] C++：字符串
来源：http://wg.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://ad.asd995.cn

[S33] C++：vector 增删
来源：http://st.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://en.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://rb.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://sq.szsharing.cn

[S35] C++：map
来源：http://co.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vg.521024.cn

[S36] C++：unordered_map
来源：http://mx.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mc.jctech888.com.cn

[S37] C++：set
来源：http://dr.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gt.bookmarksfly.cn

[S38] C++：排序
来源：http://kg.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://mv.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://jj.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ny.521024.cn

[S40] C++：查找元素
来源：http://tm.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gk.521024.cn

[S41] C++：类与构造函数
来源：http://rb.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sa.hahajie.cn

[S42] C++：继承与虚函数
来源：http://da.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://uq.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://hn.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://wv.bookmarksfly.cn

[S44] C++：引用传参
来源：http://dg.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://xl.nicolike.cn

[S45] C++：lambda
来源：http://fv.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vx.521024.cn

[S46] C++：函数模板
来源：http://rd.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mz.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://pv.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qt.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://ht.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jd.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://mj.huanxung.cn

[S49] C++：写文件
来源：http://dd.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sc.panjiajie.cn

[S50] C++：格式化数字
来源：http://ms.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gt.9csxet.cn

[S51] C++：显式类型转换
来源：http://mb.lnxyls.cn

static_cast<double>(a) / b
来源：http://sh.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://nn.newstarts.cn

int size() const noexcept { return n_; }
来源：http://kn.yuexingan06.cn

[S53] C++：移动语义
来源：http://ra.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://um.shtwfgs.cn

[S54] C++：异常处理
来源：http://hb.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ue.nszjky.cn

[S55] C++：结构化绑定
来源：http://mo.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kv.muxihuayi.cn

[S56] C++：optional
来源：http://on.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ly.szsharing.cn

[S57] C++：编译期常量
来源：http://cc.jianghongdianzi.cn

constexpr int N = 10;
来源：http://fk.haigaiapp.cn

[S58] C++：命名空间
来源：http://so.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://ss.yuexingan06.cn

[S59] C++：静态断言
来源：http://lg.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rr.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://kb.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hf.521024.cn

================================================================================
来源：http://kq.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fm.shxzskj.cn

================================================================================
来源：http://fd.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://eg.asd995.cn

println("Hello")
来源：http://hc.panjiajie.cn

[T02] Kotlin：变量
来源：http://na.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://an.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://vl.shxzukj.cn

"值: $b"
来源：http://es.gzmigu.cn

[T04] Kotlin：空安全
来源：http://aw.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://tu.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://wd.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iz.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://st.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ua.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://ja.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zm.lnxyls.cn

[T08] Kotlin：数据类
来源：http://tw.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://eb.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://qf.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://og.szsharing.cn

[T10] Kotlin：默认参数
来源：http://du.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ul.jctech888.com.cn

[T11] Kotlin：协程
来源：http://rn.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hs.colortex.cn

[T12] Kotlin：解构声明
来源：http://ow.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://je.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://zu.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://sp.nicolike.cn

[T14] Kotlin：循环
来源：http://ng.panjiajie.cn

for (i in 1..10) println(i)
来源：http://rb.huixiangedu.cn

[T15] Kotlin：接口
来源：http://cn.nszjky.cn

interface Shape { fun area(): Double }
来源：http://vw.9csxet.cn

[T16] Swift：Hello World
来源：http://yb.shtwfgs.cn

print("Hello")
来源：http://hb.lnxyls.cn

[T17] Swift：变量与常量
来源：http://dm.shxzukj.cn

var a = 1;  let b = 2
来源：http://qd.gzmigu.cn

[T18] Swift：字符串插值
来源：http://ca.wgjwhj.cn

"值: \(b)"
来源：http://rk.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://dz.muxihuayi.cn

if let n = opt { print(n) }
来源：http://nb.colortex.cn

[T20] Swift：数组操作
来源：http://ui.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wg.shxzskj.cn

[T21] Swift：遍历
来源：http://zn.asd995.cn

for x in a { print(x) }
来源：http://tg.newstarts.cn

[T22] Swift：字典
来源：http://mo.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bf.jianghongdianzi.cn

[T23] Swift：函数
来源：http://af.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ok.haigaiapp.cn

[T24] Swift：闭包
来源：http://gn.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iv.wgjwhj.cn

[T25] Swift：结构体
来源：http://nx.huanxung.cn

struct P { var x: Int }
来源：http://ht.gzmigu.cn

[T26] Swift：类与重写
来源：http://lz.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://zs.521024.cn

[T27] Swift：错误处理
来源：http://na.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://pl.bookmarksfly.cn

[T28] Swift：枚举
来源：http://qa.jianghongdianzi.cn

enum Color { case red, green }
来源：http://lj.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://zc.wgjwhj.cn

guard let x = opt else { return }
来源：http://bz.lnxyls.cn

[T30] Swift：协议
来源：http://ly.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://nt.hahajie.cn

[T31] Lua：Hello World
来源：http://xe.muxihuayi.cn

print("Hello")
来源：http://je.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://nb.gzmigu.cn

local a = 1
来源：http://gk.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://na.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rr.gzmigu.cn

[T34] Lua：遍历表
来源：http://pr.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ut.nicolike.cn

[T35] Lua：字典表
来源：http://nk.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://ol.jianghongdianzi.cn

[T36] Lua：函数
来源：http://dc.shxzukj.cn

function add(a, b) return a + b end
来源：http://st.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://ah.muxihuayi.cn

"a" .. "b"
来源：http://fn.521024.cn

[T38] Lua：条件
来源：http://uy.lnxyls.cn

if x > 0 then print("正") end
来源：http://mt.huanxung.cn

[T39] Lua：模式匹配
来源：http://ii.jctech888.com.cn

string.find(s, "%d+")
来源：http://va.nicolike.cn

[T40] Lua：元表
来源：http://di.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://xp.shxzskj.cn

[T41] Perl：Hello World
来源：http://ix.huanxung.cn

print "Hello\n";
来源：http://zr.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://gw.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sy.szsharing.cn

[T43] Perl：字符串插值
来源：http://yb.bjjhwx.cn

"值: $a"
来源：http://pp.bjjhwx.cn

[T44] Perl：条件
来源：http://rk.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://kl.9csxet.cn

[T45] Perl：数组遍历
来源：http://jm.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://na.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://wj.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ax.nszjky.cn

[T47] Perl：正则捕获
来源：http://cm.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mo.lnxyls.cn

[T48] Perl：正则替换
来源：http://pk.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://xd.huixiangedu.cn

[T49] Perl：函数
来源：http://aa.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oi.nszjky.cn

[T50] Perl：逐行读文件
来源：http://uc.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rd.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://id.shtwfgs.cn

[T51] Scala：Hello World
来源：http://xi.chemitech.net.cn

println("Hello")
来源：http://uz.yuexingan06.cn

[T52] Scala：变量
来源：http://fs.haigaiapp.cn

val a = 1;  var b = 2
来源：http://jl.9csxet.cn

[T53] Scala：字符串插值
来源：http://hd.asd995.cn

s"值: $b"
来源：http://fp.haigaiapp.cn

[T54] Scala：集合映射
来源：http://wg.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://bk.nszjky.cn

[T55] Scala：集合过滤
来源：http://pt.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bx.panjiajie.cn

[T56] Scala：样例类
来源：http://yf.gzmigu.cn

case class User(name: String, age: Int)
来源：http://ug.nszjky.cn

[T57] Scala：模式匹配
来源：http://ay.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nh.szsharing.cn

[T58] Scala：函数定义
来源：http://vf.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://za.shtwfgs.cn

[T59] Scala：循环
来源：http://mg.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://bz.521024.cn

[T60] Scala：折叠
来源：http://uh.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zk.nszjky.cn

================================================================================
来源：http://ed.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://py.szxytkj.cn

================================================================================
来源：http://kg.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://pz.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ot.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://yw.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://de.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://nh.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mi.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://ck.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eb.colortex.cn

[U05] Py：列表去重且保序
来源：http://ym.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://ay.9csxet.cn

[U06] Py：合并两个字典
来源：http://er.gzmigu.cn

{**a, **b}
来源：http://qq.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://df.hahajie.cn

{v: k for k, v in d.items()}
来源：http://pk.shxzskj.cn

[U08] Py：展平二维列表
来源：http://hq.jctech888.com.cn

[y for x in nested for y in x]
来源：http://co.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://fx.newstarts.cn

max(d, key=d.get)
来源：http://uz.szsharing.cn

[U10] Py：按值排序字典
来源：http://ba.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kl.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://sj.hahajie.cn

(x * 2 for x in arr)
来源：http://uv.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ju.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://rd.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://fe.newstarts.cn

deque(maxlen=10)
来源：http://ku.nicolike.cn

[U14] Py：分组收集到列表
来源：http://xl.huixinmuqiang.cn

defaultdict(list)
来源：http://za.shtwfgs.cn

[U15] Py：高精度计时
来源：http://xh.wgjwhj.cn

t = time.perf_counter()
来源：http://nu.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://uc.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zo.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://xg.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://vd.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://iv.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://mj.huanxung.cn

[U19] Py：正则替换带回调
来源：http://ga.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yo.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://cp.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://og.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://rm.hnjuh.cn

@contextlib.contextmanager
来源：http://xc.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://zi.huixiangedu.cn

list(zip(*m))
来源：http://ey.asd995.cn

[U23] Py：分块读取大文件
来源：http://dd.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ix.nszjky.cn

[U24] Py：路径操作
来源：http://vn.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zp.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://ax.shxzskj.cn

csv.DictReader(f)
来源：http://cn.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://gn.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ps.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://sq.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://tz.shtwfgs.cn

[U28] Py：类型别名
来源：http://be.haigaiapp.cn

UserId = int
来源：http://yn.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://gl.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://be.shxzskj.cn

[U30] Py：数据类
来源：http://ra.521024.cn

@dataclass(slots=True)
来源：http://ih.wgjwhj.cn

[U31] Py：单测
来源：http://wm.gzmigu.cn

python -m pytest -q
来源：http://ap.lnxyls.cn

[U32] Py：代码格式化
来源：http://op.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://lo.asd995.cn

[U33] Py：打包发布
来源：http://oh.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://wk.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://cd.haigaiapp.cn

chardet.detect(raw)
来源：http://gk.yuexingan06.cn

[U35] Py：发送邮件
来源：http://bo.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tg.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://yq.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://iv.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://vd.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ud.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://oc.521024.cn

Path(__file__).resolve().parent
来源：http://zo.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://bt.gzmigu.cn

sys.stdout.isatty()
来源：http://fo.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://gc.shxzukj.cn

print("err", file=sys.stderr)
来源：http://de.wgjwhj.cn


<!-- 参考信息 -->