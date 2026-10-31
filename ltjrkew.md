代发 wailian999

int main(int argc, char **argv)
来源：http://ft.lnxyls.cn

[S19] C：快速排序
来源：http://jj.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rp.521024.cn

[S20] C：二分查找
来源：http://hu.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vi.yuexingan06.cn

[S21] C：字符类别判断
来源：http://rb.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gb.nicolike.cn

[S22] C：字符串转数字
来源：http://mb.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vm.bookmarksfly.cn

[S23] C：随机数
来源：http://ez.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dw.asd995.cn

[S24] C：获取本地时间
来源：http://ys.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rq.huanxung.cn

[S25] C：内存拷贝
来源：http://mf.jctech888.com.cn

memcpy(dst, src, n);
来源：http://gh.huixinmuqiang.cn

[S26] C：内存清零
来源：http://gc.colortex.cn

memset(a, 0, sizeof a);
来源：http://kt.nicolike.cn

[S27] C：定义常量
来源：http://ci.colortex.cn

const double PI = 3.14159;
来源：http://kg.jctech888.com.cn

[S28] C：静态变量
来源：http://jf.wgjwhj.cn

static int counter = 0;
来源：http://hm.haigaiapp.cn

[S29] C：变参函数
来源：http://ue.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rn.colortex.cn

[S30] C：头文件保护
来源：http://hn.bjjhwx.cn

#ifndef X_H
来源：http://gn.huixinmuqiang.cn

#define X_H
来源：http://re.gzmigu.cn

#endif
来源：http://ny.shtwfgs.cn

[S31] C++：Hello World
来源：http://mk.lnxyls.cn

#include <iostream>
来源：http://fs.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://dg.yuntaijiaju.cn

[S32] C++：字符串
来源：http://pp.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://mm.9csxet.cn

[S33] C++：vector 增删
来源：http://iw.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xa.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://kw.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://sp.asd995.cn

[S35] C++：map
来源：http://qg.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://di.szsharing.cn

[S36] C++：unordered_map
来源：http://qw.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qu.lnxyls.cn

[S37] C++：set
来源：http://oa.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ub.huanxung.cn

[S38] C++：排序
来源：http://kq.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://jt.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://fy.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jl.shxzskj.cn

[S40] C++：查找元素
来源：http://mt.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bs.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://hq.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jj.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://jb.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://xz.szsharing.cn

[S43] C++：智能指针
来源：http://ci.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://vc.hahajie.cn

[S44] C++：引用传参
来源：http://fh.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://ev.huixiangedu.cn

[S45] C++：lambda
来源：http://pq.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sy.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://it.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ho.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://wy.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kw.szxytkj.cn

[S48] C++：逐行读文件
来源：http://sz.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fo.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://mn.huixinmuqiang.cn

[S49] C++：写文件
来源：http://ft.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ms.lnxyls.cn

[S50] C++：格式化数字
来源：http://ee.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ko.hahajie.cn

[S51] C++：显式类型转换
来源：http://bb.jctech888.com.cn

static_cast<double>(a) / b
来源：http://nq.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://fz.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://gh.szsharing.cn

[S53] C++：移动语义
来源：http://by.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://xs.yuexingan06.cn

[S54] C++：异常处理
来源：http://nl.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ju.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://jm.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kt.bjjhwx.cn

[S56] C++：optional
来源：http://rs.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jr.muxihuayi.cn

[S57] C++：编译期常量
来源：http://tq.szsharing.cn

constexpr int N = 10;
来源：http://ks.asd995.cn

[S58] C++：命名空间
来源：http://yl.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://li.9csxet.cn

[S59] C++：静态断言
来源：http://xq.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tp.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://pb.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lm.shxzukj.cn

================================================================================
来源：http://mc.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ir.colortex.cn

================================================================================
来源：http://vk.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://lq.haigaiapp.cn

println("Hello")
来源：http://ld.muxihuayi.cn

[T02] Kotlin：变量
来源：http://ss.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fp.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://hc.hahajie.cn

"值: $b"
来源：http://tk.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://sc.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://ru.colortex.cn

[T05] Kotlin：when 表达式
来源：http://tb.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dx.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://fa.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ui.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://un.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sy.hnjuh.cn

