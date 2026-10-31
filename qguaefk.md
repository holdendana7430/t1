代发 wailian999

#include <iostream>
来源：http://xp.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://vk.panjiajie.cn

[S32] C++：字符串
来源：http://hv.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://vg.shxzukj.cn

[S33] C++：vector 增删
来源：http://qw.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zi.gzmigu.cn

[S34] C++：遍历 vector
来源：http://ya.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://cp.gzmigu.cn

[S35] C++：map
来源：http://qv.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lg.yuexingan06.cn

[S36] C++：unordered_map
来源：http://yi.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ks.huixiangedu.cn

[S37] C++：set
来源：http://xo.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ls.nicolike.cn

[S38] C++：排序
来源：http://va.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://ob.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://el.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nq.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://aw.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ur.szsharing.cn

[S41] C++：类与构造函数
来源：http://qx.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ko.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://cs.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://no.muxihuayi.cn

[S43] C++：智能指针
来源：http://pn.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://vk.yuexingan06.cn

[S44] C++：引用传参
来源：http://bp.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://hz.panjiajie.cn

[S45] C++：lambda
来源：http://gz.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vr.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://cu.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ha.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://eu.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fm.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://zz.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gx.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://kr.jctech888.com.cn

[S49] C++：写文件
来源：http://hq.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lj.yuexingan06.cn

[S50] C++：格式化数字
来源：http://ng.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sx.lnxyls.cn

[S51] C++：显式类型转换
来源：http://tl.521024.cn

static_cast<double>(a) / b
来源：http://fg.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://cb.colortex.cn

int size() const noexcept { return n_; }
来源：http://gl.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://zy.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://az.wgjwhj.cn

[S54] C++：异常处理
来源：http://nv.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kg.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://hu.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qb.lnxyls.cn

[S56] C++：optional
来源：http://zo.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ht.szxytkj.cn

[S57] C++：编译期常量
来源：http://ne.panjiajie.cn

constexpr int N = 10;
来源：http://vp.9csxet.cn

[S58] C++：命名空间
来源：http://yo.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://qc.chemitech.net.cn

[S59] C++：静态断言
来源：http://fc.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nu.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://ur.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ee.gzmigu.cn

================================================================================
来源：http://lz.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dd.jianghongdianzi.cn

================================================================================
来源：http://hi.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://jl.wgjwhj.cn

println("Hello")
来源：http://xm.newstarts.cn

[T02] Kotlin：变量
来源：http://bp.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jc.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://pj.jianghongdianzi.cn

"值: $b"
来源：http://aq.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://he.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://tu.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://xs.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zl.hahajie.cn

[T06] Kotlin：集合映射
来源：http://ww.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ox.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://fh.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vb.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://np.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://zr.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://bl.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://ue.colortex.cn

[T10] Kotlin：默认参数
来源：http://by.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yu.asd995.cn

[T11] Kotlin：协程
来源：http://xh.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mr.hahajie.cn

[T12] Kotlin：解构声明
来源：http://dy.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://ln.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://kj.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://bi.szsharing.cn

[T14] Kotlin：循环
来源：http://ak.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://xs.jctech888.com.cn

[T15] Kotlin：接口
来源：http://tt.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://ig.nszjky.cn

[T16] Swift：Hello World
来源：http://nj.colortex.cn

print("Hello")
来源：http://uz.colortex.cn

[T17] Swift：变量与常量
来源：http://jo.szsharing.cn

var a = 1;  let b = 2
来源：http://ye.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://qw.szsharing.cn

"值: \(b)"
来源：http://nz.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://ub.nicolike.cn

if let n = opt { print(n) }
来源：http://si.yuexingan06.cn

[T20] Swift：数组操作
来源：http://wc.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tm.huixiangedu.cn

[T21] Swift：遍历
来源：http://zr.huixinmuqiang.cn

for x in a { print(x) }
来源：http://lr.chemitech.net.cn

[T22] Swift：字典
来源：http://fu.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jf.haigaiapp.cn

