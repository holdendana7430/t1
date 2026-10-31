代发 wailian999

x |= (1 << 3);
来源：http://de.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://ac.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nf.9csxet.cn

[S18] C：命令行参数
来源：http://zx.huanxung.cn

int main(int argc, char **argv)
来源：http://zk.bookmarksfly.cn

[S19] C：快速排序
来源：http://hl.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sj.wgjwhj.cn

[S20] C：二分查找
来源：http://nd.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ft.shxzukj.cn

[S21] C：字符类别判断
来源：http://sx.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lj.huixiangedu.cn

[S22] C：字符串转数字
来源：http://vf.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wb.huixiangedu.cn

[S23] C：随机数
来源：http://ak.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://am.muxihuayi.cn

[S24] C：获取本地时间
来源：http://je.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ge.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://do.haigaiapp.cn

memcpy(dst, src, n);
来源：http://qh.yuntaijiaju.cn

[S26] C：内存清零
来源：http://fb.nicolike.cn

memset(a, 0, sizeof a);
来源：http://qg.shxzskj.cn

[S27] C：定义常量
来源：http://cn.shxzskj.cn

const double PI = 3.14159;
来源：http://nw.shtwfgs.cn

[S28] C：静态变量
来源：http://ai.shxzukj.cn

static int counter = 0;
来源：http://cc.jctech888.com.cn

[S29] C：变参函数
来源：http://lf.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mo.yuexingan06.cn

[S30] C：头文件保护
来源：http://is.hnjuh.cn

#ifndef X_H
来源：http://hq.521024.cn

#define X_H
来源：http://ta.newstarts.cn

#endif
来源：http://kq.newstarts.cn

[S31] C++：Hello World
来源：http://hj.shxzskj.cn

#include <iostream>
来源：http://bt.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://gw.huixiangedu.cn

[S32] C++：字符串
来源：http://ok.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://tn.jctech888.com.cn

[S33] C++：vector 增删
来源：http://fm.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sd.huanxung.cn

[S34] C++：遍历 vector
来源：http://az.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://gu.huanxung.cn

[S35] C++：map
来源：http://wt.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qw.shxzukj.cn

[S36] C++：unordered_map
来源：http://fp.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jv.yuexingan06.cn

[S37] C++：set
来源：http://zp.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zg.bookmarksfly.cn

[S38] C++：排序
来源：http://vl.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://bh.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://eg.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bk.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://ll.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bh.hnjuh.cn

[S41] C++：类与构造函数
来源：http://cr.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ca.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://fv.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://bu.chemitech.net.cn

[S43] C++：智能指针
来源：http://ak.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://yd.521024.cn

[S44] C++：引用传参
来源：http://mc.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://hz.jctech888.com.cn

[S45] C++：lambda
来源：http://gm.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fx.colortex.cn

[S46] C++：函数模板
来源：http://tq.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kq.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://zg.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rm.szsharing.cn

[S48] C++：逐行读文件
来源：http://qb.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ej.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://ma.jianghongdianzi.cn

[S49] C++：写文件
来源：http://fo.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ik.panjiajie.cn

[S50] C++：格式化数字
来源：http://pt.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://be.shxzukj.cn

[S51] C++：显式类型转换
来源：http://fs.muxihuayi.cn

static_cast<double>(a) / b
来源：http://nr.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://nf.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://lg.shxzskj.cn

[S53] C++：移动语义
来源：http://kx.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://ik.bookmarksfly.cn

[S54] C++：异常处理
来源：http://kn.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zt.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://br.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://so.newstarts.cn

[S56] C++：optional
来源：http://en.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rp.nicolike.cn

[S57] C++：编译期常量
来源：http://hz.huixinmuqiang.cn

constexpr int N = 10;
来源：http://fh.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://pe.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://kt.asd995.cn

[S59] C++：静态断言
来源：http://rl.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jz.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://ev.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ve.szxytkj.cn

================================================================================
来源：http://gm.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xj.521024.cn

================================================================================
来源：http://fx.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://rr.gzmigu.cn

println("Hello")
来源：http://yk.jctech888.com.cn

[T02] Kotlin：变量
来源：http://kj.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pz.521024.cn

[T03] Kotlin：字符串模板
来源：http://uj.panjiajie.cn

"值: $b"
来源：http://ea.szxytkj.cn

[T04] Kotlin：空安全
来源：http://co.hnjuh.cn

val n: String? = null;  n?.length
来源：http://pj.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://ak.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qc.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://qy.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ug.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://oe.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gs.nicolike.cn

