代发 wailian999

x |= (1 << 3);
来源：http://ll.asd995.cn

[S17] C：安全拼接字符串
来源：http://as.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wi.haigaiapp.cn

[S18] C：命令行参数
来源：http://gy.9csxet.cn

int main(int argc, char **argv)
来源：http://cj.newstarts.cn

[S19] C：快速排序
来源：http://js.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tw.wgjwhj.cn

[S20] C：二分查找
来源：http://qq.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cp.jctech888.com.cn

[S21] C：字符类别判断
来源：http://zh.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eb.huanxung.cn

[S22] C：字符串转数字
来源：http://yx.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ac.521024.cn

[S23] C：随机数
来源：http://eg.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hm.nicolike.cn

[S24] C：获取本地时间
来源：http://uv.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ia.bjjhwx.cn

[S25] C：内存拷贝
来源：http://ly.szsharing.cn

memcpy(dst, src, n);
来源：http://ug.bookmarksfly.cn

[S26] C：内存清零
来源：http://dk.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://us.yuexingan06.cn

[S27] C：定义常量
来源：http://cl.szxytkj.cn

const double PI = 3.14159;
来源：http://hz.panjiajie.cn

[S28] C：静态变量
来源：http://dd.hahajie.cn

static int counter = 0;
来源：http://qq.gzmigu.cn

[S29] C：变参函数
来源：http://ih.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sw.haigaiapp.cn

[S30] C：头文件保护
来源：http://ic.9csxet.cn

#ifndef X_H
来源：http://fp.hnjuh.cn

#define X_H
来源：http://zd.wgjwhj.cn

#endif
来源：http://nd.jctech888.com.cn

[S31] C++：Hello World
来源：http://yx.bookmarksfly.cn

#include <iostream>
来源：http://je.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ow.yuntaijiaju.cn

[S32] C++：字符串
来源：http://mp.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://ru.panjiajie.cn

[S33] C++：vector 增删
来源：http://gv.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ss.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://cx.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://jg.szxytkj.cn

[S35] C++：map
来源：http://rg.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ph.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://qj.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gv.nicolike.cn

[S37] C++：set
来源：http://uw.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://he.lnxyls.cn

[S38] C++：排序
来源：http://ws.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://xh.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://rw.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qy.szxytkj.cn

[S40] C++：查找元素
来源：http://lm.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://is.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://ek.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://am.hahajie.cn

[S42] C++：继承与虚函数
来源：http://su.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://yh.huanxung.cn

[S43] C++：智能指针
来源：http://gb.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://br.haigaiapp.cn

[S44] C++：引用传参
来源：http://nv.colortex.cn

void inc(int &x) { ++x; }
来源：http://of.bookmarksfly.cn

[S45] C++：lambda
来源：http://hd.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://so.bookmarksfly.cn

[S46] C++：函数模板
来源：http://ty.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bm.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://nc.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ja.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://zv.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zv.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://oj.shxzskj.cn

[S49] C++：写文件
来源：http://bd.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ug.yuexingan06.cn

[S50] C++：格式化数字
来源：http://hc.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pt.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://eq.hnjuh.cn

static_cast<double>(a) / b
来源：http://mt.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://dp.521024.cn

int size() const noexcept { return n_; }
来源：http://kk.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://tb.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://ru.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://bz.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xq.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://ax.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cp.haigaiapp.cn

[S56] C++：optional
来源：http://et.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ag.newstarts.cn

[S57] C++：编译期常量
来源：http://mf.shxzukj.cn

constexpr int N = 10;
来源：http://gg.asd995.cn

[S58] C++：命名空间
来源：http://ff.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://jc.hnjuh.cn

[S59] C++：静态断言
来源：http://bo.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wd.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://rg.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bu.jctech888.com.cn

================================================================================
来源：http://et.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uz.newstarts.cn

================================================================================
来源：http://up.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://wd.yuexingan06.cn

println("Hello")
来源：http://bq.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://uv.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gl.asd995.cn

[T03] Kotlin：字符串模板
来源：http://po.lnxyls.cn

"值: $b"
来源：http://pi.newstarts.cn

[T04] Kotlin：空安全
来源：http://ah.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://kn.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://xx.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ly.hahajie.cn

[T06] Kotlin：集合映射
来源：http://ih.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eu.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://ms.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qd.nicolike.cn

