代发 wailian999

static int counter = 0;
来源：http://ow.jctech888.com.cn

[S29] C：变参函数
来源：http://gc.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zp.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://kh.huixiangedu.cn

#ifndef X_H
来源：http://na.yuexingan06.cn

#define X_H
来源：http://td.bjjhwx.cn

#endif
来源：http://fu.haigaiapp.cn

[S31] C++：Hello World
来源：http://sp.panjiajie.cn

#include <iostream>
来源：http://lv.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://sq.shxzskj.cn

[S32] C++：字符串
来源：http://fe.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://ws.gzmigu.cn

[S33] C++：vector 增删
来源：http://sa.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xp.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://cx.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://qq.colortex.cn

[S35] C++：map
来源：http://qa.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nn.nicolike.cn

[S36] C++：unordered_map
来源：http://at.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yw.shxzukj.cn

[S37] C++：set
来源：http://sa.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ww.bookmarksfly.cn

[S38] C++：排序
来源：http://ya.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://do.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://ko.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aj.bookmarksfly.cn

[S40] C++：查找元素
来源：http://al.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mw.gzmigu.cn

[S41] C++：类与构造函数
来源：http://vu.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vc.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://ca.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://kf.muxihuayi.cn

[S43] C++：智能指针
来源：http://tk.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://jb.colortex.cn

[S44] C++：引用传参
来源：http://uo.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://cu.huixiangedu.cn

[S45] C++：lambda
来源：http://vm.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gq.nicolike.cn

[S46] C++：函数模板
来源：http://vi.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ep.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://ea.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fi.hnjuh.cn

[S48] C++：逐行读文件
来源：http://ls.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hc.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://xu.muxihuayi.cn

[S49] C++：写文件
来源：http://dy.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://av.shxzskj.cn

[S50] C++：格式化数字
来源：http://yw.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xi.9csxet.cn

[S51] C++：显式类型转换
来源：http://wa.nszjky.cn

static_cast<double>(a) / b
来源：http://rl.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://mr.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://qg.nszjky.cn

[S53] C++：移动语义
来源：http://ot.asd995.cn

std::vector<int> w = std::move(v);
来源：http://pl.wgjwhj.cn

[S54] C++：异常处理
来源：http://xd.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://af.hnjuh.cn

[S55] C++：结构化绑定
来源：http://ge.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uf.9csxet.cn

[S56] C++：optional
来源：http://ri.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mc.huixiangedu.cn

[S57] C++：编译期常量
来源：http://nd.szsharing.cn

constexpr int N = 10;
来源：http://bu.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://nz.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://cy.shtwfgs.cn

[S59] C++：静态断言
来源：http://an.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rn.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://yh.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mf.huanxung.cn

================================================================================
来源：http://bi.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hn.bjjhwx.cn

================================================================================
来源：http://ni.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://mw.yuntaijiaju.cn

println("Hello")
来源：http://oc.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://bh.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://to.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://vo.panjiajie.cn

"值: $b"
来源：http://bs.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://yt.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://fr.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://vb.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wa.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://cf.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ya.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://zo.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nc.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://jd.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://mu.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://de.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://nu.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://xg.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sz.szsharing.cn

[T11] Kotlin：协程
来源：http://we.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wm.huanxung.cn

[T12] Kotlin：解构声明
来源：http://dv.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://hl.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://ti.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://yt.huanxung.cn

[T14] Kotlin：循环
来源：http://kw.hnjuh.cn

for (i in 1..10) println(i)
来源：http://vv.shxzskj.cn

[T15] Kotlin：接口
来源：http://qz.nszjky.cn

interface Shape { fun area(): Double }
来源：http://uz.nicolike.cn

[T16] Swift：Hello World
来源：http://je.hnjuh.cn

print("Hello")
来源：http://no.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://cb.shxzukj.cn

var a = 1;  let b = 2
来源：http://dg.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://bm.chemitech.net.cn

"值: \(b)"
来源：http://wi.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://mq.hahajie.cn

if let n = opt { print(n) }
来源：http://ri.nicolike.cn

