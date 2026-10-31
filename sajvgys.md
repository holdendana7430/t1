代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://rp.huixinmuqiang.cn

[S23] C：随机数
来源：http://zg.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://na.nicolike.cn

[S24] C：获取本地时间
来源：http://cm.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qb.panjiajie.cn

[S25] C：内存拷贝
来源：http://vh.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://ay.haigaiapp.cn

[S26] C：内存清零
来源：http://wz.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://eh.yuntaijiaju.cn

[S27] C：定义常量
来源：http://ab.nszjky.cn

const double PI = 3.14159;
来源：http://zl.521024.cn

[S28] C：静态变量
来源：http://nf.newstarts.cn

static int counter = 0;
来源：http://xy.huanxung.cn

[S29] C：变参函数
来源：http://ew.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hk.szxytkj.cn

[S30] C：头文件保护
来源：http://jd.hnjuh.cn

#ifndef X_H
来源：http://oz.gzmigu.cn

#define X_H
来源：http://mw.jianghongdianzi.cn

#endif
来源：http://uj.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://zk.colortex.cn

#include <iostream>
来源：http://wm.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://dz.yuexingan06.cn

[S32] C++：字符串
来源：http://lx.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://hx.hahajie.cn

[S33] C++：vector 增删
来源：http://uv.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pb.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://co.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://qg.szxytkj.cn

[S35] C++：map
来源：http://jx.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sg.asd995.cn

[S36] C++：unordered_map
来源：http://lh.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ek.colortex.cn

[S37] C++：set
来源：http://ja.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ju.colortex.cn

[S38] C++：排序
来源：http://ry.521024.cn

std::sort(v.begin(), v.end());
来源：http://vp.521024.cn

[S39] C++：自定义比较器排序
来源：http://db.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fb.hahajie.cn

[S40] C++：查找元素
来源：http://wc.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kg.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://hy.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oo.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://hk.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://fx.panjiajie.cn

[S43] C++：智能指针
来源：http://lj.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://ez.hnjuh.cn

[S44] C++：引用传参
来源：http://yk.huanxung.cn

void inc(int &x) { ++x; }
来源：http://jy.lnxyls.cn

[S45] C++：lambda
来源：http://yt.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mc.panjiajie.cn

[S46] C++：函数模板
来源：http://xd.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iz.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://bb.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ec.hnjuh.cn

[S48] C++：逐行读文件
来源：http://tl.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oy.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://xp.haigaiapp.cn

[S49] C++：写文件
来源：http://dv.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://am.asd995.cn

[S50] C++：格式化数字
来源：http://al.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ly.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://nw.jctech888.com.cn

static_cast<double>(a) / b
来源：http://sz.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://bm.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://pg.shxzskj.cn

[S53] C++：移动语义
来源：http://xf.521024.cn

std::vector<int> w = std::move(v);
来源：http://ht.shxzskj.cn

[S54] C++：异常处理
来源：http://on.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qk.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://me.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sx.gzmigu.cn

[S56] C++：optional
来源：http://ou.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ab.521024.cn

[S57] C++：编译期常量
来源：http://gy.huixiangedu.cn

constexpr int N = 10;
来源：http://xt.jctech888.com.cn

[S58] C++：命名空间
来源：http://xk.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://zz.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://gy.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://im.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://bl.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hc.lnxyls.cn

================================================================================
来源：http://zo.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xz.jianghongdianzi.cn

================================================================================
来源：http://jj.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://vm.gzmigu.cn

println("Hello")
来源：http://xn.muxihuayi.cn

[T02] Kotlin：变量
来源：http://me.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nt.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://xp.521024.cn

"值: $b"
来源：http://xi.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://rq.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://xf.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://eh.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xd.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://ta.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yh.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://aj.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dx.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://sd.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://dg.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://km.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://xq.hahajie.cn

[T10] Kotlin：默认参数
来源：http://ki.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ne.chemitech.net.cn

[T11] Kotlin：协程
来源：http://cn.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rr.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://nl.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://ve.colortex.cn

[T13] Kotlin：只读 Map
来源：http://fe.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://dx.lnxyls.cn

[T14] Kotlin：循环
来源：http://ry.521024.cn

