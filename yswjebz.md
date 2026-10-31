代发 wailian999

x |= (1 << 3);
来源：http://ku.hahajie.cn

[S17] C：安全拼接字符串
来源：http://kv.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xg.muxihuayi.cn

[S18] C：命令行参数
来源：http://jv.asd995.cn

int main(int argc, char **argv)
来源：http://yv.shxzukj.cn

[S19] C：快速排序
来源：http://qb.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fo.yuexingan06.cn

[S20] C：二分查找
来源：http://so.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gu.muxihuayi.cn

[S21] C：字符类别判断
来源：http://be.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kh.muxihuayi.cn

[S22] C：字符串转数字
来源：http://le.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gy.huixiangedu.cn

[S23] C：随机数
来源：http://ty.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hc.colortex.cn

[S24] C：获取本地时间
来源：http://bf.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bg.colortex.cn

[S25] C：内存拷贝
来源：http://af.szxytkj.cn

memcpy(dst, src, n);
来源：http://lc.9csxet.cn

[S26] C：内存清零
来源：http://zs.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://qu.hnjuh.cn

[S27] C：定义常量
来源：http://ys.szxytkj.cn

const double PI = 3.14159;
来源：http://gl.shtwfgs.cn

[S28] C：静态变量
来源：http://te.asd995.cn

static int counter = 0;
来源：http://im.muxihuayi.cn

[S29] C：变参函数
来源：http://cz.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eb.shxzskj.cn

[S30] C：头文件保护
来源：http://ng.jianghongdianzi.cn

#ifndef X_H
来源：http://kl.yuntaijiaju.cn

#define X_H
来源：http://dg.shxzukj.cn

#endif
来源：http://yv.shtwfgs.cn

[S31] C++：Hello World
来源：http://jk.lnxyls.cn

#include <iostream>
来源：http://ko.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://bc.huixiangedu.cn

[S32] C++：字符串
来源：http://sy.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://ml.huixiangedu.cn

[S33] C++：vector 增删
来源：http://jw.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tv.gzmigu.cn

[S34] C++：遍历 vector
来源：http://qa.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://as.szxytkj.cn

[S35] C++：map
来源：http://vf.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nr.yuexingan06.cn

[S36] C++：unordered_map
来源：http://eb.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lo.muxihuayi.cn

[S37] C++：set
来源：http://kf.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fg.nicolike.cn

[S38] C++：排序
来源：http://lk.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://ew.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://os.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wc.szsharing.cn

[S40] C++：查找元素
来源：http://md.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dz.nicolike.cn

[S41] C++：类与构造函数
来源：http://jk.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://de.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://aj.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://ve.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://rh.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://fo.yuexingan06.cn

[S44] C++：引用传参
来源：http://qg.newstarts.cn

void inc(int &x) { ++x; }
来源：http://dt.521024.cn

[S45] C++：lambda
来源：http://gq.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jd.wgjwhj.cn

[S46] C++：函数模板
来源：http://ko.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fq.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://re.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nd.szxytkj.cn

[S48] C++：逐行读文件
来源：http://lo.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ky.newstarts.cn

while (std::getline(in, line)) { }
来源：http://lm.hahajie.cn

[S49] C++：写文件
来源：http://os.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aa.newstarts.cn

[S50] C++：格式化数字
来源：http://xk.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fb.hahajie.cn

[S51] C++：显式类型转换
来源：http://kk.shxzukj.cn

static_cast<double>(a) / b
来源：http://vi.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://gb.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://uk.szxytkj.cn

[S53] C++：移动语义
来源：http://kq.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://jw.huixiangedu.cn

[S54] C++：异常处理
来源：http://ke.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fj.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://cu.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ct.bookmarksfly.cn

[S56] C++：optional
来源：http://ak.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vh.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://mg.hahajie.cn

constexpr int N = 10;
来源：http://um.colortex.cn

[S58] C++：命名空间
来源：http://xy.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://an.gzmigu.cn

[S59] C++：静态断言
来源：http://mi.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oe.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://fw.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fw.jianghongdianzi.cn

================================================================================
来源：http://hi.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qm.huixiangedu.cn

================================================================================
来源：http://pd.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://oi.hahajie.cn

println("Hello")
来源：http://cj.huanxung.cn

[T02] Kotlin：变量
来源：http://us.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ok.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://xp.newstarts.cn

"值: $b"
来源：http://nu.huanxung.cn

