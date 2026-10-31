代发 wailian999

#include <iostream>
来源：http://tt.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://yu.bookmarksfly.cn

[S32] C++：字符串
来源：http://qt.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://zk.hahajie.cn

[S33] C++：vector 增删
来源：http://pc.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hm.newstarts.cn

[S34] C++：遍历 vector
来源：http://rt.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://lo.nszjky.cn

[S35] C++：map
来源：http://im.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://el.asd995.cn

[S36] C++：unordered_map
来源：http://hl.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cl.9csxet.cn

[S37] C++：set
来源：http://rt.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ih.huixiangedu.cn

[S38] C++：排序
来源：http://bg.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://yo.asd995.cn

[S39] C++：自定义比较器排序
来源：http://yn.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uy.szxytkj.cn

[S40] C++：查找元素
来源：http://fv.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bl.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://et.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oj.newstarts.cn

[S42] C++：继承与虚函数
来源：http://by.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://xp.yuexingan06.cn

[S43] C++：智能指针
来源：http://kf.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://oq.yuexingan06.cn

[S44] C++：引用传参
来源：http://ar.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://pg.hnjuh.cn

[S45] C++：lambda
来源：http://ci.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qk.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://en.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lw.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://uq.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ax.colortex.cn

[S48] C++：逐行读文件
来源：http://yd.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hb.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://zn.huixinmuqiang.cn

[S49] C++：写文件
来源：http://dl.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sj.huixiangedu.cn

[S50] C++：格式化数字
来源：http://rz.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ww.hahajie.cn

[S51] C++：显式类型转换
来源：http://vk.colortex.cn

static_cast<double>(a) / b
来源：http://yz.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://nq.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://to.wgjwhj.cn

[S53] C++：移动语义
来源：http://io.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://py.chemitech.net.cn

[S54] C++：异常处理
来源：http://jq.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vx.colortex.cn

[S55] C++：结构化绑定
来源：http://bj.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kt.asd995.cn

[S56] C++：optional
来源：http://wk.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fb.huixiangedu.cn

[S57] C++：编译期常量
来源：http://zy.huanxung.cn

constexpr int N = 10;
来源：http://kc.huixiangedu.cn

[S58] C++：命名空间
来源：http://hv.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://bf.bjjhwx.cn

[S59] C++：静态断言
来源：http://ir.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gx.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://nj.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ec.panjiajie.cn

================================================================================
来源：http://du.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ay.colortex.cn

================================================================================
来源：http://bn.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://jc.haigaiapp.cn

println("Hello")
来源：http://qm.nszjky.cn

[T02] Kotlin：变量
来源：http://ci.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gt.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://kq.nszjky.cn

"值: $b"
来源：http://yn.szsharing.cn

[T04] Kotlin：空安全
来源：http://ya.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://ve.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://hk.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pm.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://wd.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zw.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://pg.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dh.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://hs.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://fw.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://ex.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://xa.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://cp.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rf.yuexingan06.cn

[T11] Kotlin：协程
来源：http://ma.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wn.szsharing.cn

[T12] Kotlin：解构声明
来源：http://fa.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://lh.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://by.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://vu.521024.cn

[T14] Kotlin：循环
来源：http://tr.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://uf.chemitech.net.cn

[T15] Kotlin：接口
来源：http://jc.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://bz.shtwfgs.cn

[T16] Swift：Hello World
来源：http://ch.nicolike.cn

print("Hello")
来源：http://ll.colortex.cn

[T17] Swift：变量与常量
来源：http://ee.lnxyls.cn

var a = 1;  let b = 2
来源：http://qe.hnjuh.cn

[T18] Swift：字符串插值
来源：http://oq.colortex.cn

"值: \(b)"
来源：http://xw.gzmigu.cn

[T19] Swift：可选绑定
来源：http://qx.huanxung.cn

if let n = opt { print(n) }
来源：http://cr.nszjky.cn

[T20] Swift：数组操作
来源：http://xm.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mv.hahajie.cn

[T21] Swift：遍历
来源：http://rn.huixinmuqiang.cn