[T08] Kotlin：数据类
来源：http://gd.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://lz.521024.cn

[T09] Kotlin：扩展函数
来源：http://br.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://fv.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://tl.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wm.panjiajie.cn

[T11] Kotlin：协程
来源：http://dx.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ju.asd995.cn

[T12] Kotlin：解构声明
来源：http://uf.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://fk.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://dq.huanxung.cn

val m = mapOf("a" to 1)
来源：http://nm.hahajie.cn

[T14] Kotlin：循环
来源：http://qd.huanxung.cn

for (i in 1..10) println(i)
来源：http://pz.colortex.cn

[T15] Kotlin：接口
来源：http://tz.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://ro.szxytkj.cn

[T16] Swift：Hello World
来源：http://eg.huanxung.cn

print("Hello")
来源：http://js.lnxyls.cn

[T17] Swift：变量与常量
来源：http://xu.asd995.cn

var a = 1;  let b = 2
来源：http://ud.nicolike.cn

[T18] Swift：字符串插值
来源：http://oq.nicolike.cn

"值: \(b)"
来源：http://mr.szxytkj.cn

[T19] Swift：可选绑定
来源：http://nx.gzmigu.cn

if let n = opt { print(n) }
来源：http://gb.newstarts.cn

[T20] Swift：数组操作
来源：http://he.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qu.521024.cn

[T21] Swift：遍历
来源：http://wl.shxzukj.cn

for x in a { print(x) }
来源：http://yr.panjiajie.cn

[T22] Swift：字典
来源：http://vt.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zd.bjjhwx.cn

[T23] Swift：函数
来源：http://ov.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cd.wgjwhj.cn

[T24] Swift：闭包
来源：http://zx.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://se.shtwfgs.cn

[T25] Swift：结构体
来源：http://tt.szxytkj.cn

struct P { var x: Int }
来源：http://ki.szsharing.cn

[T26] Swift：类与重写
来源：http://fh.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://hg.shxzukj.cn

[T27] Swift：错误处理
来源：http://dm.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://oy.gzmigu.cn

[T28] Swift：枚举
来源：http://bx.jctech888.com.cn

enum Color { case red, green }
来源：http://ub.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://pf.asd995.cn

guard let x = opt else { return }
来源：http://hs.panjiajie.cn

[T30] Swift：协议
来源：http://dy.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://bl.asd995.cn

[T31] Lua：Hello World
来源：http://wi.chemitech.net.cn

print("Hello")
来源：http://ww.asd995.cn

[T32] Lua：局部变量
来源：http://eo.newstarts.cn

local a = 1
来源：http://ru.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://tj.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pz.yuexingan06.cn

[T34] Lua：遍历表
来源：http://tc.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uo.asd995.cn

[T35] Lua：字典表
来源：http://fa.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://gy.szxytkj.cn

[T36] Lua：函数
来源：http://aw.hnjuh.cn

function add(a, b) return a + b end
来源：http://tf.asd995.cn

[T37] Lua：字符串拼接
来源：http://jp.hnjuh.cn

"a" .. "b"
来源：http://of.nszjky.cn

[T38] Lua：条件
来源：http://rw.colortex.cn

if x > 0 then print("正") end
来源：http://et.panjiajie.cn

[T39] Lua：模式匹配
来源：http://ne.jctech888.com.cn

string.find(s, "%d+")
来源：http://nf.szsharing.cn

[T40] Lua：元表
来源：http://gg.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://sl.gzmigu.cn

[T41] Perl：Hello World
来源：http://kl.nszjky.cn

print "Hello\n";
来源：http://ad.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://ot.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rj.asd995.cn

[T43] Perl：字符串插值
来源：http://tx.jctech888.com.cn

"值: $a"
来源：http://ha.panjiajie.cn

[T44] Perl：条件
来源：http://lg.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://xn.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://ta.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://xu.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://ac.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zh.9csxet.cn

[T47] Perl：正则捕获
来源：http://ih.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wc.wgjwhj.cn

[T48] Perl：正则替换
来源：http://ok.9csxet.cn

$s =~ s/old/new/g;
来源：http://pw.asd995.cn

[T49] Perl：函数
来源：http://oj.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cj.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://co.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://re.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://br.chemitech.net.cn

[T51] Scala：Hello World
来源：http://uc.nicolike.cn

println("Hello")
来源：http://hv.jctech888.com.cn

