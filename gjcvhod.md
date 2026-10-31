代发 wailian999

x |= (1 << 3);
来源：http://pa.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://by.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uj.nicolike.cn

[S18] C：命令行参数
来源：http://cj.huixiangedu.cn

int main(int argc, char **argv)
来源：http://wj.yuntaijiaju.cn

[S19] C：快速排序
来源：http://ri.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qk.colortex.cn

[S20] C：二分查找
来源：http://ju.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mh.asd995.cn

[S21] C：字符类别判断
来源：http://ed.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eu.shxzskj.cn

[S22] C：字符串转数字
来源：http://wz.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xl.wgjwhj.cn

[S23] C：随机数
来源：http://eq.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tl.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://cz.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pn.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://ku.asd995.cn

memcpy(dst, src, n);
来源：http://od.haigaiapp.cn

[S26] C：内存清零
来源：http://mm.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://bq.jctech888.com.cn

[S27] C：定义常量
来源：http://vd.9csxet.cn

const double PI = 3.14159;
来源：http://ie.huixiangedu.cn

[S28] C：静态变量
来源：http://ag.huanxung.cn

static int counter = 0;
来源：http://rg.huixiangedu.cn

[S29] C：变参函数
来源：http://bg.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ro.haigaiapp.cn

[S30] C：头文件保护
来源：http://nv.huanxung.cn

#ifndef X_H
来源：http://ch.asd995.cn

#define X_H
来源：http://gt.newstarts.cn

#endif
来源：http://rk.521024.cn

[S31] C++：Hello World
来源：http://aj.huixinmuqiang.cn

#include <iostream>
来源：http://qd.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://px.shxzukj.cn

[S32] C++：字符串
来源：http://la.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://mf.panjiajie.cn

[S33] C++：vector 增删
来源：http://gx.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://he.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://ok.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://iu.colortex.cn

[S35] C++：map
来源：http://wy.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jw.haigaiapp.cn

[S36] C++：unordered_map
来源：http://ob.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xw.gzmigu.cn

[S37] C++：set
来源：http://tx.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jj.panjiajie.cn

[S38] C++：排序
来源：http://fi.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://ed.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://lt.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xp.newstarts.cn

[S40] C++：查找元素
来源：http://tj.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://un.hnjuh.cn

[S41] C++：类与构造函数
来源：http://ds.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lf.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://lg.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://sm.bjjhwx.cn

[S43] C++：智能指针
来源：http://gh.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://hb.jctech888.com.cn

[S44] C++：引用传参
来源：http://yr.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://ku.lnxyls.cn

[S45] C++：lambda
来源：http://ab.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jy.huixiangedu.cn

[S46] C++：函数模板
来源：http://rh.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pf.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://uq.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qa.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://zn.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tv.szsharing.cn

while (std::getline(in, line)) { }
来源：http://wd.chemitech.net.cn

[S49] C++：写文件
来源：http://bk.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ia.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://av.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qc.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://nh.521024.cn

static_cast<double>(a) / b
来源：http://vb.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://zd.nicolike.cn

int size() const noexcept { return n_; }
来源：http://kr.szsharing.cn

[S53] C++：移动语义
来源：http://fv.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://iv.hnjuh.cn

[S54] C++：异常处理
来源：http://ga.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nd.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://wh.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zl.wgjwhj.cn

[S56] C++：optional
来源：http://rs.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://go.nszjky.cn

[S57] C++：编译期常量
来源：http://rf.newstarts.cn

constexpr int N = 10;
来源：http://xf.asd995.cn

[S58] C++：命名空间
来源：http://gz.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://iz.shxzskj.cn

[S59] C++：静态断言
来源：http://ww.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://my.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://xq.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kg.lnxyls.cn

================================================================================
来源：http://ej.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ys.colortex.cn

================================================================================
来源：http://ub.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://kd.haigaiapp.cn

println("Hello")
来源：http://di.nicolike.cn

[T02] Kotlin：变量
来源：http://ak.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lq.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://ht.asd995.cn

"值: $b"
来源：http://sa.9csxet.cn

[T04] Kotlin：空安全
来源：http://fd.huanxung.cn

val n: String? = null;  n?.length
来源：http://of.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://sl.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ll.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://am.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kf.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://rc.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tb.panjiajie.cn

