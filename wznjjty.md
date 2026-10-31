代发 wailian999

memset(a, 0, sizeof a);
来源：http://my.shxzukj.cn

[S27] C：定义常量
来源：http://qu.shxzskj.cn

const double PI = 3.14159;
来源：http://ni.shxzukj.cn

[S28] C：静态变量
来源：http://zf.yuexingan06.cn

static int counter = 0;
来源：http://pv.nszjky.cn

[S29] C：变参函数
来源：http://kg.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yu.szxytkj.cn

[S30] C：头文件保护
来源：http://zl.bookmarksfly.cn

#ifndef X_H
来源：http://bz.muxihuayi.cn

#define X_H
来源：http://lv.hahajie.cn

#endif
来源：http://eg.yuexingan06.cn

[S31] C++：Hello World
来源：http://co.panjiajie.cn

#include <iostream>
来源：http://fd.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://nl.9csxet.cn

[S32] C++：字符串
来源：http://fs.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://tx.huanxung.cn

[S33] C++：vector 增删
来源：http://je.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mc.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://yu.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://bk.9csxet.cn

[S35] C++：map
来源：http://pq.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ec.panjiajie.cn

[S36] C++：unordered_map
来源：http://li.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zw.nszjky.cn

[S37] C++：set
来源：http://as.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lv.chemitech.net.cn

[S38] C++：排序
来源：http://xs.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://do.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://lj.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fm.newstarts.cn

[S40] C++：查找元素
来源：http://gq.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ke.szsharing.cn

[S41] C++：类与构造函数
来源：http://jy.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ke.521024.cn

[S42] C++：继承与虚函数
来源：http://pt.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://yl.521024.cn

[S43] C++：智能指针
来源：http://iz.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://ix.szsharing.cn

[S44] C++：引用传参
来源：http://fb.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://sk.szxytkj.cn

[S45] C++：lambda
来源：http://ro.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://eq.hnjuh.cn

[S46] C++：函数模板
来源：http://wz.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fa.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://gx.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ck.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://fs.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pk.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://bk.huanxung.cn

[S49] C++：写文件
来源：http://vi.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ba.haigaiapp.cn

[S50] C++：格式化数字
来源：http://lg.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ja.colortex.cn

[S51] C++：显式类型转换
来源：http://xm.nszjky.cn

static_cast<double>(a) / b
来源：http://as.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://fs.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://rx.hnjuh.cn

[S53] C++：移动语义
来源：http://ps.colortex.cn

std::vector<int> w = std::move(v);
来源：http://zp.nicolike.cn

[S54] C++：异常处理
来源：http://bh.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gf.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://ye.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xn.szxytkj.cn

[S56] C++：optional
来源：http://fc.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wa.gzmigu.cn

[S57] C++：编译期常量
来源：http://iy.panjiajie.cn

constexpr int N = 10;
来源：http://aa.bjjhwx.cn

[S58] C++：命名空间
来源：http://th.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://xy.bookmarksfly.cn

[S59] C++：静态断言
来源：http://ey.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://so.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://fr.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ul.shxzskj.cn

================================================================================
来源：http://xp.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sm.lnxyls.cn

================================================================================
来源：http://fo.hahajie.cn

[T01] Kotlin：Hello World
来源：http://ns.huixiangedu.cn

println("Hello")
来源：http://ay.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://ph.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gv.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://zl.shxzskj.cn

"值: $b"
来源：http://ut.newstarts.cn

[T04] Kotlin：空安全
来源：http://ir.szsharing.cn

val n: String? = null;  n?.length
来源：http://xt.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://ye.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jg.521024.cn

[T06] Kotlin：集合映射
来源：http://pa.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bn.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://uj.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kj.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://hn.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://dy.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://pk.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://ev.9csxet.cn

[T10] Kotlin：默认参数
来源：http://gd.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vl.shtwfgs.cn

[T11] Kotlin：协程
来源：http://bt.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ho.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://lw.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://cv.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://cx.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://ak.nszjky.cn

[T14] Kotlin：循环
来源：http://zq.lnxyls.cn

for (i in 1..10) println(i)
来源：http://lc.gzmigu.cn

[T15] Kotlin：接口
来源：http://ba.newstarts.cn

interface Shape { fun area(): Double }
来源：http://ce.szxytkj.cn

[T16] Swift：Hello World
来源：http://yk.bjjhwx.cn