[T04] Kotlin：空安全
来源：http://by.panjiajie.cn

val n: String? = null;  n?.length
来源：http://yv.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://lt.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kw.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://fc.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://my.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://wk.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://va.9csxet.cn

[T08] Kotlin：数据类
来源：http://wx.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://qh.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://zg.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://ie.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://it.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hw.hahajie.cn

[T11] Kotlin：协程
来源：http://lp.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tg.521024.cn

[T12] Kotlin：解构声明
来源：http://mn.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://xb.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://be.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://iv.shtwfgs.cn

[T14] Kotlin：循环
来源：http://ep.szxytkj.cn

for (i in 1..10) println(i)
来源：http://fd.hnjuh.cn

[T15] Kotlin：接口
来源：http://kk.newstarts.cn

interface Shape { fun area(): Double }
来源：http://nf.colortex.cn

[T16] Swift：Hello World
来源：http://ha.szsharing.cn

print("Hello")
来源：http://ay.huanxung.cn

[T17] Swift：变量与常量
来源：http://st.huixiangedu.cn

var a = 1;  let b = 2
来源：http://vo.asd995.cn

[T18] Swift：字符串插值
来源：http://yw.hahajie.cn

"值: \(b)"
来源：http://cf.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://ug.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://ax.hnjuh.cn

[T20] Swift：数组操作
来源：http://zc.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kc.shxzukj.cn

[T21] Swift：遍历
来源：http://uf.shxzskj.cn

for x in a { print(x) }
来源：http://mt.bjjhwx.cn

[T22] Swift：字典
来源：http://qx.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fz.newstarts.cn

[T23] Swift：函数
来源：http://gt.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fx.szxytkj.cn

[T24] Swift：闭包
来源：http://md.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ii.9csxet.cn

[T25] Swift：结构体
来源：http://zj.gzmigu.cn

struct P { var x: Int }
来源：http://fr.shxzskj.cn

[T26] Swift：类与重写
来源：http://hg.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://gq.haigaiapp.cn

[T27] Swift：错误处理
来源：http://aw.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://ur.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://kg.asd995.cn

enum Color { case red, green }
来源：http://hu.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://pa.nszjky.cn

guard let x = opt else { return }
来源：http://zc.colortex.cn

[T30] Swift：协议
来源：http://ip.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://sq.asd995.cn

[T31] Lua：Hello World
来源：http://wh.hnjuh.cn

print("Hello")
来源：http://fr.huanxung.cn

[T32] Lua：局部变量
来源：http://lp.yuexingan06.cn

local a = 1
来源：http://vg.huanxung.cn

[T33] Lua：表（数组）
来源：http://ar.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sp.nszjky.cn

[T34] Lua：遍历表
来源：http://gx.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ry.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://ng.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://sk.colortex.cn

[T36] Lua：函数
来源：http://wg.szxytkj.cn

function add(a, b) return a + b end
来源：http://ht.9csxet.cn

[T37] Lua：字符串拼接
来源：http://cl.newstarts.cn

"a" .. "b"
来源：http://oc.shtwfgs.cn

[T38] Lua：条件
来源：http://hb.shtwfgs.cn

if x > 0 then print("正") end
来源：http://pp.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://mm.9csxet.cn

string.find(s, "%d+")
来源：http://so.jctech888.com.cn

[T40] Lua：元表
来源：http://tq.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://rg.szxytkj.cn

[T41] Perl：Hello World
来源：http://wf.hahajie.cn

print "Hello\n";
来源：http://rg.panjiajie.cn

[T42] Perl：变量类型
来源：http://fr.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bn.shxzukj.cn

[T43] Perl：字符串插值
来源：http://eh.bjjhwx.cn

"值: $a"
来源：http://hf.gzmigu.cn

[T44] Perl：条件
来源：http://dm.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://iz.521024.cn

[T45] Perl：数组遍历
来源：http://xg.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://zl.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://hw.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://by.huanxung.cn

[T47] Perl：正则捕获
来源：http://ob.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jr.shtwfgs.cn

[T48] Perl：正则替换
来源：http://rf.szsharing.cn

$s =~ s/old/new/g;
来源：http://fh.szxytkj.cn

[T49] Perl：函数
来源：http://nv.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ti.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://je.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vt.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://wx.shtwfgs.cn

[T51] Scala：Hello World
来源：http://xy.chemitech.net.cn

println("Hello")
来源：http://mv.szxytkj.cn

