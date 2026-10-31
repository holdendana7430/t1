代发 wailian999

static int counter = 0;
来源：http://qo.yuntaijiaju.cn

[S29] C：变参函数
来源：http://ks.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bk.szxytkj.cn

[S30] C：头文件保护
来源：http://qa.9csxet.cn

#ifndef X_H
来源：http://sj.szsharing.cn

#define X_H
来源：http://ed.hnjuh.cn

#endif
来源：http://zg.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://pw.huixinmuqiang.cn

#include <iostream>
来源：http://tp.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://ji.chemitech.net.cn

[S32] C++：字符串
来源：http://tz.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://cy.asd995.cn

[S33] C++：vector 增删
来源：http://td.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nz.szsharing.cn

[S34] C++：遍历 vector
来源：http://wo.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://of.muxihuayi.cn

[S35] C++：map
来源：http://cc.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jb.521024.cn

[S36] C++：unordered_map
来源：http://ax.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hw.newstarts.cn

[S37] C++：set
来源：http://uv.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sm.panjiajie.cn

[S38] C++：排序
来源：http://zg.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://lg.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://jv.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jy.jctech888.com.cn

[S40] C++：查找元素
来源：http://vm.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://di.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://fe.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mi.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://ay.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://xf.shxzukj.cn

[S43] C++：智能指针
来源：http://ou.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://ws.521024.cn

[S44] C++：引用传参
来源：http://ev.521024.cn

void inc(int &x) { ++x; }
来源：http://zq.chemitech.net.cn

[S45] C++：lambda
来源：http://pq.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ne.panjiajie.cn

[S46] C++：函数模板
来源：http://xe.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fh.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://dv.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ek.9csxet.cn

[S48] C++：逐行读文件
来源：http://kc.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ht.nszjky.cn

while (std::getline(in, line)) { }
来源：http://gl.asd995.cn

[S49] C++：写文件
来源：http://gu.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ky.newstarts.cn

[S50] C++：格式化数字
来源：http://km.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vf.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://vb.muxihuayi.cn

static_cast<double>(a) / b
来源：http://te.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://tp.huanxung.cn

int size() const noexcept { return n_; }
来源：http://pb.lnxyls.cn

[S53] C++：移动语义
来源：http://mv.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://zq.huixiangedu.cn

[S54] C++：异常处理
来源：http://aa.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ai.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://ea.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tl.shxzukj.cn

[S56] C++：optional
来源：http://de.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dj.521024.cn

[S57] C++：编译期常量
来源：http://ck.szsharing.cn

constexpr int N = 10;
来源：http://ah.huanxung.cn

[S58] C++：命名空间
来源：http://zf.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://ed.jctech888.com.cn

[S59] C++：静态断言
来源：http://uw.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iq.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://pw.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ib.hnjuh.cn

================================================================================
来源：http://ue.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ev.panjiajie.cn

================================================================================
来源：http://vf.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://ox.yuntaijiaju.cn

println("Hello")
来源：http://iv.szsharing.cn

[T02] Kotlin：变量
来源：http://vg.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gl.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://tn.haigaiapp.cn

"值: $b"
来源：http://xb.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://yv.szxytkj.cn

val n: String? = null;  n?.length
来源：http://jk.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://ny.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mt.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://ad.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ez.521024.cn

[T07] Kotlin：集合过滤
来源：http://nl.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jk.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://cu.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://tb.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://pm.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://nq.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://bh.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tr.shtwfgs.cn

[T11] Kotlin：协程
来源：http://ii.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yq.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://la.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://vw.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://cy.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://mn.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://bt.nszjky.cn

for (i in 1..10) println(i)
来源：http://od.jctech888.com.cn

[T15] Kotlin：接口
来源：http://ak.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://zl.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://ex.colortex.cn

print("Hello")
来源：http://up.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://he.bjjhwx.cn

var a = 1;  let b = 2
来源：http://nd.nicolike.cn

[T18] Swift：字符串插值
来源：http://ii.521024.cn

"值: \(b)"
来源：http://ak.colortex.cn

[T19] Swift：可选绑定
来源：http://ux.nszjky.cn