for x in a { print(x) }
来源：http://wv.colortex.cn

[T22] Swift：字典
来源：http://on.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tb.huixinmuqiang.cn

[T23] Swift：函数
来源：http://um.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ew.bjjhwx.cn

[T24] Swift：闭包
来源：http://ed.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bq.jctech888.com.cn

[T25] Swift：结构体
来源：http://ht.wgjwhj.cn

struct P { var x: Int }
来源：http://yh.hahajie.cn

[T26] Swift：类与重写
来源：http://da.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://eg.wgjwhj.cn

[T27] Swift：错误处理
来源：http://mv.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://pg.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://yk.hnjuh.cn

enum Color { case red, green }
来源：http://vw.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://dk.gzmigu.cn

guard let x = opt else { return }
来源：http://fd.9csxet.cn

[T30] Swift：协议
来源：http://pq.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://tk.newstarts.cn

[T31] Lua：Hello World
来源：http://mj.shxzukj.cn

print("Hello")
来源：http://al.bjjhwx.cn

[T32] Lua：局部变量
来源：http://bj.wgjwhj.cn

local a = 1
来源：http://bv.hahajie.cn

[T33] Lua：表（数组）
来源：http://ac.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wl.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://sf.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uo.nszjky.cn

[T35] Lua：字典表
来源：http://dl.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://kp.lnxyls.cn

[T36] Lua：函数
来源：http://hb.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://dd.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://to.gzmigu.cn

"a" .. "b"
来源：http://tw.hahajie.cn

[T38] Lua：条件
来源：http://fz.asd995.cn

if x > 0 then print("正") end
来源：http://xi.9csxet.cn

[T39] Lua：模式匹配
来源：http://kh.hahajie.cn

string.find(s, "%d+")
来源：http://fr.shxzukj.cn

[T40] Lua：元表
来源：http://oo.szsharing.cn

setmetatable({}, { __index = base })
来源：http://xo.yuexingan06.cn

[T41] Perl：Hello World
来源：http://fi.shxzukj.cn

print "Hello\n";
来源：http://jl.panjiajie.cn

[T42] Perl：变量类型
来源：http://ca.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bx.hahajie.cn

[T43] Perl：字符串插值
来源：http://vm.yuntaijiaju.cn

"值: $a"
来源：http://gb.wgjwhj.cn

[T44] Perl：条件
来源：http://bj.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://ds.gzmigu.cn

[T45] Perl：数组遍历
来源：http://tz.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://fm.colortex.cn

[T46] Perl：哈希操作
来源：http://gw.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bj.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://vy.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ax.yuexingan06.cn

[T48] Perl：正则替换
来源：http://tr.nszjky.cn

$s =~ s/old/new/g;
来源：http://ek.lnxyls.cn

[T49] Perl：函数
来源：http://tf.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vs.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://tj.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://go.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://lv.nicolike.cn

[T51] Scala：Hello World
来源：http://pl.chemitech.net.cn

println("Hello")
来源：http://dh.yuntaijiaju.cn

[T52] Scala：变量
来源：http://ia.hnjuh.cn

val a = 1;  var b = 2
来源：http://jz.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://id.yuntaijiaju.cn

s"值: $b"
来源：http://hg.asd995.cn

[T54] Scala：集合映射
来源：http://mn.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://nn.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://zh.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ug.colortex.cn

[T56] Scala：样例类
来源：http://pw.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://fy.521024.cn

[T57] Scala：模式匹配
来源：http://zz.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ae.shxzukj.cn

[T58] Scala：函数定义
来源：http://ij.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ic.nszjky.cn

[T59] Scala：循环
来源：http://xv.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://iw.huixiangedu.cn

[T60] Scala：折叠
来源：http://sc.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zj.shtwfgs.cn

================================================================================
来源：http://ni.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zh.asd995.cn

================================================================================
来源：http://rn.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://qp.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sm.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://et.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jn.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://ge.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ca.nszjky.cn

[U04] Py：变量调试打印
来源：http://vb.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gt.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://xk.521024.cn

