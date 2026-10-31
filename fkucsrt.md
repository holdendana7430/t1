代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yb.shxzskj.cn

[S25] C：内存拷贝
来源：http://fb.nicolike.cn

memcpy(dst, src, n);
来源：http://ab.huanxung.cn

[S26] C：内存清零
来源：http://jc.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://ls.yuntaijiaju.cn

[S27] C：定义常量
来源：http://dc.hahajie.cn

const double PI = 3.14159;
来源：http://ke.gzmigu.cn

[S28] C：静态变量
来源：http://ra.jctech888.com.cn

static int counter = 0;
来源：http://cl.nszjky.cn

[S29] C：变参函数
来源：http://py.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nn.haigaiapp.cn

[S30] C：头文件保护
来源：http://zo.jianghongdianzi.cn

#ifndef X_H
来源：http://ta.gzmigu.cn

#define X_H
来源：http://ux.bookmarksfly.cn

#endif
来源：http://it.shxzukj.cn

[S31] C++：Hello World
来源：http://xo.bookmarksfly.cn

#include <iostream>
来源：http://as.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://gg.panjiajie.cn

[S32] C++：字符串
来源：http://la.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://nl.hahajie.cn

[S33] C++：vector 增删
来源：http://cf.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pe.panjiajie.cn

[S34] C++：遍历 vector
来源：http://mj.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://bc.panjiajie.cn

[S35] C++：map
来源：http://eu.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tt.nicolike.cn

[S36] C++：unordered_map
来源：http://pw.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tv.huixinmuqiang.cn

[S37] C++：set
来源：http://uh.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ny.shxzukj.cn

[S38] C++：排序
来源：http://tx.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://sk.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://ks.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sc.haigaiapp.cn

[S40] C++：查找元素
来源：http://ra.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wl.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://nw.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lk.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://tg.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://tb.nicolike.cn

[S43] C++：智能指针
来源：http://il.521024.cn

auto p = std::make_unique<int>(5);
来源：http://ua.huixiangedu.cn

[S44] C++：引用传参
来源：http://hz.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://gn.gzmigu.cn

[S45] C++：lambda
来源：http://if.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://es.muxihuayi.cn

[S46] C++：函数模板
来源：http://hp.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mo.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://rd.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fw.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://ts.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ji.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://gq.panjiajie.cn

[S49] C++：写文件
来源：http://pc.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uu.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://tr.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hc.521024.cn

[S51] C++：显式类型转换
来源：http://mq.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://ld.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://rv.521024.cn

int size() const noexcept { return n_; }
来源：http://jl.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://sv.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://bl.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://ze.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nf.9csxet.cn

[S55] C++：结构化绑定
来源：http://os.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xz.huixiangedu.cn

[S56] C++：optional
来源：http://pb.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ah.szxytkj.cn

[S57] C++：编译期常量
来源：http://hh.shtwfgs.cn

constexpr int N = 10;
来源：http://px.hahajie.cn

[S58] C++：命名空间
来源：http://kq.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://lu.szxytkj.cn

[S59] C++：静态断言
来源：http://is.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ht.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://xq.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xz.shtwfgs.cn

================================================================================
来源：http://gd.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wq.chemitech.net.cn

================================================================================
来源：http://mu.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://kb.hnjuh.cn

println("Hello")
来源：http://ws.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://nf.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oz.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://ve.hnjuh.cn

"值: $b"
来源：http://ch.nszjky.cn

[T04] Kotlin：空安全
来源：http://qt.9csxet.cn

val n: String? = null;  n?.length
来源：http://gd.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://gx.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ms.newstarts.cn

[T06] Kotlin：集合映射
来源：http://nl.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hf.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://dn.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://go.nicolike.cn

[T08] Kotlin：数据类
来源：http://pj.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://ip.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://om.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://qi.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://mg.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wt.szxytkj.cn

[T11] Kotlin：协程
来源：http://sx.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sq.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://dq.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://uj.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://pl.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://zc.szsharing.cn

[T14] Kotlin：循环
来源：http://br.hnjuh.cn

for (i in 1..10) println(i)
来源：http://hp.shxzukj.cn

[T15] Kotlin：接口
来源：http://tr.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://kj.gzmigu.cn

[T16] Swift：Hello World
来源：http://ro.chemitech.net.cn