[T20] Swift：数组操作
来源：http://zn.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ac.bookmarksfly.cn

[T21] Swift：遍历
来源：http://xh.szsharing.cn

for x in a { print(x) }
来源：http://bi.yuntaijiaju.cn

[T22] Swift：字典
来源：http://my.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cl.lnxyls.cn

[T23] Swift：函数
来源：http://ww.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tj.colortex.cn

[T24] Swift：闭包
来源：http://po.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://na.shxzskj.cn

[T25] Swift：结构体
来源：http://ci.colortex.cn

struct P { var x: Int }
来源：http://ry.gzmigu.cn

[T26] Swift：类与重写
来源：http://ve.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://ju.hnjuh.cn

[T27] Swift：错误处理
来源：http://id.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://gk.asd995.cn

[T28] Swift：枚举
来源：http://ex.shxzukj.cn

enum Color { case red, green }
来源：http://gf.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://zq.gzmigu.cn

guard let x = opt else { return }
来源：http://io.shxzukj.cn

[T30] Swift：协议
来源：http://rd.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://zh.muxihuayi.cn

[T31] Lua：Hello World
来源：http://li.asd995.cn

print("Hello")
来源：http://cu.lnxyls.cn

[T32] Lua：局部变量
来源：http://tb.hnjuh.cn

local a = 1
来源：http://rz.521024.cn

[T33] Lua：表（数组）
来源：http://rg.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yk.yuexingan06.cn

[T34] Lua：遍历表
来源：http://ap.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jf.huanxung.cn

[T35] Lua：字典表
来源：http://yy.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://hk.shxzukj.cn

[T36] Lua：函数
来源：http://qh.521024.cn

function add(a, b) return a + b end
来源：http://kq.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://cz.chemitech.net.cn

"a" .. "b"
来源：http://zd.hahajie.cn

[T38] Lua：条件
来源：http://iy.gzmigu.cn

if x > 0 then print("正") end
来源：http://bp.colortex.cn

[T39] Lua：模式匹配
来源：http://fv.hnjuh.cn

string.find(s, "%d+")
来源：http://nq.huixinmuqiang.cn

[T40] Lua：元表
来源：http://dj.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://xi.shxzskj.cn

[T41] Perl：Hello World
来源：http://ab.shxzskj.cn

print "Hello\n";
来源：http://jc.bjjhwx.cn

[T42] Perl：变量类型
来源：http://om.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tk.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://ca.gzmigu.cn

"值: $a"
来源：http://zk.szxytkj.cn

[T44] Perl：条件
来源：http://iq.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://eh.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://ob.colortex.cn

for my $x (@arr) { print $x; }
来源：http://pl.9csxet.cn

[T46] Perl：哈希操作
来源：http://rc.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://om.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://os.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ij.nicolike.cn

[T48] Perl：正则替换
来源：http://et.huanxung.cn

$s =~ s/old/new/g;
来源：http://cq.szxytkj.cn

[T49] Perl：函数
来源：http://nr.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jm.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://xz.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://so.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://da.hnjuh.cn

[T51] Scala：Hello World
来源：http://nn.huixinmuqiang.cn

println("Hello")
来源：http://jj.szsharing.cn

[T52] Scala：变量
来源：http://iw.newstarts.cn

val a = 1;  var b = 2
来源：http://pk.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://vw.hahajie.cn

s"值: $b"
来源：http://qi.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://nb.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://dj.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://kn.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gf.jctech888.com.cn

[T56] Scala：样例类
来源：http://rc.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://go.szxytkj.cn

[T57] Scala：模式匹配
来源：http://el.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dj.wgjwhj.cn

[T58] Scala：函数定义
来源：http://kk.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bj.wgjwhj.cn

[T59] Scala：循环
来源：http://rj.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://qh.newstarts.cn

[T60] Scala：折叠
来源：http://sw.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ts.lnxyls.cn

================================================================================
来源：http://ow.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zk.bookmarksfly.cn

================================================================================
来源：http://wu.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://kn.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://in.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://at.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lw.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://ra.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xf.521024.cn