[T23] Swift：函数
来源：http://cj.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://if.yuexingan06.cn

[T24] Swift：闭包
来源：http://sh.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jh.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://sk.asd995.cn

struct P { var x: Int }
来源：http://fb.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://jj.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://kw.szxytkj.cn

[T27] Swift：错误处理
来源：http://dl.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://sn.521024.cn

[T28] Swift：枚举
来源：http://ta.colortex.cn

enum Color { case red, green }
来源：http://ej.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://vx.bjjhwx.cn

guard let x = opt else { return }
来源：http://ch.yuexingan06.cn

[T30] Swift：协议
来源：http://zz.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://ro.nszjky.cn

[T31] Lua：Hello World
来源：http://az.nszjky.cn

print("Hello")
来源：http://sh.lnxyls.cn

[T32] Lua：局部变量
来源：http://ma.nszjky.cn

local a = 1
来源：http://bb.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://wp.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tc.lnxyls.cn

[T34] Lua：遍历表
来源：http://ws.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kz.nicolike.cn

[T35] Lua：字典表
来源：http://ka.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://xh.szsharing.cn

[T36] Lua：函数
来源：http://ht.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://kp.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://sx.9csxet.cn

"a" .. "b"
来源：http://py.muxihuayi.cn

[T38] Lua：条件
来源：http://fm.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://wg.9csxet.cn

[T39] Lua：模式匹配
来源：http://pr.yuexingan06.cn

string.find(s, "%d+")
来源：http://yk.nszjky.cn

[T40] Lua：元表
来源：http://ij.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://xe.nicolike.cn

[T41] Perl：Hello World
来源：http://hz.colortex.cn

print "Hello\n";
来源：http://zc.lnxyls.cn

[T42] Perl：变量类型
来源：http://xo.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bh.szsharing.cn

[T43] Perl：字符串插值
来源：http://yo.hnjuh.cn

"值: $a"
来源：http://zt.521024.cn

[T44] Perl：条件
来源：http://xu.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://xh.gzmigu.cn

[T45] Perl：数组遍历
来源：http://sc.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://ob.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://oy.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rf.nicolike.cn

[T47] Perl：正则捕获
来源：http://zd.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qn.muxihuayi.cn

[T48] Perl：正则替换
来源：http://zv.lnxyls.cn

$s =~ s/old/new/g;
来源：http://up.huixiangedu.cn

[T49] Perl：函数
来源：http://jr.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kd.hahajie.cn

[T50] Perl：逐行读文件
来源：http://qq.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://un.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://yt.asd995.cn

[T51] Scala：Hello World
来源：http://eu.bookmarksfly.cn

println("Hello")
来源：http://ew.jctech888.com.cn

[T52] Scala：变量
来源：http://by.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://li.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://sp.yuntaijiaju.cn

s"值: $b"
来源：http://qp.shxzskj.cn

[T54] Scala：集合映射
来源：http://vk.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://fa.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://de.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wp.haigaiapp.cn

[T56] Scala：样例类
来源：http://eg.asd995.cn

case class User(name: String, age: Int)
来源：http://bv.nszjky.cn

[T57] Scala：模式匹配
来源：http://tq.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wr.lnxyls.cn

[T58] Scala：函数定义
来源：http://ha.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ih.shtwfgs.cn

[T59] Scala：循环
来源：http://sp.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://ny.asd995.cn

[T60] Scala：折叠
来源：http://ng.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gb.colortex.cn

================================================================================
来源：http://do.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fo.yuntaijiaju.cn

================================================================================
来源：http://fq.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://ir.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dh.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://dm.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ob.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://mt.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://go.9csxet.cn

[U04] Py：变量调试打印
来源：http://rs.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yw.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://up.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://iz.newstarts.cn

[U06] Py：合并两个字典
来源：http://xk.hnjuh.cn

{**a, **b}
来源：http://zc.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://vc.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://ut.newstarts.cn

[U08] Py：展平二维列表
来源：http://tl.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://wz.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://gp.huixinmuqiang.cn