if let n = opt { print(n) }
来源：http://lf.shxzskj.cn

[T20] Swift：数组操作
来源：http://hg.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sv.huixiangedu.cn

[T21] Swift：遍历
来源：http://og.jianghongdianzi.cn

for x in a { print(x) }
来源：http://jt.asd995.cn

[T22] Swift：字典
来源：http://qb.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xw.chemitech.net.cn

[T23] Swift：函数
来源：http://ib.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dv.bookmarksfly.cn

[T24] Swift：闭包
来源：http://hl.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tq.bookmarksfly.cn

[T25] Swift：结构体
来源：http://on.521024.cn

struct P { var x: Int }
来源：http://kp.szsharing.cn

[T26] Swift：类与重写
来源：http://cc.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://cb.shtwfgs.cn

[T27] Swift：错误处理
来源：http://iy.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://fy.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://ia.szxytkj.cn

enum Color { case red, green }
来源：http://od.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://we.muxihuayi.cn

guard let x = opt else { return }
来源：http://em.shxzukj.cn

[T30] Swift：协议
来源：http://yz.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://zc.shxzskj.cn

[T31] Lua：Hello World
来源：http://px.nszjky.cn

print("Hello")
来源：http://ku.huixiangedu.cn

[T32] Lua：局部变量
来源：http://ae.jianghongdianzi.cn

local a = 1
来源：http://fy.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://ut.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ns.muxihuayi.cn

[T34] Lua：遍历表
来源：http://ye.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://so.szxytkj.cn

[T35] Lua：字典表
来源：http://if.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://kf.szxytkj.cn

[T36] Lua：函数
来源：http://kb.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://td.521024.cn

[T37] Lua：字符串拼接
来源：http://zk.hahajie.cn

"a" .. "b"
来源：http://jl.yuexingan06.cn

[T38] Lua：条件
来源：http://zy.shxzukj.cn

if x > 0 then print("正") end
来源：http://xd.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://ad.yuexingan06.cn

string.find(s, "%d+")
来源：http://py.muxihuayi.cn

[T40] Lua：元表
来源：http://jy.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://lu.shtwfgs.cn

[T41] Perl：Hello World
来源：http://er.szsharing.cn

print "Hello\n";
来源：http://cz.hahajie.cn

[T42] Perl：变量类型
来源：http://jx.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kr.nicolike.cn

[T43] Perl：字符串插值
来源：http://ty.szsharing.cn

"值: $a"
来源：http://dc.huixinmuqiang.cn

[T44] Perl：条件
来源：http://nk.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://fk.shxzukj.cn

[T45] Perl：数组遍历
来源：http://jr.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://dy.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://pa.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ba.panjiajie.cn

[T47] Perl：正则捕获
来源：http://xn.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ml.colortex.cn

[T48] Perl：正则替换
来源：http://jb.colortex.cn

$s =~ s/old/new/g;
来源：http://la.huixiangedu.cn

[T49] Perl：函数
来源：http://lu.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xs.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://dr.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ly.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://xx.jctech888.com.cn

[T51] Scala：Hello World
来源：http://qq.bjjhwx.cn

println("Hello")
来源：http://aw.521024.cn

[T52] Scala：变量
来源：http://fp.huanxung.cn

val a = 1;  var b = 2
来源：http://xb.nszjky.cn

[T53] Scala：字符串插值
来源：http://gn.hnjuh.cn

s"值: $b"
来源：http://zu.szsharing.cn

[T54] Scala：集合映射
来源：http://et.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://je.gzmigu.cn

[T55] Scala：集合过滤
来源：http://zq.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bo.gzmigu.cn

[T56] Scala：样例类
来源：http://nn.9csxet.cn

case class User(name: String, age: Int)
来源：http://to.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://fk.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uf.nicolike.cn

[T58] Scala：函数定义
来源：http://lj.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sn.asd995.cn

[T59] Scala：循环
来源：http://mo.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://yo.shxzukj.cn

[T60] Scala：折叠
来源：http://jb.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ys.9csxet.cn

================================================================================
来源：http://mi.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rl.jctech888.com.cn