print("Hello")
来源：http://oi.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://zo.chemitech.net.cn

var a = 1;  let b = 2
来源：http://dn.huanxung.cn

[T18] Swift：字符串插值
来源：http://vf.nicolike.cn

"值: \(b)"
来源：http://tq.hahajie.cn

[T19] Swift：可选绑定
来源：http://zx.haigaiapp.cn

if let n = opt { print(n) }
来源：http://hf.colortex.cn

[T20] Swift：数组操作
来源：http://od.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ac.asd995.cn

[T21] Swift：遍历
来源：http://cf.jctech888.com.cn

for x in a { print(x) }
来源：http://fa.yuntaijiaju.cn

[T22] Swift：字典
来源：http://zw.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nj.shxzskj.cn

[T23] Swift：函数
来源：http://ay.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wm.shtwfgs.cn

[T24] Swift：闭包
来源：http://xg.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yt.huanxung.cn

[T25] Swift：结构体
来源：http://qx.newstarts.cn

struct P { var x: Int }
来源：http://oq.huixiangedu.cn

[T26] Swift：类与重写
来源：http://ue.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://vq.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://gs.asd995.cn

do { try f() } catch { print(error) }
来源：http://vu.gzmigu.cn

[T28] Swift：枚举
来源：http://ca.jianghongdianzi.cn

enum Color { case red, green }
来源：http://og.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://bc.colortex.cn

guard let x = opt else { return }
来源：http://oa.nszjky.cn

[T30] Swift：协议
来源：http://mn.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://nu.hahajie.cn

[T31] Lua：Hello World
来源：http://pa.gzmigu.cn

print("Hello")
来源：http://mj.hnjuh.cn

[T32] Lua：局部变量
来源：http://ej.shxzskj.cn

local a = 1
来源：http://zs.9csxet.cn

[T33] Lua：表（数组）
来源：http://mb.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ey.shxzukj.cn

[T34] Lua：遍历表
来源：http://tv.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ud.yuexingan06.cn

[T35] Lua：字典表
来源：http://yr.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://we.bjjhwx.cn

[T36] Lua：函数
来源：http://rd.muxihuayi.cn

function add(a, b) return a + b end
来源：http://la.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://wq.yuntaijiaju.cn

"a" .. "b"
来源：http://uk.nicolike.cn

[T38] Lua：条件
来源：http://wd.colortex.cn

if x > 0 then print("正") end
来源：http://qf.9csxet.cn

[T39] Lua：模式匹配
来源：http://ul.haigaiapp.cn

string.find(s, "%d+")
来源：http://gb.521024.cn

[T40] Lua：元表
来源：http://wr.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://uu.szsharing.cn

[T41] Perl：Hello World
来源：http://as.gzmigu.cn

print "Hello\n";
来源：http://fy.muxihuayi.cn

[T42] Perl：变量类型
来源：http://pl.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lk.panjiajie.cn

[T43] Perl：字符串插值
来源：http://zw.jianghongdianzi.cn

"值: $a"
来源：http://uy.bookmarksfly.cn

[T44] Perl：条件
来源：http://hn.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://th.panjiajie.cn

[T45] Perl：数组遍历
来源：http://hh.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://wm.lnxyls.cn

[T46] Perl：哈希操作
来源：http://wa.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kx.shxzskj.cn

[T47] Perl：正则捕获
来源：http://zs.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bc.shtwfgs.cn

[T48] Perl：正则替换
来源：http://wj.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://fn.hnjuh.cn

[T49] Perl：函数
来源：http://vn.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nq.nszjky.cn

[T50] Perl：逐行读文件
来源：http://xq.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ff.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://fk.shxzskj.cn

[T51] Scala：Hello World
来源：http://qu.newstarts.cn

println("Hello")
来源：http://jo.nicolike.cn

[T52] Scala：变量
来源：http://mt.newstarts.cn

val a = 1;  var b = 2
来源：http://cj.shxzskj.cn

[T53] Scala：字符串插值
来源：http://zy.szxytkj.cn

s"值: $b"
来源：http://uq.gzmigu.cn

[T54] Scala：集合映射
来源：http://vg.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://me.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://cl.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mq.hahajie.cn

[T56] Scala：样例类
来源：http://ix.nszjky.cn

case class User(name: String, age: Int)
来源：http://wg.shxzskj.cn

[T57] Scala：模式匹配
来源：http://wo.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nh.jctech888.com.cn