for (i in 1..10) println(i)
来源：http://gt.521024.cn

[T15] Kotlin：接口
来源：http://xt.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://uo.nszjky.cn

[T16] Swift：Hello World
来源：http://sk.newstarts.cn

print("Hello")
来源：http://mw.nicolike.cn

[T17] Swift：变量与常量
来源：http://xa.muxihuayi.cn

var a = 1;  let b = 2
来源：http://kb.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://hr.gzmigu.cn

"值: \(b)"
来源：http://hj.asd995.cn

[T19] Swift：可选绑定
来源：http://vo.szxytkj.cn

if let n = opt { print(n) }
来源：http://iz.shxzukj.cn

[T20] Swift：数组操作
来源：http://ze.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fa.colortex.cn

[T21] Swift：遍历
来源：http://tz.newstarts.cn

for x in a { print(x) }
来源：http://yh.yuntaijiaju.cn

[T22] Swift：字典
来源：http://rs.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xx.521024.cn

[T23] Swift：函数
来源：http://ay.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nr.wgjwhj.cn

[T24] Swift：闭包
来源：http://mo.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lg.chemitech.net.cn

[T25] Swift：结构体
来源：http://va.shtwfgs.cn

struct P { var x: Int }
来源：http://lj.lnxyls.cn

[T26] Swift：类与重写
来源：http://fh.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://sb.muxihuayi.cn

[T27] Swift：错误处理
来源：http://cn.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://hn.nszjky.cn

[T28] Swift：枚举
来源：http://dt.yuexingan06.cn

enum Color { case red, green }
来源：http://sn.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://sc.jctech888.com.cn

guard let x = opt else { return }
来源：http://tj.szsharing.cn

[T30] Swift：协议
来源：http://dq.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://cq.521024.cn

[T31] Lua：Hello World
来源：http://lr.muxihuayi.cn

print("Hello")
来源：http://sy.hahajie.cn

[T32] Lua：局部变量
来源：http://cg.colortex.cn

local a = 1
来源：http://tv.shxzskj.cn

[T33] Lua：表（数组）
来源：http://fa.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yy.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://ur.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fc.shxzskj.cn

[T35] Lua：字典表
来源：http://yf.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://oc.521024.cn

[T36] Lua：函数
来源：http://jk.szxytkj.cn

function add(a, b) return a + b end
来源：http://rg.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://rh.gzmigu.cn

"a" .. "b"
来源：http://bl.gzmigu.cn

[T38] Lua：条件
来源：http://jf.wgjwhj.cn

if x > 0 then print("正") end
来源：http://uk.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://pr.szsharing.cn

string.find(s, "%d+")
来源：http://wx.panjiajie.cn

[T40] Lua：元表
来源：http://uh.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://ch.shtwfgs.cn

[T41] Perl：Hello World
来源：http://zd.szsharing.cn

print "Hello\n";
来源：http://hr.gzmigu.cn

[T42] Perl：变量类型
来源：http://xb.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bh.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://ii.gzmigu.cn

"值: $a"
来源：http://fi.lnxyls.cn

[T44] Perl：条件
来源：http://yg.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://te.panjiajie.cn

[T45] Perl：数组遍历
来源：http://ab.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://tp.szxytkj.cn

[T46] Perl：哈希操作
来源：http://wx.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fw.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://tj.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jn.colortex.cn

[T48] Perl：正则替换
来源：http://dt.shxzskj.cn

$s =~ s/old/new/g;
来源：http://sl.huanxung.cn

[T49] Perl：函数
来源：http://xa.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mm.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://rj.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tk.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://bm.chemitech.net.cn

[T51] Scala：Hello World
来源：http://mc.yuexingan06.cn

println("Hello")
来源：http://qh.haigaiapp.cn

[T52] Scala：变量
来源：http://wq.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://sk.szxytkj.cn

[T53] Scala：字符串插值
来源：http://il.haigaiapp.cn

s"值: $b"
来源：http://np.wgjwhj.cn

[T54] Scala：集合映射
来源：http://sa.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://on.lnxyls.cn

[T55] Scala：集合过滤
来源：http://nv.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ps.nicolike.cn

[T56] Scala：样例类
来源：http://uo.colortex.cn

