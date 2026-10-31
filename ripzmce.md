代发 wailian999

x |= (1 << 3);
来源：http://fn.colortex.cn

[S17] C：安全拼接字符串
来源：http://lf.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rj.huanxung.cn

[S18] C：命令行参数
来源：http://wh.521024.cn

int main(int argc, char **argv)
来源：http://gf.wgjwhj.cn

[S19] C：快速排序
来源：http://an.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sp.nicolike.cn

[S20] C：二分查找
来源：http://gq.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://if.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://zw.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sa.szsharing.cn

[S22] C：字符串转数字
来源：http://ua.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dl.jctech888.com.cn

[S23] C：随机数
来源：http://jb.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://my.huixiangedu.cn

[S24] C：获取本地时间
来源：http://nu.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vl.nicolike.cn

[S25] C：内存拷贝
来源：http://ne.hahajie.cn

memcpy(dst, src, n);
来源：http://we.haigaiapp.cn

[S26] C：内存清零
来源：http://lr.nszjky.cn

memset(a, 0, sizeof a);
来源：http://dh.gzmigu.cn

[S27] C：定义常量
来源：http://km.muxihuayi.cn

const double PI = 3.14159;
来源：http://nf.huanxung.cn

[S28] C：静态变量
来源：http://me.jianghongdianzi.cn

static int counter = 0;
来源：http://ht.huixiangedu.cn

[S29] C：变参函数
来源：http://rp.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://in.bjjhwx.cn

[S30] C：头文件保护
来源：http://ww.asd995.cn

#ifndef X_H
来源：http://os.yuexingan06.cn

#define X_H
来源：http://ho.chemitech.net.cn

#endif
来源：http://zx.521024.cn

[S31] C++：Hello World
来源：http://ts.jctech888.com.cn

#include <iostream>
来源：http://su.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://qg.chemitech.net.cn

[S32] C++：字符串
来源：http://bf.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://ry.yuexingan06.cn

[S33] C++：vector 增删
来源：http://bq.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ug.nicolike.cn

[S34] C++：遍历 vector
来源：http://jm.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://te.gzmigu.cn

[S35] C++：map
来源：http://sa.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ce.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://rc.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qc.9csxet.cn

[S37] C++：set
来源：http://pk.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qv.shxzskj.cn

[S38] C++：排序
来源：http://ue.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://bl.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://oa.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ow.shtwfgs.cn

[S40] C++：查找元素
来源：http://wh.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cn.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://bo.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lz.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://dr.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://ed.nicolike.cn

[S43] C++：智能指针
来源：http://ty.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://ii.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://ya.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://qx.hahajie.cn

[S45] C++：lambda
来源：http://nq.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lt.szsharing.cn

[S46] C++：函数模板
来源：http://kn.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bh.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://pt.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://st.nicolike.cn

[S48] C++：逐行读文件
来源：http://bf.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bj.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://uq.panjiajie.cn

[S49] C++：写文件
来源：http://sy.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ad.asd995.cn

[S50] C++：格式化数字
来源：http://su.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oc.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://lt.szxytkj.cn

static_cast<double>(a) / b
来源：http://gc.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://rt.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://eq.9csxet.cn

[S53] C++：移动语义
来源：http://kw.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://xw.shxzukj.cn

[S54] C++：异常处理
来源：http://ge.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rt.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://zb.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oc.bjjhwx.cn

[S56] C++：optional
来源：http://nn.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jq.gzmigu.cn

[S57] C++：编译期常量
来源：http://dj.shtwfgs.cn

constexpr int N = 10;
来源：http://jx.shxzskj.cn

[S58] C++：命名空间
来源：http://px.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://am.nszjky.cn

[S59] C++：静态断言
来源：http://ap.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vp.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://py.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sa.nszjky.cn

================================================================================
来源：http://zt.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nn.asd995.cn

================================================================================
来源：http://ey.asd995.cn

[T01] Kotlin：Hello World
来源：http://vc.asd995.cn

println("Hello")
来源：http://tz.newstarts.cn

[T02] Kotlin：变量
来源：http://eq.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mv.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://tk.hahajie.cn

"值: $b"
来源：http://bd.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://fl.nicolike.cn

val n: String? = null;  n?.length
来源：http://sx.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://qf.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yx.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://qy.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tu.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://ze.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xm.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://pg.colortex.cn

