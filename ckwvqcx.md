代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kk.chemitech.net.cn

[S25] C：内存拷贝
来源：http://os.nicolike.cn

memcpy(dst, src, n);
来源：http://xp.wgjwhj.cn

[S26] C：内存清零
来源：http://kw.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://lr.nszjky.cn

[S27] C：定义常量
来源：http://nu.wgjwhj.cn

const double PI = 3.14159;
来源：http://zr.nszjky.cn

[S28] C：静态变量
来源：http://kg.huixiangedu.cn

static int counter = 0;
来源：http://ym.wgjwhj.cn

[S29] C：变参函数
来源：http://iq.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hk.gzmigu.cn

[S30] C：头文件保护
来源：http://tq.haigaiapp.cn

#ifndef X_H
来源：http://gl.huanxung.cn

#define X_H
来源：http://fz.muxihuayi.cn

#endif
来源：http://ik.bjjhwx.cn

[S31] C++：Hello World
来源：http://uv.panjiajie.cn

#include <iostream>
来源：http://dc.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://vb.huixiangedu.cn

[S32] C++：字符串
来源：http://nk.asd995.cn

std::string s = "hi";  s += "!";
来源：http://ov.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://ac.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xy.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://sj.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://mq.colortex.cn

[S35] C++：map
来源：http://zk.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fe.521024.cn

[S36] C++：unordered_map
来源：http://bx.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qu.chemitech.net.cn

[S37] C++：set
来源：http://xt.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cf.shtwfgs.cn

[S38] C++：排序
来源：http://yv.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://hd.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://wp.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sq.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://ch.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cq.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://yr.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://is.hahajie.cn

[S42] C++：继承与虚函数
来源：http://sk.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://ig.shxzskj.cn

[S43] C++：智能指针
来源：http://pi.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://hf.szxytkj.cn

[S44] C++：引用传参
来源：http://sk.521024.cn

void inc(int &x) { ++x; }
来源：http://bn.yuntaijiaju.cn

[S45] C++：lambda
来源：http://vi.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ys.muxihuayi.cn

[S46] C++：函数模板
来源：http://zy.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sp.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://dl.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sg.nicolike.cn

[S48] C++：逐行读文件
来源：http://ry.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zz.colortex.cn

while (std::getline(in, line)) { }
来源：http://eu.jianghongdianzi.cn

[S49] C++：写文件
来源：http://su.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ks.huixiangedu.cn

[S50] C++：格式化数字
来源：http://tg.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://no.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://of.hnjuh.cn

static_cast<double>(a) / b
来源：http://wz.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://qi.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://he.szsharing.cn

[S53] C++：移动语义
来源：http://ws.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://ed.huixiangedu.cn

[S54] C++：异常处理
来源：http://ob.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pl.szxytkj.cn

[S55] C++：结构化绑定
来源：http://ic.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pw.bookmarksfly.cn

[S56] C++：optional
来源：http://oa.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ov.shxzskj.cn

[S57] C++：编译期常量
来源：http://bq.yuexingan06.cn

constexpr int N = 10;
来源：http://ez.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://fj.521024.cn

namespace ns { int f() { return 1; } }
来源：http://hv.haigaiapp.cn

[S59] C++：静态断言
来源：http://iy.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uk.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://tz.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cg.muxihuayi.cn

================================================================================
来源：http://ke.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nk.szxytkj.cn

================================================================================
来源：http://sd.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://ke.nicolike.cn

println("Hello")
来源：http://he.shxzukj.cn

[T02] Kotlin：变量
来源：http://ac.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://on.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://gj.haigaiapp.cn

"值: $b"
来源：http://us.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://rr.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://bk.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://jk.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ba.asd995.cn

[T06] Kotlin：集合映射
来源：http://tk.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ew.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://zo.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ba.huanxung.cn

[T08] Kotlin：数据类
来源：http://fi.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://vr.colortex.cn

[T09] Kotlin：扩展函数
来源：http://ui.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://bj.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://mx.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ap.521024.cn

[T11] Kotlin：协程
来源：http://wu.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mg.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://ke.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://ph.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://wg.newstarts.cn

val m = mapOf("a" to 1)
来源：http://rj.jctech888.com.cn

[T14] Kotlin：循环
来源：http://ek.colortex.cn

for (i in 1..10) println(i)
来源：http://iz.colortex.cn

[T15] Kotlin：接口
来源：http://pi.hahajie.cn

interface Shape { fun area(): Double }
来源：http://qd.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://gj.szsharing.cn