[T08] Kotlin：数据类
来源：http://al.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://qt.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://uj.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://hg.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://lx.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://di.newstarts.cn

[T11] Kotlin：协程
来源：http://cg.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lh.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://vf.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://vh.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://mw.newstarts.cn

val m = mapOf("a" to 1)
来源：http://jz.huanxung.cn

[T14] Kotlin：循环
来源：http://zm.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://nn.9csxet.cn

[T15] Kotlin：接口
来源：http://py.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://bo.shxzukj.cn

[T16] Swift：Hello World
来源：http://my.szsharing.cn

print("Hello")
来源：http://cm.hahajie.cn

[T17] Swift：变量与常量
来源：http://xx.hahajie.cn

var a = 1;  let b = 2
来源：http://rz.hnjuh.cn

[T18] Swift：字符串插值
来源：http://uu.szxytkj.cn

"值: \(b)"
来源：http://ho.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://bw.bjjhwx.cn

if let n = opt { print(n) }
来源：http://og.jctech888.com.cn

[T20] Swift：数组操作
来源：http://io.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ja.nszjky.cn

[T21] Swift：遍历
来源：http://ku.szxytkj.cn

for x in a { print(x) }
来源：http://jt.colortex.cn

[T22] Swift：字典
来源：http://rl.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fb.huixinmuqiang.cn

[T23] Swift：函数
来源：http://lh.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bw.jctech888.com.cn

[T24] Swift：闭包
来源：http://pg.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kf.colortex.cn

[T25] Swift：结构体
来源：http://mn.nicolike.cn

struct P { var x: Int }
来源：http://xu.newstarts.cn

[T26] Swift：类与重写
来源：http://he.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://lg.9csxet.cn

[T27] Swift：错误处理
来源：http://oz.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://tj.panjiajie.cn

[T28] Swift：枚举
来源：http://ta.szsharing.cn

enum Color { case red, green }
来源：http://fq.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://su.chemitech.net.cn

guard let x = opt else { return }
来源：http://mc.bjjhwx.cn

[T30] Swift：协议
来源：http://bk.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://mj.colortex.cn

[T31] Lua：Hello World
来源：http://ny.muxihuayi.cn

print("Hello")
来源：http://jg.huanxung.cn

[T32] Lua：局部变量
来源：http://lb.huixinmuqiang.cn

local a = 1
来源：http://gs.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://kx.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dd.newstarts.cn

[T34] Lua：遍历表
来源：http://io.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wn.nszjky.cn

[T35] Lua：字典表
来源：http://sc.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://jl.shtwfgs.cn

[T36] Lua：函数
来源：http://sw.yuexingan06.cn

function add(a, b) return a + b end
来源：http://yp.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://jo.gzmigu.cn

"a" .. "b"
来源：http://pg.9csxet.cn

[T38] Lua：条件
来源：http://ec.bjjhwx.cn

if x > 0 then print("正") end
来源：http://ph.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://kj.yuexingan06.cn

string.find(s, "%d+")
来源：http://av.jctech888.com.cn

[T40] Lua：元表
来源：http://wd.521024.cn

setmetatable({}, { __index = base })
来源：http://bh.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://wr.shtwfgs.cn

print "Hello\n";
来源：http://zl.hahajie.cn

[T42] Perl：变量类型
来源：http://lz.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ik.newstarts.cn

[T43] Perl：字符串插值
来源：http://mc.9csxet.cn

"值: $a"
来源：http://ms.gzmigu.cn

[T44] Perl：条件
来源：http://zq.asd995.cn

if ($a > 0) { print "正"; }
来源：http://kb.szsharing.cn

[T45] Perl：数组遍历
来源：http://fo.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://of.shxzukj.cn

[T46] Perl：哈希操作
来源：http://wk.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nw.nszjky.cn

[T47] Perl：正则捕获
来源：http://wf.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zj.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://dg.gzmigu.cn

$s =~ s/old/new/g;
来源：http://pn.jctech888.com.cn

[T49] Perl：函数
来源：http://rf.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gq.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://ft.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uk.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://vp.panjiajie.cn

[T51] Scala：Hello World
来源：http://cn.shxzskj.cn

