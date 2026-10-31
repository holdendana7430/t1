代发 wailian999

#include <iostream>
来源：http://pk.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://rn.panjiajie.cn

[S32] C++：字符串
来源：http://nj.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://gy.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://kt.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lt.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://uq.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://fi.jctech888.com.cn

[S35] C++：map
来源：http://sf.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ks.lnxyls.cn

[S36] C++：unordered_map
来源：http://ge.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://of.yuexingan06.cn

[S37] C++：set
来源：http://bl.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xu.jctech888.com.cn

[S38] C++：排序
来源：http://av.521024.cn

std::sort(v.begin(), v.end());
来源：http://up.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://kb.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nu.chemitech.net.cn

[S40] C++：查找元素
来源：http://yk.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vg.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://od.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uj.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://rc.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://gw.haigaiapp.cn

[S43] C++：智能指针
来源：http://jt.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://em.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://sc.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://ey.yuntaijiaju.cn

[S45] C++：lambda
来源：http://ro.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sx.shxzskj.cn

[S46] C++：函数模板
来源：http://qh.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wg.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://sh.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cz.nicolike.cn

[S48] C++：逐行读文件
来源：http://no.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wf.nszjky.cn

while (std::getline(in, line)) { }
来源：http://zt.yuntaijiaju.cn

[S49] C++：写文件
来源：http://hk.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pc.panjiajie.cn

[S50] C++：格式化数字
来源：http://mb.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bz.hahajie.cn

[S51] C++：显式类型转换
来源：http://wd.wgjwhj.cn

static_cast<double>(a) / b
来源：http://dv.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://bv.asd995.cn

int size() const noexcept { return n_; }
来源：http://ca.bjjhwx.cn

[S53] C++：移动语义
来源：http://yx.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://ss.shxzukj.cn

[S54] C++：异常处理
来源：http://hu.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tx.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://cu.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://to.lnxyls.cn

[S56] C++：optional
来源：http://pi.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jb.chemitech.net.cn

[S57] C++：编译期常量
来源：http://fi.szsharing.cn

constexpr int N = 10;
来源：http://he.shxzukj.cn

[S58] C++：命名空间
来源：http://sz.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://wh.nszjky.cn

[S59] C++：静态断言
来源：http://wi.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sh.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://tk.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fx.wgjwhj.cn

================================================================================
来源：http://yv.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gf.bjjhwx.cn

================================================================================
来源：http://rr.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://fw.521024.cn

println("Hello")
来源：http://ij.colortex.cn

[T02] Kotlin：变量
来源：http://ig.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://au.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://wk.szxytkj.cn

"值: $b"
来源：http://ht.9csxet.cn

[T04] Kotlin：空安全
来源：http://sr.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://wy.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://dz.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xf.9csxet.cn

[T06] Kotlin：集合映射
来源：http://um.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jh.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://ns.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eo.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://jf.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://gm.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://fp.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://zu.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://zs.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uv.bjjhwx.cn

[T11] Kotlin：协程
来源：http://gy.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jf.521024.cn

[T12] Kotlin：解构声明
来源：http://mb.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://py.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://lp.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://gt.szsharing.cn

[T14] Kotlin：循环
来源：http://in.panjiajie.cn

for (i in 1..10) println(i)
来源：http://xw.hnjuh.cn

[T15] Kotlin：接口
来源：http://rr.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://uv.szsharing.cn

[T16] Swift：Hello World
来源：http://mr.shxzskj.cn

print("Hello")
来源：http://cd.colortex.cn

[T17] Swift：变量与常量
来源：http://at.shxzskj.cn

var a = 1;  let b = 2
来源：http://ki.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://mt.chemitech.net.cn

"值: \(b)"
来源：http://ce.newstarts.cn

[T19] Swift：可选绑定
来源：http://lk.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://ed.shtwfgs.cn

[T20] Swift：数组操作
来源：http://of.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://li.szsharing.cn

[T21] Swift：遍历
来源：http://oe.bookmarksfly.cn

for x in a { print(x) }
来源：http://mn.lnxyls.cn

[T22] Swift：字典
来源：http://le.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://el.yuntaijiaju.cn

[T23] Swift：函数
来源：http://tp.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://za.wgjwhj.cn

[T24] Swift：闭包
来源：http://az.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pp.asd995.cn