[T08] Kotlin：数据类
来源：http://cr.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://zw.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://mb.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://uh.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://jn.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wo.nicolike.cn

[T11] Kotlin：协程
来源：http://ok.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gn.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://bh.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://jb.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://fu.nicolike.cn

val m = mapOf("a" to 1)
来源：http://ev.szsharing.cn

[T14] Kotlin：循环
来源：http://rn.9csxet.cn

for (i in 1..10) println(i)
来源：http://em.chemitech.net.cn

[T15] Kotlin：接口
来源：http://fw.521024.cn

interface Shape { fun area(): Double }
来源：http://tr.9csxet.cn

[T16] Swift：Hello World
来源：http://ob.lnxyls.cn

print("Hello")
来源：http://uu.huanxung.cn

[T17] Swift：变量与常量
来源：http://xr.nszjky.cn

var a = 1;  let b = 2
来源：http://ni.asd995.cn

[T18] Swift：字符串插值
来源：http://fq.shtwfgs.cn

"值: \(b)"
来源：http://uc.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://mt.newstarts.cn

if let n = opt { print(n) }
来源：http://xo.shxzukj.cn

[T20] Swift：数组操作
来源：http://fy.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cp.muxihuayi.cn

[T21] Swift：遍历
来源：http://ez.bookmarksfly.cn

for x in a { print(x) }
来源：http://vw.panjiajie.cn

[T22] Swift：字典
来源：http://hw.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fl.521024.cn

[T23] Swift：函数
来源：http://lq.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gs.bookmarksfly.cn

[T24] Swift：闭包
来源：http://if.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://au.shxzskj.cn

[T25] Swift：结构体
来源：http://mz.muxihuayi.cn

struct P { var x: Int }
来源：http://hw.asd995.cn

[T26] Swift：类与重写
来源：http://ff.shxzskj.cn

class A: Base { override func f() {} }
来源：http://qk.shxzukj.cn

[T27] Swift：错误处理
来源：http://lv.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://kr.huanxung.cn

[T28] Swift：枚举
来源：http://qj.muxihuayi.cn

enum Color { case red, green }
来源：http://qn.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://br.shxzskj.cn

guard let x = opt else { return }
来源：http://kw.shxzskj.cn

[T30] Swift：协议
来源：http://zo.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://mg.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://db.haigaiapp.cn

print("Hello")
来源：http://pi.chemitech.net.cn

[T32] Lua：局部变量
来源：http://na.jianghongdianzi.cn

local a = 1
来源：http://mb.lnxyls.cn

[T33] Lua：表（数组）
来源：http://eb.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wn.chemitech.net.cn

[T34] Lua：遍历表
来源：http://cv.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jy.hahajie.cn

[T35] Lua：字典表
来源：http://gb.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://af.gzmigu.cn

[T36] Lua：函数
来源：http://ft.shxzukj.cn

function add(a, b) return a + b end
来源：http://jo.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://pi.bookmarksfly.cn

"a" .. "b"
来源：http://ev.szxytkj.cn

[T38] Lua：条件
来源：http://lr.hnjuh.cn

if x > 0 then print("正") end
来源：http://pk.9csxet.cn

[T39] Lua：模式匹配
来源：http://uv.yuexingan06.cn

string.find(s, "%d+")
来源：http://se.huixinmuqiang.cn

[T40] Lua：元表
来源：http://jv.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://do.9csxet.cn

[T41] Perl：Hello World
来源：http://fb.bookmarksfly.cn

print "Hello\n";
来源：http://jb.szxytkj.cn

[T42] Perl：变量类型
来源：http://sx.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dg.lnxyls.cn

[T43] Perl：字符串插值
来源：http://yn.panjiajie.cn

"值: $a"
来源：http://jq.haigaiapp.cn

[T44] Perl：条件
来源：http://vr.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://mt.lnxyls.cn

[T45] Perl：数组遍历
来源：http://br.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://db.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://pr.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ea.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://kx.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wn.bjjhwx.cn

[T48] Perl：正则替换
来源：http://im.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://jz.szsharing.cn

[T49] Perl：函数
来源：http://bm.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mh.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://jo.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fq.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://ed.huixiangedu.cn

[T51] Scala：Hello World
来源：http://gi.haigaiapp.cn

println("Hello")
来源：http://ca.bjjhwx.cn

[T52] Scala：变量
来源：http://yt.colortex.cn