case class User(name: String, age: Int)
来源：http://mi.colortex.cn

[T57] Scala：模式匹配
来源：http://vu.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lf.shtwfgs.cn

[T58] Scala：函数定义
来源：http://er.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ga.shxzukj.cn

[T59] Scala：循环
来源：http://dt.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://vw.hnjuh.cn

[T60] Scala：折叠
来源：http://ld.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ie.muxihuayi.cn

================================================================================
来源：http://yv.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bz.521024.cn

================================================================================
来源：http://re.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://tv.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ju.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://th.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gh.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://an.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zi.hahajie.cn

[U04] Py：变量调试打印
来源：http://zi.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fh.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://gf.521024.cn

list(dict.fromkeys(arr))
来源：http://kt.panjiajie.cn

[U06] Py：合并两个字典
来源：http://lx.bookmarksfly.cn

{**a, **b}
来源：http://xd.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://yt.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://kg.shxzskj.cn

[U08] Py：展平二维列表
来源：http://xb.newstarts.cn

[y for x in nested for y in x]
来源：http://pg.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://fw.chemitech.net.cn

max(d, key=d.get)
来源：http://ql.nszjky.cn

[U10] Py：按值排序字典
来源：http://ha.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sk.colortex.cn

[U11] Py：生成器表达式
来源：http://wj.lnxyls.cn

(x * 2 for x in arr)
来源：http://ln.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cu.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://md.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://jm.jctech888.com.cn

deque(maxlen=10)
来源：http://sv.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://my.huixiangedu.cn

defaultdict(list)
来源：http://kq.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://at.bookmarksfly.cn

t = time.perf_counter()
来源：http://pr.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://pb.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oz.panjiajie.cn

[U17] Py：初始化日志
来源：http://qy.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://mk.chemitech.net.cn

[U18] Py：预编译正则
来源：http://zx.nszjky.cn

pat = re.compile(r"\d+")
来源：http://ni.newstarts.cn

[U19] Py：正则替换带回调
来源：http://yq.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gx.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://tl.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://cy.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://ph.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://pw.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://py.jianghongdianzi.cn

list(zip(*m))
来源：http://zn.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://tu.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://su.hahajie.cn

[U24] Py：路径操作
来源：http://xt.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://io.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://ch.shxzskj.cn

csv.DictReader(f)
来源：http://pe.9csxet.cn

[U26] Py：并发下载
来源：http://hy.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hs.521024.cn

[U27] Py：异步 HTTP
来源：http://yr.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://ka.hnjuh.cn

[U28] Py：类型别名
来源：http://qg.bjjhwx.cn

UserId = int
来源：http://ef.newstarts.cn

[U29] Py：属性校验
来源：http://gn.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://wx.jianghongdianzi.cn

[U30] Py：数据类
来源：http://dt.huanxung.cn

@dataclass(slots=True)
来源：http://fd.nszjky.cn

[U31] Py：单测
来源：http://gb.huixiangedu.cn

python -m pytest -q
来源：http://rb.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://xz.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://rd.shxzskj.cn

[U33] Py：打包发布
来源：http://zz.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://rc.colortex.cn

[U34] Py：判断编码
来源：http://mn.gzmigu.cn

chardet.detect(raw)
来源：http://oo.hnjuh.cn

[U35] Py：发送邮件
来源：http://es.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ab.chemitech.net.cn

[U36] Py：定时任务
来源：http://jw.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://dj.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://uy.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ed.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://ts.lnxyls.cn

Path(__file__).resolve().parent
来源：http://up.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://uf.521024.cn

sys.stdout.isatty()
来源：http://ia.9csxet.cn

[U40] Py：打印到标准错误
来源：http://yf.asd995.cn

print("err", file=sys.stderr)
来源：http://ul.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://gr.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://in.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ak.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ae.huanxung.cn

[U43] PHP：声明命名空间
来源：http://ih.asd995.cn

namespace App\Http;
来源：http://ub.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://cw.newstarts.cn

declare(strict_types=1);
来源：http://jp.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://yd.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xm.panjiajie.cn

[U46] PHP：可空类型
来源：http://mz.haigaiapp.cn

?string $name = null
来源：http://io.colortex.cn


<!-- 参考信息 -->