data class User(val name: String, val age: Int)
来源：http://zc.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://br.asd995.cn

fun String.exclaim() = this + "!"
来源：http://wt.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://qp.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jn.shxzukj.cn

[T11] Kotlin：协程
来源：http://jc.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://az.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://ua.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://ug.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://xm.nszjky.cn

val m = mapOf("a" to 1)
来源：http://fq.shxzskj.cn

[T14] Kotlin：循环
来源：http://iv.hnjuh.cn

for (i in 1..10) println(i)
来源：http://gh.newstarts.cn

[T15] Kotlin：接口
来源：http://ur.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://uu.lnxyls.cn

[T16] Swift：Hello World
来源：http://td.newstarts.cn

print("Hello")
来源：http://jk.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://fx.szxytkj.cn

var a = 1;  let b = 2
来源：http://ne.gzmigu.cn

[T18] Swift：字符串插值
来源：http://rk.hnjuh.cn

"值: \(b)"
来源：http://mt.lnxyls.cn

[T19] Swift：可选绑定
来源：http://pf.szsharing.cn

if let n = opt { print(n) }
来源：http://rq.hnjuh.cn

[T20] Swift：数组操作
来源：http://cu.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yd.shxzskj.cn

[T21] Swift：遍历
来源：http://tx.muxihuayi.cn

for x in a { print(x) }
来源：http://fs.yuntaijiaju.cn

[T22] Swift：字典
来源：http://ki.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://an.haigaiapp.cn

[T23] Swift：函数
来源：http://ky.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pg.huanxung.cn

[T24] Swift：闭包
来源：http://bg.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zg.asd995.cn

[T25] Swift：结构体
来源：http://ar.gzmigu.cn

struct P { var x: Int }
来源：http://vv.szsharing.cn

[T26] Swift：类与重写
来源：http://xu.szsharing.cn

class A: Base { override func f() {} }
来源：http://jd.9csxet.cn

[T27] Swift：错误处理
来源：http://fp.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://jl.jctech888.com.cn

[T28] Swift：枚举
来源：http://hz.wgjwhj.cn

enum Color { case red, green }
来源：http://iy.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://eb.bjjhwx.cn

guard let x = opt else { return }
来源：http://zm.nicolike.cn

[T30] Swift：协议
来源：http://hv.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://pu.gzmigu.cn

[T31] Lua：Hello World
来源：http://xk.szxytkj.cn

print("Hello")
来源：http://kz.gzmigu.cn

[T32] Lua：局部变量
来源：http://cs.colortex.cn

local a = 1
来源：http://ti.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://sp.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bu.haigaiapp.cn

[T34] Lua：遍历表
来源：http://el.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hq.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://fg.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://qo.panjiajie.cn

[T36] Lua：函数
来源：http://nj.shxzukj.cn

function add(a, b) return a + b end
来源：http://tc.colortex.cn

[T37] Lua：字符串拼接
来源：http://qe.521024.cn

"a" .. "b"
来源：http://tc.asd995.cn

[T38] Lua：条件
来源：http://ib.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://ln.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://sy.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://un.hahajie.cn

[T40] Lua：元表
来源：http://ph.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://qc.asd995.cn

[T41] Perl：Hello World
来源：http://ko.bjjhwx.cn

print "Hello\n";
来源：http://ci.chemitech.net.cn

[T42] Perl：变量类型
来源：http://wd.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rl.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://aa.hnjuh.cn

"值: $a"
来源：http://ug.asd995.cn

[T44] Perl：条件
来源：http://rc.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://ql.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://qz.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://eh.colortex.cn

[T46] Perl：哈希操作
来源：http://bw.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://as.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://sy.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ax.gzmigu.cn

[T48] Perl：正则替换
来源：http://mm.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://cl.huixiangedu.cn

[T49] Perl：函数
来源：http://dy.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wu.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://ly.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ti.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://ic.colortex.cn

[T51] Scala：Hello World
来源：http://ym.szsharing.cn

println("Hello")
来源：http://oj.chemitech.net.cn

[T52] Scala：变量
来源：http://zm.shtwfgs.cn

val a = 1;  var b = 2
来源：http://vn.szsharing.cn

[T53] Scala：字符串插值
来源：http://be.colortex.cn

