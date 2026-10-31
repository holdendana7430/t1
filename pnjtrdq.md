代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://to.bookmarksfly.cn

[S15] C：类型转换
来源：http://ik.muxihuayi.cn

(double) a / b
来源：http://zi.yuexingan06.cn

[S16] C：位操作置位
来源：http://qw.chemitech.net.cn

x |= (1 << 3);
来源：http://oj.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://ou.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ho.colortex.cn

[S18] C：命令行参数
来源：http://fb.shxzukj.cn

int main(int argc, char **argv)
来源：http://os.bjjhwx.cn

[S19] C：快速排序
来源：http://rt.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mt.shxzskj.cn

[S20] C：二分查找
来源：http://di.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yy.nszjky.cn

[S21] C：字符类别判断
来源：http://su.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tz.haigaiapp.cn

[S22] C：字符串转数字
来源：http://sg.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kp.hahajie.cn

[S23] C：随机数
来源：http://cd.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cw.hnjuh.cn

[S24] C：获取本地时间
来源：http://ie.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wr.huanxung.cn

[S25] C：内存拷贝
来源：http://zs.yuexingan06.cn

memcpy(dst, src, n);
来源：http://yj.9csxet.cn

[S26] C：内存清零
来源：http://jy.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://ht.hnjuh.cn

[S27] C：定义常量
来源：http://jh.nszjky.cn

const double PI = 3.14159;
来源：http://hr.nszjky.cn

[S28] C：静态变量
来源：http://dg.huixiangedu.cn

static int counter = 0;
来源：http://vj.gzmigu.cn

[S29] C：变参函数
来源：http://xl.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://al.muxihuayi.cn

[S30] C：头文件保护
来源：http://cc.panjiajie.cn

#ifndef X_H
来源：http://zm.lnxyls.cn

#define X_H
来源：http://bu.9csxet.cn

#endif
来源：http://ox.colortex.cn

[S31] C++：Hello World
来源：http://lc.haigaiapp.cn

#include <iostream>
来源：http://il.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://ct.haigaiapp.cn

[S32] C++：字符串
来源：http://if.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://uz.lnxyls.cn

[S33] C++：vector 增删
来源：http://ng.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xi.szxytkj.cn

[S34] C++：遍历 vector
来源：http://ps.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://fg.hnjuh.cn

[S35] C++：map
来源：http://ln.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ah.colortex.cn

[S36] C++：unordered_map
来源：http://zx.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://km.yuntaijiaju.cn

[S37] C++：set
来源：http://vv.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jc.asd995.cn

[S38] C++：排序
来源：http://og.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://wc.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://xk.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qz.bjjhwx.cn

[S40] C++：查找元素
来源：http://df.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://um.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://pa.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gg.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://kg.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://yv.521024.cn

[S43] C++：智能指针
来源：http://bj.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://ym.bookmarksfly.cn

[S44] C++：引用传参
来源：http://vb.nicolike.cn

void inc(int &x) { ++x; }
来源：http://gk.bjjhwx.cn

[S45] C++：lambda
来源：http://xb.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sj.shtwfgs.cn

[S46] C++：函数模板
来源：http://pt.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ot.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://pe.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yp.lnxyls.cn

[S48] C++：逐行读文件
来源：http://iv.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jr.nicolike.cn

while (std::getline(in, line)) { }
来源：http://gr.bookmarksfly.cn

[S49] C++：写文件
来源：http://ab.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uq.jctech888.com.cn

[S50] C++：格式化数字
来源：http://ho.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eu.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://bw.shxzskj.cn

static_cast<double>(a) / b
来源：http://wg.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://ai.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://ez.bjjhwx.cn

[S53] C++：移动语义
来源：http://ei.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://mh.nszjky.cn

[S54] C++：异常处理
来源：http://fm.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pg.szxytkj.cn

[S55] C++：结构化绑定
来源：http://lq.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jg.shxzskj.cn

[S56] C++：optional
来源：http://jm.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vk.hahajie.cn

[S57] C++：编译期常量
来源：http://kh.wgjwhj.cn

constexpr int N = 10;
来源：http://it.nicolike.cn

[S58] C++：命名空间
来源：http://yu.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://wr.chemitech.net.cn

[S59] C++：静态断言
来源：http://qf.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://md.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://lx.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cc.shxzukj.cn

================================================================================
来源：http://fo.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gy.nicolike.cn