print("Hello")
来源：http://er.szxytkj.cn

[T17] Swift：变量与常量
来源：http://sq.9csxet.cn

var a = 1;  let b = 2
来源：http://bv.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://wi.chemitech.net.cn

"值: \(b)"
来源：http://rz.nszjky.cn

[T19] Swift：可选绑定
来源：http://ta.colortex.cn

if let n = opt { print(n) }
来源：http://kd.shtwfgs.cn

[T20] Swift：数组操作
来源：http://nt.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mz.bookmarksfly.cn

[T21] Swift：遍历
来源：http://jh.haigaiapp.cn

for x in a { print(x) }
来源：http://we.asd995.cn

[T22] Swift：字典
来源：http://if.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ge.haigaiapp.cn

[T23] Swift：函数
来源：http://xw.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kq.szxytkj.cn

[T24] Swift：闭包
来源：http://ug.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tl.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://yu.szsharing.cn

struct P { var x: Int }
来源：http://gd.colortex.cn

[T26] Swift：类与重写
来源：http://pz.9csxet.cn

class A: Base { override func f() {} }
来源：http://gw.wgjwhj.cn

[T27] Swift：错误处理
来源：http://ea.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://hy.9csxet.cn

[T28] Swift：枚举
来源：http://gz.haigaiapp.cn

enum Color { case red, green }
来源：http://fm.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://nl.nszjky.cn

guard let x = opt else { return }
来源：http://no.521024.cn

[T30] Swift：协议
来源：http://ci.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://bj.lnxyls.cn

[T31] Lua：Hello World
来源：http://kw.huanxung.cn

print("Hello")
来源：http://pj.hahajie.cn

[T32] Lua：局部变量
来源：http://eb.huanxung.cn

local a = 1
来源：http://pi.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://oi.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://of.lnxyls.cn

[T34] Lua：遍历表
来源：http://xc.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ep.hnjuh.cn

[T35] Lua：字典表
来源：http://xh.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://jj.shxzskj.cn

[T36] Lua：函数
来源：http://ra.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://ii.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://mt.9csxet.cn

"a" .. "b"
来源：http://ug.gzmigu.cn

[T38] Lua：条件
来源：http://bl.colortex.cn

if x > 0 then print("正") end
来源：http://lp.gzmigu.cn

[T39] Lua：模式匹配
来源：http://nq.bjjhwx.cn

string.find(s, "%d+")
来源：http://vt.huixiangedu.cn

[T40] Lua：元表
来源：http://po.huanxung.cn

setmetatable({}, { __index = base })
来源：http://ml.huixiangedu.cn

[T41] Perl：Hello World
来源：http://ep.nszjky.cn

print "Hello\n";
来源：http://bd.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://sl.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dm.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://pv.colortex.cn

"值: $a"
来源：http://aw.jianghongdianzi.cn

[T44] Perl：条件
来源：http://vi.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://hc.huanxung.cn

[T45] Perl：数组遍历
来源：http://yi.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://uu.hahajie.cn

[T46] Perl：哈希操作
来源：http://do.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yr.9csxet.cn

[T47] Perl：正则捕获
来源：http://pk.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bo.gzmigu.cn

[T48] Perl：正则替换
来源：http://hn.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://sr.521024.cn

[T49] Perl：函数
来源：http://dg.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://db.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://rx.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yh.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://jl.newstarts.cn

[T51] Scala：Hello World
来源：http://el.muxihuayi.cn

println("Hello")
来源：http://wp.shxzukj.cn

[T52] Scala：变量
来源：http://sz.nicolike.cn

val a = 1;  var b = 2
来源：http://gc.asd995.cn

[T53] Scala：字符串插值
来源：http://sj.wgjwhj.cn

s"值: $b"
来源：http://hk.521024.cn

[T54] Scala：集合映射
来源：http://fd.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://xe.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://wc.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://aw.wgjwhj.cn

[T56] Scala：样例类
来源：http://gx.gzmigu.cn

case class User(name: String, age: Int)
来源：http://dr.szxytkj.cn

[T57] Scala：模式匹配
来源：http://ym.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ia.shxzukj.cn

[T58] Scala：函数定义
来源：http://zd.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gd.shxzukj.cn

[T59] Scala：循环
来源：http://qo.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://ow.huanxung.cn