[T52] Scala：变量
来源：http://bw.yuexingan06.cn

val a = 1;  var b = 2
来源：http://ep.hahajie.cn

[T53] Scala：字符串插值
来源：http://hm.colortex.cn

s"值: $b"
来源：http://if.chemitech.net.cn

[T54] Scala：集合映射
来源：http://mc.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://wq.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://yw.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iq.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://du.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://oz.lnxyls.cn

[T57] Scala：模式匹配
来源：http://ml.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qe.colortex.cn

[T58] Scala：函数定义
来源：http://wm.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://je.hahajie.cn

[T59] Scala：循环
来源：http://se.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://vl.gzmigu.cn

[T60] Scala：折叠
来源：http://tp.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://th.bjjhwx.cn

================================================================================
来源：http://ec.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hv.asd995.cn

================================================================================
来源：http://zs.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://ub.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cq.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://zc.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xl.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://dw.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://en.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://hy.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qc.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://ln.newstarts.cn

list(dict.fromkeys(arr))
来源：http://px.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://gd.hnjuh.cn

{**a, **b}
来源：http://ku.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://yu.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://mo.lnxyls.cn

[U08] Py：展平二维列表
来源：http://ng.szxytkj.cn

[y for x in nested for y in x]
来源：http://az.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://rt.chemitech.net.cn

max(d, key=d.get)
来源：http://ny.panjiajie.cn

[U10] Py：按值排序字典
来源：http://ak.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lx.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://lz.szxytkj.cn

(x * 2 for x in arr)
来源：http://zt.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hp.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://rq.hahajie.cn

[U13] Py：固定长度队列
来源：http://oq.panjiajie.cn

deque(maxlen=10)
来源：http://kh.nszjky.cn

[U14] Py：分组收集到列表
来源：http://vd.jctech888.com.cn

defaultdict(list)
来源：http://bc.hahajie.cn

[U15] Py：高精度计时
来源：http://hy.huanxung.cn

t = time.perf_counter()
来源：http://tk.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://fb.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ka.panjiajie.cn

[U17] Py：初始化日志
来源：http://pn.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://pu.colortex.cn

[U18] Py：预编译正则
来源：http://wb.hahajie.cn

pat = re.compile(r"\d+")
来源：http://lh.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://it.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fv.521024.cn

[U20] Py：缓存函数结果
来源：http://sk.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://pf.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://gk.huanxung.cn

@contextlib.contextmanager
来源：http://vh.nszjky.cn

[U22] Py：矩阵转置
来源：http://zj.szxytkj.cn

list(zip(*m))
来源：http://wo.nszjky.cn

[U23] Py：分块读取大文件
来源：http://bi.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ve.szxytkj.cn

[U24] Py：路径操作
来源：http://or.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mt.521024.cn

[U25] Py：CSV 按字典读
来源：http://qh.nszjky.cn

csv.DictReader(f)
来源：http://pk.colortex.cn

[U26] Py：并发下载
来源：http://so.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wu.9csxet.cn

[U27] Py：异步 HTTP
来源：http://op.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://od.colortex.cn

[U28] Py：类型别名
来源：http://ok.shxzskj.cn

UserId = int
来源：http://wg.shxzukj.cn

[U29] Py：属性校验
来源：http://bl.panjiajie.cn

@property 与 @x.setter 配合
来源：http://pr.hahajie.cn

[U30] Py：数据类
来源：http://jf.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://zh.lnxyls.cn

[U31] Py：单测
来源：http://br.chemitech.net.cn

python -m pytest -q
来源：http://zj.yuexingan06.cn

[U32] Py：代码格式化
来源：http://bu.huanxung.cn

ruff format . && ruff check --fix .
来源：http://kj.huixiangedu.cn

[U33] Py：打包发布
来源：http://pd.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://jn.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://zd.shxzskj.cn

chardet.detect(raw)
来源：http://jn.gzmigu.cn

[U35] Py：发送邮件
来源：http://pl.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iw.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://dx.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://at.newstarts.cn

[U37] Py：读写 Excel
来源：http://um.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bs.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://gt.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://fx.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://en.huixiangedu.cn

sys.stdout.isatty()
来源：http://xu.nicolike.cn

[U40] Py：打印到标准错误
来源：http://kj.nszjky.cn

print("err", file=sys.stderr)
来源：http://bb.huixiangedu.cn


<!-- 参考信息 -->