================================================================================
来源：http://mk.521024.cn

[T01] Kotlin：Hello World
来源：http://qq.shxzskj.cn

println("Hello")
来源：http://xa.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://ue.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ry.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://wm.colortex.cn

"值: $b"
来源：http://am.panjiajie.cn

[T04] Kotlin：空安全
来源：http://be.nicolike.cn

val n: String? = null;  n?.length
来源：http://vz.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://et.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ks.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://yn.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qk.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://ti.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://os.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://tn.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://dn.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://tn.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://iv.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://pw.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cg.wgjwhj.cn

[T11] Kotlin：协程
来源：http://sv.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ru.asd995.cn

[T12] Kotlin：解构声明
来源：http://zd.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://vt.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://br.hahajie.cn

val m = mapOf("a" to 1)
来源：http://dt.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://tk.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://rj.huanxung.cn

[T15] Kotlin：接口
来源：http://ms.colortex.cn

interface Shape { fun area(): Double }
来源：http://mb.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://xm.wgjwhj.cn

print("Hello")
来源：http://xq.shxzukj.cn

[T17] Swift：变量与常量
来源：http://he.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://qu.szxytkj.cn

[T18] Swift：字符串插值
来源：http://lw.bjjhwx.cn

"值: \(b)"
来源：http://jm.shxzukj.cn

[T19] Swift：可选绑定
来源：http://cn.wgjwhj.cn

if let n = opt { print(n) }
来源：http://kp.bjjhwx.cn

[T20] Swift：数组操作
来源：http://xw.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uc.bookmarksfly.cn

[T21] Swift：遍历
来源：http://oo.jianghongdianzi.cn

for x in a { print(x) }
来源：http://nu.newstarts.cn

[T22] Swift：字典
来源：http://cm.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ks.jctech888.com.cn

[T23] Swift：函数
来源：http://im.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ld.nicolike.cn

[T24] Swift：闭包
来源：http://hp.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://el.shxzskj.cn

[T25] Swift：结构体
来源：http://jb.hahajie.cn

struct P { var x: Int }
来源：http://cf.newstarts.cn

[T26] Swift：类与重写
来源：http://gr.nicolike.cn

class A: Base { override func f() {} }
来源：http://si.haigaiapp.cn

[T27] Swift：错误处理
来源：http://ak.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://nl.lnxyls.cn

[T28] Swift：枚举
来源：http://dn.huixinmuqiang.cn

enum Color { case red, green }
来源：http://ky.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://pc.shxzskj.cn

guard let x = opt else { return }
来源：http://qo.lnxyls.cn

[T30] Swift：协议
来源：http://fr.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://kp.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://na.521024.cn

print("Hello")
来源：http://nu.muxihuayi.cn

[T32] Lua：局部变量
来源：http://dz.haigaiapp.cn

local a = 1
来源：http://db.newstarts.cn

[T33] Lua：表（数组）
来源：http://mi.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qb.colortex.cn

[T34] Lua：遍历表
来源：http://ul.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fa.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://pr.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://ip.bjjhwx.cn

[T36] Lua：函数
来源：http://gq.shxzskj.cn

function add(a, b) return a + b end
来源：http://le.asd995.cn

[T37] Lua：字符串拼接
来源：http://ah.chemitech.net.cn

"a" .. "b"
来源：http://cj.nicolike.cn

[T38] Lua：条件
来源：http://xh.newstarts.cn

if x > 0 then print("正") end
来源：http://af.shxzskj.cn

[T39] Lua：模式匹配
来源：http://it.lnxyls.cn

string.find(s, "%d+")
来源：http://au.szsharing.cn

[T40] Lua：元表
来源：http://jy.hahajie.cn

setmetatable({}, { __index = base })
来源：http://rk.newstarts.cn

[T41] Perl：Hello World
来源：http://kp.jctech888.com.cn

print "Hello\n";
来源：http://nm.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://qn.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://op.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://el.szsharing.cn

"值: $a"
来源：http://fn.hnjuh.cn

[T44] Perl：条件
来源：http://sn.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://bj.szsharing.cn

[T45] Perl：数组遍历
来源：http://hr.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://na.colortex.cn

[T46] Perl：哈希操作
来源：http://tk.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jq.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://ey.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xm.haigaiapp.cn

[T48] Perl：正则替换
来源：http://rg.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://ke.nicolike.cn

