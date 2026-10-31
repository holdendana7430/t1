代发 wailian999

#include <iostream>
来源：http://wz.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://zy.gzmigu.cn

[S32] C++：字符串
来源：http://rn.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://ih.shtwfgs.cn

[S33] C++：vector 增删
来源：http://gd.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gj.szxytkj.cn

[S34] C++：遍历 vector
来源：http://oy.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://eb.colortex.cn

[S35] C++：map
来源：http://qu.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bb.hnjuh.cn

[S36] C++：unordered_map
来源：http://pq.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bm.hnjuh.cn

[S37] C++：set
来源：http://ll.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://za.wgjwhj.cn

[S38] C++：排序
来源：http://yp.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://aa.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://nq.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ld.hahajie.cn

[S40] C++：查找元素
来源：http://rq.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dt.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://mz.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ae.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://lu.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://dr.colortex.cn

[S43] C++：智能指针
来源：http://gq.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://br.haigaiapp.cn

[S44] C++：引用传参
来源：http://kq.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://yi.szxytkj.cn

[S45] C++：lambda
来源：http://fo.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cw.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://ue.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://od.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://gd.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vi.asd995.cn

[S48] C++：逐行读文件
来源：http://tg.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gp.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://ru.shxzskj.cn

[S49] C++：写文件
来源：http://dd.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cm.hnjuh.cn

[S50] C++：格式化数字
来源：http://rg.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qz.shxzukj.cn

[S51] C++：显式类型转换
来源：http://bd.haigaiapp.cn

static_cast<double>(a) / b
来源：http://qj.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://fp.colortex.cn

int size() const noexcept { return n_; }
来源：http://zf.shtwfgs.cn

[S53] C++：移动语义
来源：http://ku.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://ds.szxytkj.cn

[S54] C++：异常处理
来源：http://yc.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hb.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://ay.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lf.szsharing.cn

[S56] C++：optional
来源：http://lp.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ss.huixiangedu.cn

[S57] C++：编译期常量
来源：http://df.szsharing.cn

constexpr int N = 10;
来源：http://yk.gzmigu.cn

[S58] C++：命名空间
来源：http://hc.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://db.yuntaijiaju.cn

[S59] C++：静态断言
来源：http://gp.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://um.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://gq.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ul.szsharing.cn

================================================================================
来源：http://mn.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eq.szsharing.cn

================================================================================
来源：http://kx.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://tq.bjjhwx.cn

println("Hello")
来源：http://fz.chemitech.net.cn

[T02] Kotlin：变量
来源：http://wi.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://co.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://zu.hnjuh.cn

"值: $b"
来源：http://cm.shxzskj.cn

[T04] Kotlin：空安全
来源：http://ed.newstarts.cn

val n: String? = null;  n?.length
来源：http://po.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://mx.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zf.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://jz.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ii.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://cq.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hq.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://xm.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://vc.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://ps.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://bj.nicolike.cn

[T10] Kotlin：默认参数
来源：http://my.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rc.huanxung.cn

[T11] Kotlin：协程
来源：http://cw.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://me.nszjky.cn

[T12] Kotlin：解构声明
来源：http://py.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://vh.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://ck.newstarts.cn

val m = mapOf("a" to 1)
来源：http://fm.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://nd.nicolike.cn

for (i in 1..10) println(i)
来源：http://vr.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://fm.nszjky.cn

interface Shape { fun area(): Double }
来源：http://zb.nszjky.cn

[T16] Swift：Hello World
来源：http://qg.szxytkj.cn

print("Hello")
来源：http://nm.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://ns.szxytkj.cn

var a = 1;  let b = 2
来源：http://hm.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://ei.muxihuayi.cn

"值: \(b)"
来源：http://dh.521024.cn

[T19] Swift：可选绑定
来源：http://dt.haigaiapp.cn

if let n = opt { print(n) }
来源：http://dd.shxzskj.cn

[T20] Swift：数组操作
来源：http://yb.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://eq.newstarts.cn

[T21] Swift：遍历
来源：http://es.nszjky.cn

for x in a { print(x) }
来源：http://zj.bookmarksfly.cn