================================================================================
来源：http://kl.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://ey.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ia.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://ne.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nc.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://dn.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wx.newstarts.cn

[U04] Py：变量调试打印
来源：http://fw.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bj.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://gi.hahajie.cn

list(dict.fromkeys(arr))
来源：http://ws.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://si.jctech888.com.cn

{**a, **b}
来源：http://bu.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://xo.colortex.cn

{v: k for k, v in d.items()}
来源：http://bp.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://ak.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://eg.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://qk.wgjwhj.cn

max(d, key=d.get)
来源：http://cd.shxzukj.cn

[U10] Py：按值排序字典
来源：http://lw.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sf.hnjuh.cn

[U11] Py：生成器表达式
来源：http://we.huixiangedu.cn

(x * 2 for x in arr)
来源：http://xe.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lt.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://bs.9csxet.cn

[U13] Py：固定长度队列
来源：http://zl.bookmarksfly.cn

deque(maxlen=10)
来源：http://xz.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://ag.bjjhwx.cn

defaultdict(list)
来源：http://vp.9csxet.cn

[U15] Py：高精度计时
来源：http://qq.jianghongdianzi.cn

t = time.perf_counter()
来源：http://cd.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://rm.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://io.szsharing.cn

[U17] Py：初始化日志
来源：http://vx.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://aw.lnxyls.cn

[U18] Py：预编译正则
来源：http://us.colortex.cn

pat = re.compile(r"\d+")
来源：http://fv.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://pk.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://np.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://wp.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://pa.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://se.yuexingan06.cn

@contextlib.contextmanager
来源：http://gd.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://qa.nszjky.cn

list(zip(*m))
来源：http://vw.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://rg.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yf.bookmarksfly.cn

[U24] Py：路径操作
来源：http://ld.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ha.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://ow.huanxung.cn

csv.DictReader(f)
来源：http://at.bjjhwx.cn

[U26] Py：并发下载
来源：http://bj.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vp.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://bf.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://xa.szsharing.cn

[U28] Py：类型别名
来源：http://kn.bjjhwx.cn

UserId = int
来源：http://fr.muxihuayi.cn

[U29] Py：属性校验
来源：http://hc.asd995.cn

@property 与 @x.setter 配合
来源：http://yd.521024.cn

[U30] Py：数据类
来源：http://as.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://xt.hahajie.cn

[U31] Py：单测
来源：http://rl.newstarts.cn

python -m pytest -q
来源：http://pn.huixiangedu.cn

[U32] Py：代码格式化
来源：http://ip.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://em.hnjuh.cn

[U33] Py：打包发布
来源：http://rs.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://pu.panjiajie.cn

[U34] Py：判断编码
来源：http://hz.wgjwhj.cn

chardet.detect(raw)
来源：http://eu.nszjky.cn

[U35] Py：发送邮件
来源：http://vl.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vq.shtwfgs.cn

[U36] Py：定时任务
来源：http://at.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://gr.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://sl.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pz.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://qz.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://mj.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://fj.9csxet.cn

sys.stdout.isatty()
来源：http://th.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://wa.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://ld.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://em.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vz.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ii.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ej.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://mc.shxzukj.cn

namespace App\Http;
来源：http://al.9csxet.cn

[U44] PHP：开启严格类型
来源：http://sy.gzmigu.cn

declare(strict_types=1);
来源：http://dw.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://mp.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kb.panjiajie.cn

[U46] PHP：可空类型
来源：http://hl.asd995.cn

?string $name = null
来源：http://hn.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://io.yuntaijiaju.cn

int|string $id
来源：http://ro.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://bv.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cq.shxzukj.cn

[U49] PHP：只读属性
来源：http://dw.wgjwhj.cn

public readonly string $name
来源：http://vc.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://zx.nicolike.cn

public function __construct(private int $id) {}
来源：http://zu.bjjhwx.cn

[U51] PHP：数组解构
来源：http://rb.nicolike.cn

[$a, $b] = $arr;
来源：http://yf.colortex.cn

[U52] PHP：箭头函数
来源：http://vq.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://ug.colortex.cn


<!-- 参考信息 -->