list(dict.fromkeys(arr))
来源：http://be.9csxet.cn

[U06] Py：合并两个字典
来源：http://jo.huanxung.cn

{**a, **b}
来源：http://oh.lnxyls.cn

[U07] Py：反转字典键值
来源：http://hv.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://vb.hnjuh.cn

[U08] Py：展平二维列表
来源：http://pl.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://lx.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://qd.chemitech.net.cn

max(d, key=d.get)
来源：http://aa.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://hc.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vy.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://wu.9csxet.cn

(x * 2 for x in arr)
来源：http://we.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bt.hnjuh.cn

Counter(arr).most_common(3)
来源：http://xr.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://nw.yuexingan06.cn

deque(maxlen=10)
来源：http://jt.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://ak.521024.cn

defaultdict(list)
来源：http://vj.hahajie.cn

[U15] Py：高精度计时
来源：http://ll.bjjhwx.cn

t = time.perf_counter()
来源：http://ay.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://zi.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dl.hnjuh.cn

[U17] Py：初始化日志
来源：http://ht.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://xy.bjjhwx.cn

[U18] Py：预编译正则
来源：http://ce.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://ek.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://ie.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mg.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://bg.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://yh.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://pa.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://bv.hahajie.cn

[U22] Py：矩阵转置
来源：http://rx.shxzukj.cn

list(zip(*m))
来源：http://fk.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://zb.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://py.szxytkj.cn

[U24] Py：路径操作
来源：http://bt.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mf.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://em.szxytkj.cn

csv.DictReader(f)
来源：http://qh.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://kl.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nb.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://qn.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://bp.jctech888.com.cn

[U28] Py：类型别名
来源：http://hr.colortex.cn

UserId = int
来源：http://dk.szxytkj.cn

[U29] Py：属性校验
来源：http://eq.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://yc.yuntaijiaju.cn

[U30] Py：数据类
来源：http://de.hnjuh.cn

@dataclass(slots=True)
来源：http://ri.wgjwhj.cn

[U31] Py：单测
来源：http://lg.nszjky.cn

python -m pytest -q
来源：http://em.521024.cn

[U32] Py：代码格式化
来源：http://hh.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://qo.shxzukj.cn

[U33] Py：打包发布
来源：http://wj.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://yk.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://jl.huixinmuqiang.cn

chardet.detect(raw)
来源：http://ig.panjiajie.cn

[U35] Py：发送邮件
来源：http://ub.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uh.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://cl.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://ek.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://hh.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cq.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://qm.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://zg.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://vt.wgjwhj.cn

sys.stdout.isatty()
来源：http://jr.521024.cn

[U40] Py：打印到标准错误
来源：http://zh.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://up.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://er.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oq.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://hb.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xm.szsharing.cn

[U43] PHP：声明命名空间
来源：http://qk.haigaiapp.cn

namespace App\Http;
来源：http://nb.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://tw.muxihuayi.cn

declare(strict_types=1);
来源：http://mi.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://yl.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zx.shtwfgs.cn

[U46] PHP：可空类型
来源：http://de.colortex.cn

?string $name = null
来源：http://zm.gzmigu.cn

[U47] PHP：联合类型
来源：http://ep.shxzskj.cn

int|string $id
来源：http://fw.szxytkj.cn

[U48] PHP：纯枚举
来源：http://cv.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sa.521024.cn

[U49] PHP：只读属性
来源：http://ly.haigaiapp.cn

public readonly string $name
来源：http://cq.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://dw.nszjky.cn

public function __construct(private int $id) {}
来源：http://hk.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://za.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://vx.lnxyls.cn

[U52] PHP：箭头函数
来源：http://up.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://mq.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://qv.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://yh.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://ph.9csxet.cn

$obj?->method()
来源：http://nn.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://lh.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://id.wgjwhj.cn

[U56] PHP：命名参数
来源：http://nx.muxihuayi.cn

f(a: 1, b: 2)
来源：http://by.jctech888.com.cn


<!-- 参考信息 -->