[T08] Kotlin：数据类
来源：http://oi.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://rx.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://yt.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://uf.521024.cn

[T10] Kotlin：默认参数
来源：http://vx.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://va.9csxet.cn

[T11] Kotlin：协程
来源：http://ff.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fs.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://mn.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://wu.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://kd.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://dd.newstarts.cn

[T14] Kotlin：循环
来源：http://jh.newstarts.cn

for (i in 1..10) println(i)
来源：http://ui.lnxyls.cn

[T15] Kotlin：接口
来源：http://ii.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://ej.chemitech.net.cn

[T16] Swift：Hello World
来源：http://pb.gzmigu.cn

print("Hello")
来源：http://dh.gzmigu.cn

[T17] Swift：变量与常量
来源：http://sz.szxytkj.cn

var a = 1;  let b = 2
来源：http://ad.panjiajie.cn

[T18] Swift：字符串插值
来源：http://ta.lnxyls.cn

"值: \(b)"
来源：http://hb.shxzskj.cn

[T19] Swift：可选绑定
来源：http://rv.nszjky.cn

if let n = opt { print(n) }
来源：http://ev.wgjwhj.cn

[T20] Swift：数组操作
来源：http://lu.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ig.panjiajie.cn

[T21] Swift：遍历
来源：http://vi.gzmigu.cn

for x in a { print(x) }
来源：http://sq.muxihuayi.cn

[T22] Swift：字典
来源：http://si.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://he.jctech888.com.cn

[T23] Swift：函数
来源：http://dn.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mo.shtwfgs.cn

[T24] Swift：闭包
来源：http://gm.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lr.yuexingan06.cn

[T25] Swift：结构体
来源：http://cv.chemitech.net.cn

struct P { var x: Int }
来源：http://dn.szsharing.cn

[T26] Swift：类与重写
来源：http://bb.szsharing.cn

class A: Base { override func f() {} }
来源：http://na.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://ee.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://us.newstarts.cn

[T28] Swift：枚举
来源：http://ae.shxzukj.cn

enum Color { case red, green }
来源：http://wb.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://yb.chemitech.net.cn

guard let x = opt else { return }
来源：http://qy.bjjhwx.cn

[T30] Swift：协议
来源：http://me.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://nr.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://qx.panjiajie.cn

print("Hello")
来源：http://wf.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://jc.521024.cn

local a = 1
来源：http://fw.hnjuh.cn

[T33] Lua：表（数组）
来源：http://om.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lq.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://zj.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vk.521024.cn

[T35] Lua：字典表
来源：http://fy.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://fx.nicolike.cn

[T36] Lua：函数
来源：http://tk.9csxet.cn

function add(a, b) return a + b end
来源：http://je.colortex.cn

[T37] Lua：字符串拼接
来源：http://aj.szxytkj.cn

"a" .. "b"
来源：http://js.szsharing.cn

[T38] Lua：条件
来源：http://po.9csxet.cn

if x > 0 then print("正") end
来源：http://if.521024.cn

[T39] Lua：模式匹配
来源：http://lk.shxzskj.cn

string.find(s, "%d+")
来源：http://xu.szxytkj.cn

[T40] Lua：元表
来源：http://ln.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://ew.szsharing.cn

[T41] Perl：Hello World
来源：http://gt.gzmigu.cn

print "Hello\n";
来源：http://fa.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://cc.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ed.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://vd.nszjky.cn

"值: $a"
来源：http://jo.bjjhwx.cn

[T44] Perl：条件
来源：http://bk.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://md.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://jd.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://bb.hahajie.cn

[T46] Perl：哈希操作
来源：http://pr.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xv.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://vx.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wh.jctech888.com.cn

[T48] Perl：正则替换
来源：http://sm.shxzskj.cn

$s =~ s/old/new/g;
来源：http://zc.shxzukj.cn

[T49] Perl：函数
来源：http://ag.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mk.asd995.cn

[T50] Perl：逐行读文件
来源：http://vq.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://js.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://bg.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://wh.colortex.cn

println("Hello")
来源：http://oj.nicolike.cn

[T52] Scala：变量
来源：http://ib.jctech888.com.cn

val a = 1;  var b = 2
来源：http://zo.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://nx.hahajie.cn

s"值: $b"
来源：http://uv.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://wx.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://xl.521024.cn