print("Hello")
来源：http://gl.colortex.cn

[T17] Swift：变量与常量
来源：http://pl.szxytkj.cn

var a = 1;  let b = 2
来源：http://lx.nicolike.cn

[T18] Swift：字符串插值
来源：http://ya.colortex.cn

"值: \(b)"
来源：http://yk.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://sa.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://pp.hnjuh.cn

[T20] Swift：数组操作
来源：http://zx.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ga.szsharing.cn

[T21] Swift：遍历
来源：http://zr.gzmigu.cn

for x in a { print(x) }
来源：http://vy.huixinmuqiang.cn

[T22] Swift：字典
来源：http://ql.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zh.gzmigu.cn

[T23] Swift：函数
来源：http://ca.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oi.asd995.cn

[T24] Swift：闭包
来源：http://pv.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ld.bookmarksfly.cn

[T25] Swift：结构体
来源：http://ri.asd995.cn

struct P { var x: Int }
来源：http://yf.panjiajie.cn

[T26] Swift：类与重写
来源：http://dp.hnjuh.cn

class A: Base { override func f() {} }
来源：http://px.muxihuayi.cn

[T27] Swift：错误处理
来源：http://bh.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://vv.muxihuayi.cn

[T28] Swift：枚举
来源：http://uh.hahajie.cn

enum Color { case red, green }
来源：http://fn.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://yh.shtwfgs.cn

guard let x = opt else { return }
来源：http://qq.szxytkj.cn

[T30] Swift：协议
来源：http://ip.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://lo.huixiangedu.cn

[T31] Lua：Hello World
来源：http://fe.521024.cn

print("Hello")
来源：http://wu.hnjuh.cn

[T32] Lua：局部变量
来源：http://dk.nicolike.cn

local a = 1
来源：http://ph.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://ss.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qb.9csxet.cn

[T34] Lua：遍历表
来源：http://yk.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://at.jctech888.com.cn

[T35] Lua：字典表
来源：http://br.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://wn.shtwfgs.cn

[T36] Lua：函数
来源：http://ky.lnxyls.cn

function add(a, b) return a + b end
来源：http://ag.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://vs.lnxyls.cn

"a" .. "b"
来源：http://jo.bjjhwx.cn

[T38] Lua：条件
来源：http://ma.muxihuayi.cn

if x > 0 then print("正") end
来源：http://gz.szxytkj.cn

[T39] Lua：模式匹配
来源：http://kj.gzmigu.cn

string.find(s, "%d+")
来源：http://co.wgjwhj.cn

[T40] Lua：元表
来源：http://az.szsharing.cn

setmetatable({}, { __index = base })
来源：http://sc.chemitech.net.cn

[T41] Perl：Hello World
来源：http://ot.nicolike.cn

print "Hello\n";
来源：http://bd.chemitech.net.cn

[T42] Perl：变量类型
来源：http://ex.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cw.hnjuh.cn

[T43] Perl：字符串插值
来源：http://yc.521024.cn

"值: $a"
来源：http://po.yuntaijiaju.cn

[T44] Perl：条件
来源：http://yh.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://cz.9csxet.cn

[T45] Perl：数组遍历
来源：http://ca.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://uz.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://yn.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ko.gzmigu.cn

[T47] Perl：正则捕获
来源：http://rz.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nh.jctech888.com.cn

[T48] Perl：正则替换
来源：http://vh.asd995.cn

$s =~ s/old/new/g;
来源：http://jm.shxzskj.cn

[T49] Perl：函数
来源：http://dq.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cl.nszjky.cn

[T50] Perl：逐行读文件
来源：http://ve.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ql.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://kq.hnjuh.cn

[T51] Scala：Hello World
来源：http://wx.yuntaijiaju.cn

println("Hello")
来源：http://mk.shxzukj.cn

[T52] Scala：变量
来源：http://ge.asd995.cn

val a = 1;  var b = 2
来源：http://qu.panjiajie.cn

[T53] Scala：字符串插值
来源：http://fq.szxytkj.cn

s"值: $b"
来源：http://wl.bjjhwx.cn

[T54] Scala：集合映射
来源：http://bu.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://mz.asd995.cn

[T55] Scala：集合过滤
来源：http://qe.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fd.szsharing.cn

[T56] Scala：样例类
来源：http://kg.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://ne.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://fo.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yh.521024.cn

[T58] Scala：函数定义
来源：http://ik.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dv.shtwfgs.cn