[U04] Py：变量调试打印
来源：http://jw.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gi.newstarts.cn

[U05] Py：列表去重且保序
来源：http://zk.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://ra.szsharing.cn

[U06] Py：合并两个字典
来源：http://vy.9csxet.cn

{**a, **b}
来源：http://zj.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://bd.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://bi.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://fw.nszjky.cn

[y for x in nested for y in x]
来源：http://vw.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://ln.yuexingan06.cn

max(d, key=d.get)
来源：http://si.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://gj.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gl.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://cx.gzmigu.cn

(x * 2 for x in arr)
来源：http://dr.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://um.lnxyls.cn

Counter(arr).most_common(3)
来源：http://nz.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://pz.muxihuayi.cn

deque(maxlen=10)
来源：http://in.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://kk.haigaiapp.cn

defaultdict(list)
来源：http://vt.yuexingan06.cn

[U15] Py：高精度计时
来源：http://yo.wgjwhj.cn

t = time.perf_counter()
来源：http://sk.szsharing.cn

[U16] Py：命令行参数解析
来源：http://gb.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hi.jctech888.com.cn

[U17] Py：初始化日志
来源：http://bh.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://ol.huixiangedu.cn

[U18] Py：预编译正则
来源：http://ik.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://xu.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://af.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ho.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://zw.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://ff.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://wx.newstarts.cn

@contextlib.contextmanager
来源：http://ed.szxytkj.cn

[U22] Py：矩阵转置
来源：http://hr.huanxung.cn

list(zip(*m))
来源：http://zn.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://ju.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ta.nicolike.cn

[U24] Py：路径操作
来源：http://tl.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hy.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://nv.yuntaijiaju.cn

csv.DictReader(f)
来源：http://oy.nicolike.cn

[U26] Py：并发下载
来源：http://ba.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dd.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://sx.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://pl.521024.cn

[U28] Py：类型别名
来源：http://qt.jctech888.com.cn

UserId = int
来源：http://gu.muxihuayi.cn

[U29] Py：属性校验
来源：http://ht.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://ua.huixinmuqiang.cn

[U30] Py：数据类
来源：http://df.hnjuh.cn

@dataclass(slots=True)
来源：http://wl.jctech888.com.cn

[U31] Py：单测
来源：http://cm.haigaiapp.cn

python -m pytest -q
来源：http://sm.gzmigu.cn

[U32] Py：代码格式化
来源：http://qb.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://or.shtwfgs.cn

[U33] Py：打包发布
来源：http://pn.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://vh.9csxet.cn

[U34] Py：判断编码
来源：http://hq.jctech888.com.cn

chardet.detect(raw)
来源：http://fx.wgjwhj.cn

[U35] Py：发送邮件
来源：http://sw.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fj.chemitech.net.cn

[U36] Py：定时任务
来源：http://jx.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://lj.szxytkj.cn

[U37] Py：读写 Excel
来源：http://gz.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fe.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://ae.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://go.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://qh.wgjwhj.cn

sys.stdout.isatty()
来源：http://yg.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://dv.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://gh.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://cs.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://az.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://hu.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mj.hahajie.cn

[U43] PHP：声明命名空间
来源：http://ff.bookmarksfly.cn

namespace App\Http;
来源：http://uh.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://lf.yuntaijiaju.cn

declare(strict_types=1);
来源：http://qj.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://wh.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jc.9csxet.cn

[U46] PHP：可空类型
来源：http://vu.hnjuh.cn

?string $name = null
来源：http://sc.lnxyls.cn

[U47] PHP：联合类型
来源：http://uf.bookmarksfly.cn

int|string $id
来源：http://yx.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://eq.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mw.hahajie.cn

[U49] PHP：只读属性
来源：http://jp.hnjuh.cn

public readonly string $name
来源：http://nn.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://dl.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://ot.huixiangedu.cn

[U51] PHP：数组解构
来源：http://gs.newstarts.cn

[$a, $b] = $arr;
来源：http://yc.panjiajie.cn

[U52] PHP：箭头函数
来源：http://qq.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://vf.nszjky.cn


<!-- 参考信息 -->