[T58] Scala：函数定义
来源：http://dz.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ps.hnjuh.cn

[T59] Scala：循环
来源：http://ro.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://rt.szsharing.cn

[T60] Scala：折叠
来源：http://th.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sh.lnxyls.cn

================================================================================
来源：http://hq.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zz.bookmarksfly.cn

================================================================================
来源：http://fc.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://ad.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ow.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://lw.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gb.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://ve.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mp.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://az.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gr.asd995.cn

[U05] Py：列表去重且保序
来源：http://ta.huanxung.cn

list(dict.fromkeys(arr))
来源：http://cy.521024.cn

[U06] Py：合并两个字典
来源：http://wq.huanxung.cn

{**a, **b}
来源：http://ur.nszjky.cn

[U07] Py：反转字典键值
来源：http://bj.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://uf.hnjuh.cn

[U08] Py：展平二维列表
来源：http://ju.jctech888.com.cn

[y for x in nested for y in x]
来源：http://xr.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://fy.szsharing.cn

max(d, key=d.get)
来源：http://en.hahajie.cn

[U10] Py：按值排序字典
来源：http://me.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wf.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://wc.newstarts.cn

(x * 2 for x in arr)
来源：http://hg.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rx.hahajie.cn

Counter(arr).most_common(3)
来源：http://ig.huanxung.cn

[U13] Py：固定长度队列
来源：http://nh.haigaiapp.cn

deque(maxlen=10)
来源：http://kb.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://ly.hahajie.cn

defaultdict(list)
来源：http://nl.wgjwhj.cn

[U15] Py：高精度计时
来源：http://he.chemitech.net.cn

t = time.perf_counter()
来源：http://ae.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://ey.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rs.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://up.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://lv.hahajie.cn

[U18] Py：预编译正则
来源：http://vm.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://hx.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://yh.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ao.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://qa.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://sh.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://ii.hnjuh.cn

@contextlib.contextmanager
来源：http://dr.gzmigu.cn

[U22] Py：矩阵转置
来源：http://bl.lnxyls.cn

list(zip(*m))
来源：http://xu.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://ys.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nn.shxzskj.cn

[U24] Py：路径操作
来源：http://ry.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ia.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://yq.newstarts.cn

csv.DictReader(f)
来源：http://ud.521024.cn

[U26] Py：并发下载
来源：http://qk.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rq.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://nm.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://ui.bookmarksfly.cn

[U28] Py：类型别名
来源：http://sl.521024.cn

UserId = int
来源：http://yd.chemitech.net.cn

[U29] Py：属性校验
来源：http://vz.panjiajie.cn

@property 与 @x.setter 配合
来源：http://bu.panjiajie.cn

[U30] Py：数据类
来源：http://wx.9csxet.cn

@dataclass(slots=True)
来源：http://ni.colortex.cn

[U31] Py：单测
来源：http://vu.yuexingan06.cn

python -m pytest -q
来源：http://ov.szsharing.cn

[U32] Py：代码格式化
来源：http://yf.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://ar.bjjhwx.cn

[U33] Py：打包发布
来源：http://md.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://ox.wgjwhj.cn

[U34] Py：判断编码
来源：http://ws.wgjwhj.cn

chardet.detect(raw)
来源：http://rf.szxytkj.cn

[U35] Py：发送邮件
来源：http://lo.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kl.9csxet.cn

[U36] Py：定时任务
来源：http://ja.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://ev.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://zj.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sz.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://yj.9csxet.cn

Path(__file__).resolve().parent
来源：http://gt.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://ff.521024.cn

sys.stdout.isatty()
来源：http://km.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://er.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://cx.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://id.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vh.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://ns.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ql.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://ve.521024.cn

namespace App\Http;
来源：http://hh.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://bu.bjjhwx.cn

declare(strict_types=1);
来源：http://dt.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://dl.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nb.colortex.cn

[U46] PHP：可空类型
来源：http://pe.szxytkj.cn

?string $name = null
来源：http://bg.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://sb.shtwfgs.cn

int|string $id
来源：http://jg.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://jo.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ri.jctech888.com.cn

[U49] PHP：只读属性
来源：http://lo.panjiajie.cn

public readonly string $name
来源：http://rg.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://ak.hahajie.cn

public function __construct(private int $id) {}
来源：http://aa.wgjwhj.cn


<!-- 参考信息 -->