[T22] Swift：字典
来源：http://uw.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://eo.wgjwhj.cn

[T23] Swift：函数
来源：http://xn.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hk.shxzukj.cn

[T24] Swift：闭包
来源：http://cl.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.bjjhwx.cn

[T25] Swift：结构体
来源：http://bf.huixinmuqiang.cn

struct P { var x: Int }
来源：http://qy.9csxet.cn

[T26] Swift：类与重写
来源：http://wc.huanxung.cn

class A: Base { override func f() {} }
来源：http://ti.chemitech.net.cn

[T27] Swift：错误处理
来源：http://hy.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://oo.shtwfgs.cn

[T28] Swift：枚举
来源：http://ia.huixiangedu.cn

enum Color { case red, green }
来源：http://mi.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://ci.shxzukj.cn

guard let x = opt else { return }
来源：http://th.jianghongdianzi.cn

[T30] Swift：协议
来源：http://hk.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://ad.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://hx.shxzskj.cn

print("Hello")
来源：http://ww.chemitech.net.cn

[T32] Lua：局部变量
来源：http://cp.huixinmuqiang.cn

local a = 1
来源：http://bn.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://nv.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cf.colortex.cn

[T34] Lua：遍历表
来源：http://dx.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mn.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://nt.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://qt.jctech888.com.cn

[T36] Lua：函数
来源：http://el.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://pg.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://gi.nszjky.cn

"a" .. "b"
来源：http://hy.nicolike.cn

[T38] Lua：条件
来源：http://vw.nicolike.cn

if x > 0 then print("正") end
来源：http://cm.gzmigu.cn

[T39] Lua：模式匹配
来源：http://fn.nicolike.cn

string.find(s, "%d+")
来源：http://qa.bookmarksfly.cn

[T40] Lua：元表
来源：http://ig.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://xd.chemitech.net.cn

[T41] Perl：Hello World
来源：http://nu.huixinmuqiang.cn

print "Hello\n";
来源：http://qz.yuexingan06.cn

[T42] Perl：变量类型
来源：http://bc.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mi.newstarts.cn

[T43] Perl：字符串插值
来源：http://gr.bookmarksfly.cn

"值: $a"
来源：http://ou.haigaiapp.cn

[T44] Perl：条件
来源：http://ff.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://ln.hnjuh.cn

[T45] Perl：数组遍历
来源：http://ka.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://co.szsharing.cn

[T46] Perl：哈希操作
来源：http://ye.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fc.shxzskj.cn

[T47] Perl：正则捕获
来源：http://zs.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tm.panjiajie.cn

[T48] Perl：正则替换
来源：http://og.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://nj.chemitech.net.cn

[T49] Perl：函数
来源：http://tb.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zb.newstarts.cn

[T50] Perl：逐行读文件
来源：http://mr.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://aj.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://rr.chemitech.net.cn

[T51] Scala：Hello World
来源：http://uo.yuexingan06.cn

println("Hello")
来源：http://wa.hnjuh.cn

[T52] Scala：变量
来源：http://sa.shxzskj.cn

val a = 1;  var b = 2
来源：http://jm.newstarts.cn

[T53] Scala：字符串插值
来源：http://vt.newstarts.cn

s"值: $b"
来源：http://zy.gzmigu.cn

[T54] Scala：集合映射
来源：http://hx.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://mc.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://fb.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ve.gzmigu.cn

[T56] Scala：样例类
来源：http://bu.newstarts.cn

case class User(name: String, age: Int)
来源：http://ag.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://vq.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ku.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://ve.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://en.hahajie.cn

[T59] Scala：循环
来源：http://ng.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://tu.lnxyls.cn

[T60] Scala：折叠
来源：http://jk.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ej.szxytkj.cn

================================================================================
来源：http://re.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qd.jctech888.com.cn

================================================================================
来源：http://pe.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://db.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xd.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://mq.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://on.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://df.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dj.hnjuh.cn

[U04] Py：变量调试打印
来源：http://dc.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bo.hahajie.cn

[U05] Py：列表去重且保序
来源：http://ik.521024.cn

list(dict.fromkeys(arr))
来源：http://eh.hnjuh.cn

[U06] Py：合并两个字典
来源：http://ug.szsharing.cn