[T25] Swift：结构体
来源：http://yw.asd995.cn

struct P { var x: Int }
来源：http://jm.yuexingan06.cn

[T26] Swift：类与重写
来源：http://cq.szsharing.cn

class A: Base { override func f() {} }
来源：http://dm.colortex.cn

[T27] Swift：错误处理
来源：http://vh.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://dk.szsharing.cn

[T28] Swift：枚举
来源：http://va.newstarts.cn

enum Color { case red, green }
来源：http://bf.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://bj.jctech888.com.cn

guard let x = opt else { return }
来源：http://tc.szxytkj.cn

[T30] Swift：协议
来源：http://ez.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://ou.colortex.cn

[T31] Lua：Hello World
来源：http://xf.szxytkj.cn

print("Hello")
来源：http://iz.muxihuayi.cn

[T32] Lua：局部变量
来源：http://ql.wgjwhj.cn

local a = 1
来源：http://kp.nicolike.cn

[T33] Lua：表（数组）
来源：http://kq.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yl.asd995.cn

[T34] Lua：遍历表
来源：http://lh.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://js.wgjwhj.cn

[T35] Lua：字典表
来源：http://aq.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://ap.jianghongdianzi.cn

[T36] Lua：函数
来源：http://us.huanxung.cn

function add(a, b) return a + b end
来源：http://ic.nicolike.cn

[T37] Lua：字符串拼接
来源：http://zf.yuntaijiaju.cn

"a" .. "b"
来源：http://up.szxytkj.cn

[T38] Lua：条件
来源：http://xf.shxzukj.cn

if x > 0 then print("正") end
来源：http://iw.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://tk.bjjhwx.cn

string.find(s, "%d+")
来源：http://rl.muxihuayi.cn

[T40] Lua：元表
来源：http://ct.521024.cn

setmetatable({}, { __index = base })
来源：http://lg.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://zu.asd995.cn

print "Hello\n";
来源：http://fe.szsharing.cn

[T42] Perl：变量类型
来源：http://pk.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wi.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://ia.shtwfgs.cn

"值: $a"
来源：http://pa.muxihuayi.cn

[T44] Perl：条件
来源：http://jr.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://lj.colortex.cn

[T45] Perl：数组遍历
来源：http://oo.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://ef.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://as.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xw.gzmigu.cn

[T47] Perl：正则捕获
来源：http://wr.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ay.hahajie.cn

[T48] Perl：正则替换
来源：http://jz.panjiajie.cn

$s =~ s/old/new/g;
来源：http://zy.szsharing.cn

[T49] Perl：函数
来源：http://kx.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ul.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://wd.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oc.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://ti.wgjwhj.cn

[T51] Scala：Hello World
来源：http://vx.huanxung.cn

println("Hello")
来源：http://na.asd995.cn

[T52] Scala：变量
来源：http://do.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://le.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://sy.huixiangedu.cn

s"值: $b"
来源：http://ob.huanxung.cn

[T54] Scala：集合映射
来源：http://qw.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ti.shxzskj.cn

[T55] Scala：集合过滤
来源：http://jn.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oz.9csxet.cn

[T56] Scala：样例类
来源：http://hy.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://ae.gzmigu.cn

[T57] Scala：模式匹配
来源：http://zl.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ak.haigaiapp.cn

[T58] Scala：函数定义
来源：http://bz.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ez.huixiangedu.cn

[T59] Scala：循环
来源：http://fp.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://gx.shtwfgs.cn

[T60] Scala：折叠
来源：http://uj.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fs.shxzukj.cn

================================================================================
来源：http://hi.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tb.jctech888.com.cn

================================================================================
来源：http://bs.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://xk.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ep.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://ji.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ro.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://qo.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rc.szsharing.cn

[U04] Py：变量调试打印
来源：http://kl.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nb.hahajie.cn

[U05] Py：列表去重且保序
来源：http://ze.newstarts.cn

list(dict.fromkeys(arr))
来源：http://bm.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://ve.yuexingan06.cn

{**a, **b}
来源：http://yt.huanxung.cn

[U07] Py：反转字典键值
来源：http://pr.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://lm.9csxet.cn

[U08] Py：展平二维列表
来源：http://sw.colortex.cn