[T59] Scala：循环
来源：http://xc.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://lc.colortex.cn

[T60] Scala：折叠
来源：http://pz.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yi.newstarts.cn

================================================================================
来源：http://oj.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jh.shxzukj.cn

================================================================================
来源：http://ne.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://ca.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ee.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://nw.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zd.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://jh.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nd.9csxet.cn

[U04] Py：变量调试打印
来源：http://tk.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hm.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://kc.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://ok.hahajie.cn

[U06] Py：合并两个字典
来源：http://yw.huixinmuqiang.cn

{**a, **b}
来源：http://ax.hnjuh.cn

[U07] Py：反转字典键值
来源：http://vv.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://qs.9csxet.cn

[U08] Py：展平二维列表
来源：http://mc.shxzskj.cn

[y for x in nested for y in x]
来源：http://ia.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://is.chemitech.net.cn

max(d, key=d.get)
来源：http://at.nicolike.cn

[U10] Py：按值排序字典
来源：http://fy.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cy.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://xt.yuexingan06.cn

(x * 2 for x in arr)
来源：http://to.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fw.gzmigu.cn

Counter(arr).most_common(3)
来源：http://hb.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://lr.shxzskj.cn

deque(maxlen=10)
来源：http://lp.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://kt.hnjuh.cn

defaultdict(list)
来源：http://se.gzmigu.cn

[U15] Py：高精度计时
来源：http://bu.huixiangedu.cn

t = time.perf_counter()
来源：http://gk.nszjky.cn

[U16] Py：命令行参数解析
来源：http://jg.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xk.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://wf.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://ne.shtwfgs.cn

[U18] Py：预编译正则
来源：http://aw.nicolike.cn

pat = re.compile(r"\d+")
来源：http://gg.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://aa.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qo.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://vd.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://wp.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://nd.yuexingan06.cn

@contextlib.contextmanager
来源：http://wr.nicolike.cn

[U22] Py：矩阵转置
来源：http://dk.nicolike.cn

list(zip(*m))
来源：http://no.huanxung.cn

[U23] Py：分块读取大文件
来源：http://ip.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fq.521024.cn

[U24] Py：路径操作
来源：http://ar.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pl.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://ry.newstarts.cn

csv.DictReader(f)
来源：http://qb.wgjwhj.cn

[U26] Py：并发下载
来源：http://hb.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vv.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://qh.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://kn.chemitech.net.cn

[U28] Py：类型别名
来源：http://ah.huixinmuqiang.cn

UserId = int
来源：http://wu.hnjuh.cn

[U29] Py：属性校验
来源：http://ko.lnxyls.cn

@property 与 @x.setter 配合
来源：http://pq.huanxung.cn

[U30] Py：数据类
来源：http://pg.nszjky.cn

@dataclass(slots=True)
来源：http://na.huixiangedu.cn

[U31] Py：单测
来源：http://km.yuexingan06.cn

python -m pytest -q
来源：http://tg.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://il.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://ch.huixiangedu.cn

[U33] Py：打包发布
来源：http://ko.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://sx.nszjky.cn

[U34] Py：判断编码
来源：http://ls.9csxet.cn

chardet.detect(raw)
来源：http://is.yuexingan06.cn

[U35] Py：发送邮件
来源：http://ln.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uy.panjiajie.cn

[U36] Py：定时任务
来源：http://rn.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://up.nszjky.cn

[U37] Py：读写 Excel
来源：http://lp.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ks.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://zo.gzmigu.cn

Path(__file__).resolve().parent
来源：http://mg.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://qj.nszjky.cn

sys.stdout.isatty()
来源：http://qb.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://uq.nicolike.cn

print("err", file=sys.stderr)
来源：http://kp.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://aj.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kz.chemitech.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://zt.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tc.nszjky.cn

[U43] PHP：声明命名空间
来源：http://hl.hnjuh.cn

namespace App\Http;
来源：http://ws.521024.cn

[U44] PHP：开启严格类型
来源：http://cg.newstarts.cn

declare(strict_types=1);
来源：http://zg.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://et.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://no.jctech888.com.cn

[U46] PHP：可空类型
来源：http://hi.yuexingan06.cn

?string $name = null
来源：http://qm.muxihuayi.cn

[U47] PHP：联合类型
来源：http://hp.9csxet.cn

int|string $id
来源：http://hd.panjiajie.cn

[U48] PHP：纯枚举
来源：http://ya.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hs.gzmigu.cn


<!-- 参考信息 -->