val a = 1;  var b = 2
来源：http://nb.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://gx.huixiangedu.cn

s"值: $b"
来源：http://rk.nicolike.cn

[T54] Scala：集合映射
来源：http://nh.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://mo.nicolike.cn

[T55] Scala：集合过滤
来源：http://nh.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rm.shtwfgs.cn

[T56] Scala：样例类
来源：http://gv.huanxung.cn

case class User(name: String, age: Int)
来源：http://ib.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://ak.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sy.wgjwhj.cn

[T58] Scala：函数定义
来源：http://ko.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fk.521024.cn

[T59] Scala：循环
来源：http://ff.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://tb.shtwfgs.cn

[T60] Scala：折叠
来源：http://cd.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zv.haigaiapp.cn

================================================================================
来源：http://jl.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fh.shtwfgs.cn

================================================================================
来源：http://qc.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://yb.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ry.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://ws.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yg.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://rh.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dz.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://yu.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://la.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://yp.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://rd.asd995.cn

[U06] Py：合并两个字典
来源：http://dx.lnxyls.cn

{**a, **b}
来源：http://oi.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://ig.521024.cn

{v: k for k, v in d.items()}
来源：http://ez.panjiajie.cn

[U08] Py：展平二维列表
来源：http://wm.colortex.cn

[y for x in nested for y in x]
来源：http://kr.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://uu.bookmarksfly.cn

max(d, key=d.get)
来源：http://ll.panjiajie.cn

[U10] Py：按值排序字典
来源：http://yp.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rn.szxytkj.cn

[U11] Py：生成器表达式
来源：http://pf.lnxyls.cn

(x * 2 for x in arr)
来源：http://dt.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://aj.nszjky.cn

Counter(arr).most_common(3)
来源：http://ws.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://ki.gzmigu.cn

deque(maxlen=10)
来源：http://nu.nicolike.cn

[U14] Py：分组收集到列表
来源：http://gu.hahajie.cn

defaultdict(list)
来源：http://sf.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://hf.yuexingan06.cn

t = time.perf_counter()
来源：http://xo.9csxet.cn

[U16] Py：命令行参数解析
来源：http://ng.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yz.shtwfgs.cn

[U17] Py：初始化日志
来源：http://nn.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://ef.hnjuh.cn

[U18] Py：预编译正则
来源：http://lq.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://sd.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://go.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zm.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://vg.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://oz.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://vb.bjjhwx.cn

@contextlib.contextmanager
来源：http://nr.hnjuh.cn

[U22] Py：矩阵转置
来源：http://sb.hahajie.cn

list(zip(*m))
来源：http://we.asd995.cn

[U23] Py：分块读取大文件
来源：http://ov.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://po.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://nc.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nn.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://qp.nszjky.cn

csv.DictReader(f)
来源：http://oa.szsharing.cn

[U26] Py：并发下载
来源：http://cw.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ge.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://ue.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://vq.gzmigu.cn

[U28] Py：类型别名
来源：http://qp.hahajie.cn

UserId = int
来源：http://qk.shtwfgs.cn

[U29] Py：属性校验
来源：http://ls.lnxyls.cn

@property 与 @x.setter 配合
来源：http://pv.wgjwhj.cn

[U30] Py：数据类
来源：http://bs.hahajie.cn

@dataclass(slots=True)
来源：http://mr.hahajie.cn

[U31] Py：单测
来源：http://az.bookmarksfly.cn

python -m pytest -q
来源：http://pj.asd995.cn

[U32] Py：代码格式化
来源：http://wq.szsharing.cn

ruff format . && ruff check --fix .
来源：http://tw.nszjky.cn

[U33] Py：打包发布
来源：http://gk.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://pz.newstarts.cn

[U34] Py：判断编码
来源：http://vs.9csxet.cn

chardet.detect(raw)
来源：http://rq.szsharing.cn

[U35] Py：发送邮件
来源：http://zt.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qy.yuexingan06.cn

[U36] Py：定时任务
来源：http://jb.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://bo.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://vb.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qv.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://jc.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://la.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://kn.nicolike.cn

sys.stdout.isatty()
来源：http://on.newstarts.cn

[U40] Py：打印到标准错误
来源：http://ya.shxzukj.cn

print("err", file=sys.stderr)
来源：http://hl.bookmarksfly.cn


<!-- 参考信息 -->