[T49] Perl：函数
来源：http://kt.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kn.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://ln.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fz.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://ec.bjjhwx.cn

[T51] Scala：Hello World
来源：http://nk.shxzukj.cn

println("Hello")
来源：http://jp.newstarts.cn

[T52] Scala：变量
来源：http://rd.nszjky.cn

val a = 1;  var b = 2
来源：http://pv.huanxung.cn

[T53] Scala：字符串插值
来源：http://hi.yuexingan06.cn

s"值: $b"
来源：http://dh.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://cc.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://nk.huanxung.cn

[T55] Scala：集合过滤
来源：http://iz.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hq.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://wu.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://nm.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://ue.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xy.colortex.cn

[T58] Scala：函数定义
来源：http://gn.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yz.9csxet.cn

[T59] Scala：循环
来源：http://wo.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://zh.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://wx.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vm.bjjhwx.cn

================================================================================
来源：http://tg.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dg.huanxung.cn

================================================================================
来源：http://mg.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://ij.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zs.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://qc.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kh.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://ic.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qi.gzmigu.cn

[U04] Py：变量调试打印
来源：http://jq.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ww.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://vx.huanxung.cn

list(dict.fromkeys(arr))
来源：http://nm.szxytkj.cn

[U06] Py：合并两个字典
来源：http://gf.jianghongdianzi.cn

{**a, **b}
来源：http://wc.9csxet.cn

[U07] Py：反转字典键值
来源：http://al.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://ay.shxzukj.cn

[U08] Py：展平二维列表
来源：http://bn.chemitech.net.cn

[y for x in nested for y in x]
来源：http://zm.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://vf.panjiajie.cn

max(d, key=d.get)
来源：http://qi.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://ej.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ui.gzmigu.cn

[U11] Py：生成器表达式
来源：http://pd.shtwfgs.cn

(x * 2 for x in arr)
来源：http://mg.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lm.9csxet.cn

Counter(arr).most_common(3)
来源：http://lg.hnjuh.cn

[U13] Py：固定长度队列
来源：http://az.muxihuayi.cn

deque(maxlen=10)
来源：http://gy.nszjky.cn

[U14] Py：分组收集到列表
来源：http://vc.shxzskj.cn

defaultdict(list)
来源：http://ih.jctech888.com.cn

[U15] Py：高精度计时
来源：http://qv.muxihuayi.cn

t = time.perf_counter()
来源：http://ct.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://lq.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kv.colortex.cn

[U17] Py：初始化日志
来源：http://bd.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://tb.shxzskj.cn

[U18] Py：预编译正则
来源：http://tl.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://qp.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://uv.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ly.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://um.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://rk.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://kw.colortex.cn

@contextlib.contextmanager
来源：http://ji.gzmigu.cn

[U22] Py：矩阵转置
来源：http://hf.haigaiapp.cn

list(zip(*m))
来源：http://ma.521024.cn

[U23] Py：分块读取大文件
来源：http://ed.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uz.colortex.cn

[U24] Py：路径操作
来源：http://om.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oy.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://ym.huixinmuqiang.cn

csv.DictReader(f)
来源：http://ww.newstarts.cn

[U26] Py：并发下载
来源：http://sr.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uw.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://th.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://km.gzmigu.cn

[U28] Py：类型别名
来源：http://au.bookmarksfly.cn

UserId = int
来源：http://ud.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://bd.shxzukj.cn

@property 与 @x.setter 配合
来源：http://za.yuexingan06.cn

[U30] Py：数据类
来源：http://ph.shxzukj.cn

@dataclass(slots=True)
来源：http://ds.shxzskj.cn

[U31] Py：单测
来源：http://ah.9csxet.cn

python -m pytest -q
来源：http://ww.asd995.cn

[U32] Py：代码格式化
来源：http://fq.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://yt.hahajie.cn

[U33] Py：打包发布
来源：http://oh.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://ow.yuexingan06.cn

[U34] Py：判断编码
来源：http://bd.panjiajie.cn

chardet.detect(raw)
来源：http://yr.bjjhwx.cn

[U35] Py：发送邮件
来源：http://nv.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ox.shxzukj.cn

[U36] Py：定时任务
来源：http://ok.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://in.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://rx.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jp.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://bj.colortex.cn

Path(__file__).resolve().parent
来源：http://op.hnjuh.cn


<!-- 参考信息 -->