[T60] Scala：折叠
来源：http://fq.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ir.asd995.cn

================================================================================
来源：http://fm.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://to.hahajie.cn

================================================================================
来源：http://vc.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://je.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qv.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://mw.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xh.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://qc.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mr.shxzukj.cn

[U04] Py：变量调试打印
来源：http://fa.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vz.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://sr.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://dj.colortex.cn

[U06] Py：合并两个字典
来源：http://qb.wgjwhj.cn

{**a, **b}
来源：http://oe.hnjuh.cn

[U07] Py：反转字典键值
来源：http://cw.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://za.shxzskj.cn

[U08] Py：展平二维列表
来源：http://kh.9csxet.cn

[y for x in nested for y in x]
来源：http://ku.asd995.cn

[U09] Py：字典取最大值的键
来源：http://zi.wgjwhj.cn

max(d, key=d.get)
来源：http://jf.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://nn.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ck.gzmigu.cn

[U11] Py：生成器表达式
来源：http://ak.panjiajie.cn

(x * 2 for x in arr)
来源：http://rd.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jz.hahajie.cn

Counter(arr).most_common(3)
来源：http://mc.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://ay.newstarts.cn

deque(maxlen=10)
来源：http://zv.521024.cn

[U14] Py：分组收集到列表
来源：http://zh.panjiajie.cn

defaultdict(list)
来源：http://ee.9csxet.cn

[U15] Py：高精度计时
来源：http://tj.wgjwhj.cn

t = time.perf_counter()
来源：http://au.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://ru.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ad.bjjhwx.cn

[U17] Py：初始化日志
来源：http://ng.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://ay.yuexingan06.cn

[U18] Py：预编译正则
来源：http://rk.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://vb.hahajie.cn

[U19] Py：正则替换带回调
来源：http://gk.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fm.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://ri.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://kn.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://oe.panjiajie.cn

@contextlib.contextmanager
来源：http://xo.hahajie.cn

[U22] Py：矩阵转置
来源：http://sp.hahajie.cn

list(zip(*m))
来源：http://wa.szsharing.cn

[U23] Py：分块读取大文件
来源：http://or.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rh.panjiajie.cn

[U24] Py：路径操作
来源：http://vw.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rv.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://xv.wgjwhj.cn

csv.DictReader(f)
来源：http://rc.shxzukj.cn

[U26] Py：并发下载
来源：http://xg.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yr.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://rs.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://la.jctech888.com.cn

[U28] Py：类型别名
来源：http://kn.yuexingan06.cn

UserId = int
来源：http://eh.szxytkj.cn

[U29] Py：属性校验
来源：http://xl.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://vn.huanxung.cn

[U30] Py：数据类
来源：http://nc.shtwfgs.cn

@dataclass(slots=True)
来源：http://jj.newstarts.cn

[U31] Py：单测
来源：http://ux.muxihuayi.cn

python -m pytest -q
来源：http://nv.panjiajie.cn

[U32] Py：代码格式化
来源：http://pk.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://ar.shxzukj.cn

[U33] Py：打包发布
来源：http://fr.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://ax.nszjky.cn

[U34] Py：判断编码
来源：http://fe.huixiangedu.cn

chardet.detect(raw)
来源：http://fz.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://ew.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kw.yuexingan06.cn

[U36] Py：定时任务
来源：http://pn.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://mz.shxzukj.cn

[U37] Py：读写 Excel
来源：http://gv.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qi.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://rb.nszjky.cn

Path(__file__).resolve().parent
来源：http://uo.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://qa.panjiajie.cn

sys.stdout.isatty()
来源：http://lr.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://kj.newstarts.cn

print("err", file=sys.stderr)
来源：http://sj.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://vr.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jp.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://ve.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rg.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://fg.gzmigu.cn

namespace App\Http;
来源：http://ix.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://wq.jctech888.com.cn

declare(strict_types=1);
来源：http://er.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://ui.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://er.hnjuh.cn

[U46] PHP：可空类型
来源：http://ym.chemitech.net.cn

?string $name = null
来源：http://lh.jctech888.com.cn

[U47] PHP：联合类型
来源：http://uj.haigaiapp.cn

int|string $id
来源：http://jw.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://nv.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ba.lnxyls.cn


<!-- 参考信息 -->