s"值: $b"
来源：http://iw.hnjuh.cn

[T54] Scala：集合映射
来源：http://qy.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://lt.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://sz.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uo.nicolike.cn

[T56] Scala：样例类
来源：http://fp.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://gw.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://cf.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zq.szxytkj.cn

[T58] Scala：函数定义
来源：http://sr.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sa.gzmigu.cn

[T59] Scala：循环
来源：http://jp.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://eo.wgjwhj.cn

[T60] Scala：折叠
来源：http://lo.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zo.shxzskj.cn

================================================================================
来源：http://ex.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ij.szsharing.cn

================================================================================
来源：http://mx.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://fs.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mq.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://vi.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jp.asd995.cn

[U03] Py：加载 .env 配置
来源：http://ez.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nb.nicolike.cn

[U04] Py：变量调试打印
来源：http://mq.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tl.9csxet.cn

[U05] Py：列表去重且保序
来源：http://wa.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://rd.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://qx.lnxyls.cn

{**a, **b}
来源：http://et.shxzskj.cn

[U07] Py：反转字典键值
来源：http://kp.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://kb.nicolike.cn

[U08] Py：展平二维列表
来源：http://ql.huanxung.cn

[y for x in nested for y in x]
来源：http://ri.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://ns.szsharing.cn

max(d, key=d.get)
来源：http://tn.shxzukj.cn

[U10] Py：按值排序字典
来源：http://xt.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://to.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://rj.nicolike.cn

(x * 2 for x in arr)
来源：http://dp.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mo.nicolike.cn

Counter(arr).most_common(3)
来源：http://zq.colortex.cn

[U13] Py：固定长度队列
来源：http://jx.shxzukj.cn

deque(maxlen=10)
来源：http://ia.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://st.bjjhwx.cn

defaultdict(list)
来源：http://bv.shtwfgs.cn

[U15] Py：高精度计时
来源：http://ke.gzmigu.cn

t = time.perf_counter()
来源：http://iu.szsharing.cn

[U16] Py：命令行参数解析
来源：http://qr.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jh.haigaiapp.cn

[U17] Py：初始化日志
来源：http://va.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://lj.gzmigu.cn

[U18] Py：预编译正则
来源：http://ro.521024.cn

pat = re.compile(r"\d+")
来源：http://xr.huanxung.cn

[U19] Py：正则替换带回调
来源：http://ij.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aj.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://qj.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://nm.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://nh.wgjwhj.cn

@contextlib.contextmanager
来源：http://cy.shxzskj.cn

[U22] Py：矩阵转置
来源：http://gx.huixinmuqiang.cn

list(zip(*m))
来源：http://lm.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://cx.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ax.newstarts.cn

[U24] Py：路径操作
来源：http://tc.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fo.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://sy.9csxet.cn

csv.DictReader(f)
来源：http://sp.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://rr.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pn.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://as.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://od.nszjky.cn

[U28] Py：类型别名
来源：http://lj.nszjky.cn

UserId = int
来源：http://uo.szsharing.cn

[U29] Py：属性校验
来源：http://bj.panjiajie.cn

@property 与 @x.setter 配合
来源：http://kg.huixinmuqiang.cn

[U30] Py：数据类
来源：http://ur.bjjhwx.cn

@dataclass(slots=True)
来源：http://hf.asd995.cn

[U31] Py：单测
来源：http://rs.bjjhwx.cn

python -m pytest -q
来源：http://gb.chemitech.net.cn

[U32] Py：代码格式化
来源：http://zp.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://mj.newstarts.cn

[U33] Py：打包发布
来源：http://dq.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://if.huanxung.cn

[U34] Py：判断编码
来源：http://cp.hnjuh.cn

chardet.detect(raw)
来源：http://nt.chemitech.net.cn

[U35] Py：发送邮件
来源：http://ri.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wk.newstarts.cn

[U36] Py：定时任务
来源：http://oh.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://ab.hahajie.cn

[U37] Py：读写 Excel
来源：http://ab.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gn.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://yg.colortex.cn

Path(__file__).resolve().parent
来源：http://nr.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://yw.hnjuh.cn

sys.stdout.isatty()
来源：http://th.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://ej.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://tr.shxzukj.cn


<!-- 参考信息 -->