[T52] Scala：变量
来源：http://ne.haigaiapp.cn

val a = 1;  var b = 2
来源：http://ih.asd995.cn

[T53] Scala：字符串插值
来源：http://oe.szxytkj.cn

s"值: $b"
来源：http://px.jctech888.com.cn

[T54] Scala：集合映射
来源：http://xw.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://rf.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://hp.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cg.haigaiapp.cn

[T56] Scala：样例类
来源：http://dg.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://us.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://xn.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://od.hahajie.cn

[T58] Scala：函数定义
来源：http://fw.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ib.panjiajie.cn

[T59] Scala：循环
来源：http://bu.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://lx.bjjhwx.cn

[T60] Scala：折叠
来源：http://js.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lb.huixinmuqiang.cn

================================================================================
来源：http://iy.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fz.huanxung.cn

================================================================================
来源：http://fh.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://ly.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gr.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://mv.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lz.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://et.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gr.shxzukj.cn

[U04] Py：变量调试打印
来源：http://oi.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qk.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://ow.szsharing.cn

list(dict.fromkeys(arr))
来源：http://fz.9csxet.cn

[U06] Py：合并两个字典
来源：http://gj.9csxet.cn

{**a, **b}
来源：http://ja.huanxung.cn

[U07] Py：反转字典键值
来源：http://bn.hahajie.cn

{v: k for k, v in d.items()}
来源：http://wb.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://yt.9csxet.cn

[y for x in nested for y in x]
来源：http://vx.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://tz.szxytkj.cn

max(d, key=d.get)
来源：http://rn.shxzskj.cn

[U10] Py：按值排序字典
来源：http://cw.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tk.hnjuh.cn

[U11] Py：生成器表达式
来源：http://sx.asd995.cn

(x * 2 for x in arr)
来源：http://uc.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://df.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://ne.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://aw.chemitech.net.cn

deque(maxlen=10)
来源：http://zg.nszjky.cn

[U14] Py：分组收集到列表
来源：http://um.nszjky.cn

defaultdict(list)
来源：http://dm.bjjhwx.cn

[U15] Py：高精度计时
来源：http://nq.colortex.cn

t = time.perf_counter()
来源：http://cr.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://qx.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ew.gzmigu.cn

[U17] Py：初始化日志
来源：http://zv.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://wr.hnjuh.cn

[U18] Py：预编译正则
来源：http://kn.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://ls.nicolike.cn

[U19] Py：正则替换带回调
来源：http://cn.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dr.szsharing.cn

[U20] Py：缓存函数结果
来源：http://xh.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://dn.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://oq.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://ia.huanxung.cn

[U22] Py：矩阵转置
来源：http://yb.huanxung.cn

list(zip(*m))
来源：http://au.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://cn.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xo.muxihuayi.cn

[U24] Py：路径操作
来源：http://fg.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ue.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://xt.shxzukj.cn

csv.DictReader(f)
来源：http://mq.nicolike.cn

[U26] Py：并发下载
来源：http://iz.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ht.nszjky.cn

[U27] Py：异步 HTTP
来源：http://px.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://fa.hnjuh.cn

[U28] Py：类型别名
来源：http://mr.nicolike.cn

UserId = int
来源：http://bb.panjiajie.cn

[U29] Py：属性校验
来源：http://ld.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://zk.shxzukj.cn

[U30] Py：数据类
来源：http://hz.asd995.cn

@dataclass(slots=True)
来源：http://sb.nicolike.cn

[U31] Py：单测
来源：http://xm.nicolike.cn

python -m pytest -q
来源：http://qh.shtwfgs.cn

[U32] Py：代码格式化
来源：http://op.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://rr.bjjhwx.cn

[U33] Py：打包发布
来源：http://rp.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://cd.huixiangedu.cn

[U34] Py：判断编码
来源：http://nt.jianghongdianzi.cn

chardet.detect(raw)
来源：http://ss.chemitech.net.cn

[U35] Py：发送邮件
来源：http://yo.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jp.bookmarksfly.cn

[U36] Py：定时任务
来源：http://ro.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://jn.521024.cn

[U37] Py：读写 Excel
来源：http://xa.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mw.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://dn.gzmigu.cn

Path(__file__).resolve().parent
来源：http://pl.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://bc.szsharing.cn

sys.stdout.isatty()
来源：http://pd.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://lr.hnjuh.cn

print("err", file=sys.stderr)
来源：http://nb.shtwfgs.cn


<!-- 参考信息 -->