println("Hello")
来源：http://ot.bookmarksfly.cn

[T52] Scala：变量
来源：http://tg.nszjky.cn

val a = 1;  var b = 2
来源：http://if.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://hr.huanxung.cn

s"值: $b"
来源：http://qw.shxzskj.cn

[T54] Scala：集合映射
来源：http://ec.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://qk.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://aq.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eq.panjiajie.cn

[T56] Scala：样例类
来源：http://vu.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://uy.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://dq.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zw.hnjuh.cn

[T58] Scala：函数定义
来源：http://ht.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bf.huixinmuqiang.cn

[T59] Scala：循环
来源：http://jd.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://el.shxzukj.cn

[T60] Scala：折叠
来源：http://hi.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cd.newstarts.cn

================================================================================
来源：http://uc.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gd.hahajie.cn

================================================================================
来源：http://hm.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://sr.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rk.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://gw.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sk.521024.cn

[U03] Py：加载 .env 配置
来源：http://ru.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uw.asd995.cn

[U04] Py：变量调试打印
来源：http://cx.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ic.huanxung.cn

[U05] Py：列表去重且保序
来源：http://qn.szsharing.cn

list(dict.fromkeys(arr))
来源：http://eb.newstarts.cn

[U06] Py：合并两个字典
来源：http://ik.jctech888.com.cn

{**a, **b}
来源：http://xy.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://sc.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://oa.gzmigu.cn

[U08] Py：展平二维列表
来源：http://qg.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://np.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://ah.asd995.cn

max(d, key=d.get)
来源：http://sr.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://kg.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ls.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://tk.9csxet.cn

(x * 2 for x in arr)
来源：http://ew.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xq.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://fc.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://oo.newstarts.cn

deque(maxlen=10)
来源：http://zi.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://fu.shxzukj.cn

defaultdict(list)
来源：http://nj.newstarts.cn

[U15] Py：高精度计时
来源：http://ho.shxzskj.cn

t = time.perf_counter()
来源：http://ax.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://qu.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ao.chemitech.net.cn

[U17] Py：初始化日志
来源：http://ke.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://gn.newstarts.cn

[U18] Py：预编译正则
来源：http://cx.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://aq.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://lu.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ue.9csxet.cn

[U20] Py：缓存函数结果
来源：http://cz.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://xd.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://kk.szsharing.cn

@contextlib.contextmanager
来源：http://kk.521024.cn

[U22] Py：矩阵转置
来源：http://rz.huixiangedu.cn

list(zip(*m))
来源：http://sg.hahajie.cn

[U23] Py：分块读取大文件
来源：http://ky.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kw.yuexingan06.cn

[U24] Py：路径操作
来源：http://jn.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qt.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://im.hnjuh.cn

csv.DictReader(f)
来源：http://bw.haigaiapp.cn

[U26] Py：并发下载
来源：http://ka.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://js.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://ic.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://yf.colortex.cn

[U28] Py：类型别名
来源：http://xn.shxzskj.cn

UserId = int
来源：http://nm.wgjwhj.cn

[U29] Py：属性校验
来源：http://tt.nszjky.cn

@property 与 @x.setter 配合
来源：http://dg.hnjuh.cn

[U30] Py：数据类
来源：http://xs.newstarts.cn

@dataclass(slots=True)
来源：http://zt.hnjuh.cn

[U31] Py：单测
来源：http://ek.huixinmuqiang.cn

python -m pytest -q
来源：http://gm.lnxyls.cn

[U32] Py：代码格式化
来源：http://cr.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://xo.hnjuh.cn

[U33] Py：打包发布
来源：http://bv.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://wv.haigaiapp.cn

[U34] Py：判断编码
来源：http://xa.jctech888.com.cn

chardet.detect(raw)
来源：http://fz.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://lx.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sm.huanxung.cn

[U36] Py：定时任务
来源：http://fw.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://tb.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://al.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qq.521024.cn

[U38] Py：获取脚本所在目录
来源：http://gh.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://gs.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://kg.lnxyls.cn

sys.stdout.isatty()
来源：http://rb.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://sr.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://hh.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://ml.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kj.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://jr.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pj.haigaiapp.cn


<!-- 参考信息 -->