max(d, key=d.get)
来源：http://bx.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://ku.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://co.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://na.wgjwhj.cn

(x * 2 for x in arr)
来源：http://ad.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sb.asd995.cn

Counter(arr).most_common(3)
来源：http://jo.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://pp.gzmigu.cn

deque(maxlen=10)
来源：http://nw.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://jc.szsharing.cn

defaultdict(list)
来源：http://cj.shxzukj.cn

[U15] Py：高精度计时
来源：http://sm.521024.cn

t = time.perf_counter()
来源：http://lq.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://sb.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fw.chemitech.net.cn

[U17] Py：初始化日志
来源：http://iz.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://tt.chemitech.net.cn

[U18] Py：预编译正则
来源：http://io.nszjky.cn

pat = re.compile(r"\d+")
来源：http://eh.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://kz.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tv.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://oz.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://pw.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://er.wgjwhj.cn

@contextlib.contextmanager
来源：http://ey.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://ac.yuexingan06.cn

list(zip(*m))
来源：http://ox.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://qc.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xe.nicolike.cn

[U24] Py：路径操作
来源：http://ak.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yc.colortex.cn

[U25] Py：CSV 按字典读
来源：http://yz.jianghongdianzi.cn

csv.DictReader(f)
来源：http://pf.hnjuh.cn

[U26] Py：并发下载
来源：http://jo.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uk.521024.cn

[U27] Py：异步 HTTP
来源：http://qy.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://mm.nicolike.cn

[U28] Py：类型别名
来源：http://yk.yuexingan06.cn

UserId = int
来源：http://mc.shxzukj.cn

[U29] Py：属性校验
来源：http://nl.nicolike.cn

@property 与 @x.setter 配合
来源：http://zf.jctech888.com.cn

[U30] Py：数据类
来源：http://to.yuexingan06.cn

@dataclass(slots=True)
来源：http://tv.panjiajie.cn

[U31] Py：单测
来源：http://lu.newstarts.cn

python -m pytest -q
来源：http://ea.shtwfgs.cn

[U32] Py：代码格式化
来源：http://aa.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://lg.shxzskj.cn

[U33] Py：打包发布
来源：http://at.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://vg.wgjwhj.cn

[U34] Py：判断编码
来源：http://js.shtwfgs.cn

chardet.detect(raw)
来源：http://cm.szxytkj.cn

[U35] Py：发送邮件
来源：http://ce.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vj.gzmigu.cn

[U36] Py：定时任务
来源：http://ml.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://zz.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://me.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pb.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://jb.9csxet.cn

Path(__file__).resolve().parent
来源：http://fh.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://ek.nicolike.cn

sys.stdout.isatty()
来源：http://vc.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://qu.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://or.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://rw.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ob.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://zn.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fl.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://ex.lnxyls.cn

namespace App\Http;
来源：http://sn.colortex.cn

[U44] PHP：开启严格类型
来源：http://vm.9csxet.cn

declare(strict_types=1);
来源：http://ly.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://of.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vn.gzmigu.cn

[U46] PHP：可空类型
来源：http://zc.chemitech.net.cn

?string $name = null
来源：http://oy.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://ve.shtwfgs.cn

int|string $id
来源：http://pd.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://gz.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://et.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://yj.nszjky.cn

public readonly string $name
来源：http://sj.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://qh.colortex.cn

public function __construct(private int $id) {}
来源：http://nr.nszjky.cn

[U51] PHP：数组解构
来源：http://mf.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://zg.szxytkj.cn

[U52] PHP：箭头函数
来源：http://gz.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://pk.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://ye.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://lf.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://ec.muxihuayi.cn

$obj?->method()
来源：http://vq.panjiajie.cn

[U55] PHP：match 表达式
来源：http://cm.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gv.szsharing.cn

[U56] PHP：命名参数
来源：http://qq.wgjwhj.cn

f(a: 1, b: 2)
来源：http://wf.muxihuayi.cn


<!-- 参考信息 -->