[y for x in nested for y in x]
来源：http://bh.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://ly.yuexingan06.cn

max(d, key=d.get)
来源：http://ls.szsharing.cn

[U10] Py：按值排序字典
来源：http://sh.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zl.colortex.cn

[U11] Py：生成器表达式
来源：http://vn.szxytkj.cn

(x * 2 for x in arr)
来源：http://wm.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gp.szsharing.cn

Counter(arr).most_common(3)
来源：http://lx.nszjky.cn

[U13] Py：固定长度队列
来源：http://cf.9csxet.cn

deque(maxlen=10)
来源：http://sv.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://qz.szsharing.cn

defaultdict(list)
来源：http://kw.shxzskj.cn

[U15] Py：高精度计时
来源：http://pw.wgjwhj.cn

t = time.perf_counter()
来源：http://lj.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://ox.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://se.hnjuh.cn

[U17] Py：初始化日志
来源：http://gr.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://zk.bjjhwx.cn

[U18] Py：预编译正则
来源：http://ra.hahajie.cn

pat = re.compile(r"\d+")
来源：http://al.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://wy.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qp.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://yb.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://nl.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://yz.bjjhwx.cn

@contextlib.contextmanager
来源：http://hk.shxzukj.cn

[U22] Py：矩阵转置
来源：http://ps.521024.cn

list(zip(*m))
来源：http://lh.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://du.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ti.nicolike.cn

[U24] Py：路径操作
来源：http://ig.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://im.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://mo.bookmarksfly.cn

csv.DictReader(f)
来源：http://hs.bjjhwx.cn

[U26] Py：并发下载
来源：http://hf.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ty.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://my.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://uc.huixiangedu.cn

[U28] Py：类型别名
来源：http://ib.haigaiapp.cn

UserId = int
来源：http://mw.shxzukj.cn

[U29] Py：属性校验
来源：http://cb.gzmigu.cn

@property 与 @x.setter 配合
来源：http://kl.lnxyls.cn

[U30] Py：数据类
来源：http://io.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://hi.yuntaijiaju.cn

[U31] Py：单测
来源：http://vv.newstarts.cn

python -m pytest -q
来源：http://eo.shxzukj.cn

[U32] Py：代码格式化
来源：http://ly.huanxung.cn

ruff format . && ruff check --fix .
来源：http://bf.nicolike.cn

[U33] Py：打包发布
来源：http://eq.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://me.bjjhwx.cn

[U34] Py：判断编码
来源：http://lm.bookmarksfly.cn

chardet.detect(raw)
来源：http://dm.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://zk.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rf.hahajie.cn

[U36] Py：定时任务
来源：http://ev.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://cz.521024.cn

[U37] Py：读写 Excel
来源：http://qy.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mz.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://su.nicolike.cn

Path(__file__).resolve().parent
来源：http://se.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://rc.bookmarksfly.cn

sys.stdout.isatty()
来源：http://bn.nicolike.cn

[U40] Py：打印到标准错误
来源：http://vx.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://co.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://xu.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mh.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://sf.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dh.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://uo.521024.cn

namespace App\Http;
来源：http://hr.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://rt.jianghongdianzi.cn

declare(strict_types=1);
来源：http://ya.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://cs.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yk.yuexingan06.cn

[U46] PHP：可空类型
来源：http://yz.jianghongdianzi.cn

?string $name = null
来源：http://de.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://tm.huanxung.cn

int|string $id
来源：http://qt.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://dn.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eb.shxzukj.cn

[U49] PHP：只读属性
来源：http://dk.nicolike.cn

public readonly string $name
来源：http://yu.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://qo.shxzukj.cn

public function __construct(private int $id) {}
来源：http://cp.521024.cn

[U51] PHP：数组解构
来源：http://yh.huanxung.cn

[$a, $b] = $arr;
来源：http://zw.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://mx.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://as.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://si.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://gj.gzmigu.cn

[U54] PHP：空安全调用
来源：http://rv.szsharing.cn

$obj?->method()
来源：http://lg.nicolike.cn

[U55] PHP：match 表达式
来源：http://yn.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://id.chemitech.net.cn

[U56] PHP：命名参数
来源：http://nw.hahajie.cn

f(a: 1, b: 2)
来源：http://zk.shtwfgs.cn


<!-- 参考信息 -->