[T55] Scala：集合过滤
来源：http://ux.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tg.jctech888.com.cn

[T56] Scala：样例类
来源：http://jy.asd995.cn

case class User(name: String, age: Int)
来源：http://dd.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://jh.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kl.huanxung.cn

[T58] Scala：函数定义
来源：http://xo.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://og.panjiajie.cn

[T59] Scala：循环
来源：http://qv.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://dq.shxzskj.cn

[T60] Scala：折叠
来源：http://is.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yj.bookmarksfly.cn

================================================================================
来源：http://wt.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gd.bookmarksfly.cn

================================================================================
来源：http://na.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://gu.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ww.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://na.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sw.colortex.cn

[U03] Py：加载 .env 配置
来源：http://fy.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xa.shxzukj.cn

[U04] Py：变量调试打印
来源：http://gp.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sm.nszjky.cn

[U05] Py：列表去重且保序
来源：http://sq.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://rt.gzmigu.cn

[U06] Py：合并两个字典
来源：http://qq.panjiajie.cn

{**a, **b}
来源：http://hb.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://mi.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://qk.lnxyls.cn

[U08] Py：展平二维列表
来源：http://yz.szxytkj.cn

[y for x in nested for y in x]
来源：http://qe.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://om.nszjky.cn

max(d, key=d.get)
来源：http://lj.szsharing.cn

[U10] Py：按值排序字典
来源：http://cv.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qm.asd995.cn

[U11] Py：生成器表达式
来源：http://ur.nicolike.cn

(x * 2 for x in arr)
来源：http://ym.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://py.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://jp.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://jp.shxzukj.cn

deque(maxlen=10)
来源：http://ik.newstarts.cn

[U14] Py：分组收集到列表
来源：http://qc.huixiangedu.cn

defaultdict(list)
来源：http://cv.shtwfgs.cn

[U15] Py：高精度计时
来源：http://qt.shxzskj.cn

t = time.perf_counter()
来源：http://xf.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://ft.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uv.lnxyls.cn

[U17] Py：初始化日志
来源：http://ih.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://ph.newstarts.cn

[U18] Py：预编译正则
来源：http://gk.nicolike.cn

pat = re.compile(r"\d+")
来源：http://vb.hahajie.cn

[U19] Py：正则替换带回调
来源：http://dm.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ju.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://cb.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://br.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://xy.muxihuayi.cn

@contextlib.contextmanager
来源：http://kd.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://yp.szsharing.cn

list(zip(*m))
来源：http://ju.asd995.cn

[U23] Py：分块读取大文件
来源：http://js.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pl.yuexingan06.cn

[U24] Py：路径操作
来源：http://tv.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rv.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://vq.bookmarksfly.cn

csv.DictReader(f)
来源：http://vn.bjjhwx.cn

[U26] Py：并发下载
来源：http://fx.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rv.asd995.cn

[U27] Py：异步 HTTP
来源：http://dn.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://kw.shtwfgs.cn

[U28] Py：类型别名
来源：http://su.newstarts.cn

UserId = int
来源：http://uq.chemitech.net.cn

[U29] Py：属性校验
来源：http://qo.9csxet.cn

@property 与 @x.setter 配合
来源：http://gi.colortex.cn

[U30] Py：数据类
来源：http://uy.wgjwhj.cn

@dataclass(slots=True)
来源：http://fi.huixinmuqiang.cn

[U31] Py：单测
来源：http://nj.bookmarksfly.cn

python -m pytest -q
来源：http://bh.muxihuayi.cn

[U32] Py：代码格式化
来源：http://hb.asd995.cn

ruff format . && ruff check --fix .
来源：http://mz.hahajie.cn

[U33] Py：打包发布
来源：http://rr.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://yi.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://yd.wgjwhj.cn

chardet.detect(raw)
来源：http://cb.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://la.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ls.hnjuh.cn

[U36] Py：定时任务
来源：http://vx.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://kd.nszjky.cn

[U37] Py：读写 Excel
来源：http://ih.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://og.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://vp.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://bq.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://xx.wgjwhj.cn

sys.stdout.isatty()
来源：http://ih.nszjky.cn

[U40] Py：打印到标准错误
来源：http://ns.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://ce.hnjuh.cn


<!-- 参考信息 -->