{**a, **b}
来源：http://ww.colortex.cn

[U07] Py：反转字典键值
来源：http://ak.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://yl.huanxung.cn

[U08] Py：展平二维列表
来源：http://wk.shtwfgs.cn

[y for x in nested for y in x]
来源：http://nk.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://vx.huixiangedu.cn

max(d, key=d.get)
来源：http://qx.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://az.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lt.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://ql.colortex.cn

(x * 2 for x in arr)
来源：http://ue.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ir.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://tl.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://ti.hahajie.cn

deque(maxlen=10)
来源：http://pt.nicolike.cn

[U14] Py：分组收集到列表
来源：http://rj.wgjwhj.cn

defaultdict(list)
来源：http://ti.gzmigu.cn

[U15] Py：高精度计时
来源：http://zz.shxzskj.cn

t = time.perf_counter()
来源：http://ma.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://cx.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rh.huanxung.cn

[U17] Py：初始化日志
来源：http://lc.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://la.nicolike.cn

[U18] Py：预编译正则
来源：http://xu.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://om.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://ij.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://br.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://hy.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://cf.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://gg.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://ot.newstarts.cn

[U22] Py：矩阵转置
来源：http://hd.nicolike.cn

list(zip(*m))
来源：http://oy.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://zp.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qe.haigaiapp.cn

[U24] Py：路径操作
来源：http://td.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://no.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://lj.muxihuayi.cn

csv.DictReader(f)
来源：http://br.shxzukj.cn

[U26] Py：并发下载
来源：http://wa.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://no.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://dj.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://by.yuexingan06.cn

[U28] Py：类型别名
来源：http://ls.asd995.cn

UserId = int
来源：http://mv.nszjky.cn

[U29] Py：属性校验
来源：http://sh.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://cm.lnxyls.cn

[U30] Py：数据类
来源：http://qm.wgjwhj.cn

@dataclass(slots=True)
来源：http://lo.hnjuh.cn

[U31] Py：单测
来源：http://zg.jctech888.com.cn

python -m pytest -q
来源：http://he.huanxung.cn

[U32] Py：代码格式化
来源：http://bj.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://op.nicolike.cn

[U33] Py：打包发布
来源：http://yp.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://hc.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://as.haigaiapp.cn

chardet.detect(raw)
来源：http://ny.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://ad.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tw.newstarts.cn

[U36] Py：定时任务
来源：http://bj.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://si.szxytkj.cn

[U37] Py：读写 Excel
来源：http://ro.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ad.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://db.szxytkj.cn

Path(__file__).resolve().parent
来源：http://nn.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://se.muxihuayi.cn

sys.stdout.isatty()
来源：http://kk.newstarts.cn

[U40] Py：打印到标准错误
来源：http://af.hahajie.cn

print("err", file=sys.stderr)
来源：http://zd.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://sw.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bd.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://nj.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pq.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://uz.hahajie.cn

namespace App\Http;
来源：http://ze.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://ip.nicolike.cn

declare(strict_types=1);
来源：http://yz.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://nb.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cs.hahajie.cn

[U46] PHP：可空类型
来源：http://tn.huixinmuqiang.cn

?string $name = null
来源：http://qo.haigaiapp.cn

[U47] PHP：联合类型
来源：http://ex.szsharing.cn

int|string $id
来源：http://ia.shxzukj.cn

[U48] PHP：纯枚举
来源：http://rd.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xr.huixiangedu.cn

[U49] PHP：只读属性
来源：http://vy.panjiajie.cn

public readonly string $name
来源：http://sd.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://gj.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://cd.panjiajie.cn

[U51] PHP：数组解构
来源：http://is.lnxyls.cn

[$a, $b] = $arr;
来源：http://no.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://jn.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://mr.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://cx.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://wk.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://xq.hahajie.cn

$obj?->method()
来源：http://bh.asd995.cn

[U55] PHP：match 表达式
来源：http://ty.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dk.521024.cn

[U56] PHP：命名参数
来源：http://ev.yuexingan06.cn

f(a: 1, b: 2)
来源：http://aa.shtwfgs.cn


<!-- 参考信息 -->