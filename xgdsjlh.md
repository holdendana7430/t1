代发 wailian999

#ifndef X_H
来源：http://nq.chemitech.net.cn

#define X_H
来源：http://sr.haigaiapp.cn

#endif
来源：http://xi.yuexingan06.cn

[S31] C++：Hello World
来源：http://bt.muxihuayi.cn

#include <iostream>
来源：http://vs.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://dj.shxzskj.cn

[S32] C++：字符串
来源：http://fy.colortex.cn

std::string s = "hi";  s += "!";
来源：http://rf.shtwfgs.cn

[S33] C++：vector 增删
来源：http://is.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ls.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://rs.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://rn.521024.cn

[S35] C++：map
来源：http://rf.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://od.szxytkj.cn

[S36] C++：unordered_map
来源：http://jh.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nr.gzmigu.cn

[S37] C++：set
来源：http://fo.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qw.colortex.cn

[S38] C++：排序
来源：http://qn.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://qd.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://ro.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vk.nszjky.cn

[S40] C++：查找元素
来源：http://em.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qx.shxzskj.cn

[S41] C++：类与构造函数
来源：http://cy.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eq.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://fq.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://ms.bookmarksfly.cn

[S43] C++：智能指针
来源：http://pp.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://yo.asd995.cn

[S44] C++：引用传参
来源：http://im.szsharing.cn

void inc(int &x) { ++x; }
来源：http://eg.asd995.cn

[S45] C++：lambda
来源：http://sn.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dp.szsharing.cn

[S46] C++：函数模板
来源：http://rn.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tp.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://xc.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bi.nszjky.cn

[S48] C++：逐行读文件
来源：http://zi.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jn.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://to.9csxet.cn

[S49] C++：写文件
来源：http://px.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kp.hahajie.cn

[S50] C++：格式化数字
来源：http://ba.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cd.nicolike.cn

[S51] C++：显式类型转换
来源：http://jo.gzmigu.cn

static_cast<double>(a) / b
来源：http://xr.asd995.cn

[S52] C++：const 与 noexcept
来源：http://rq.asd995.cn

int size() const noexcept { return n_; }
来源：http://sc.yuexingan06.cn

[S53] C++：移动语义
来源：http://pw.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://wy.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://zj.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rz.szsharing.cn

[S55] C++：结构化绑定
来源：http://zr.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ip.yuntaijiaju.cn

[S56] C++：optional
来源：http://sl.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://az.shxzukj.cn

[S57] C++：编译期常量
来源：http://tt.wgjwhj.cn

constexpr int N = 10;
来源：http://gi.colortex.cn

[S58] C++：命名空间
来源：http://uq.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://ob.shxzukj.cn

[S59] C++：静态断言
来源：http://wp.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ha.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://hk.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nb.panjiajie.cn

================================================================================
来源：http://qz.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ec.gzmigu.cn

================================================================================
来源：http://li.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://mz.colortex.cn

println("Hello")
来源：http://go.szsharing.cn

[T02] Kotlin：变量
来源：http://ob.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cx.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://xt.hnjuh.cn

"值: $b"
来源：http://bt.panjiajie.cn

[T04] Kotlin：空安全
来源：http://eg.lnxyls.cn

val n: String? = null;  n?.length
来源：http://ww.colortex.cn

[T05] Kotlin：when 表达式
来源：http://pc.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hj.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://sz.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yv.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://yl.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nj.shxzskj.cn

[T08] Kotlin：数据类
来源：http://ef.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://ls.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://sn.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://qo.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://yo.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vp.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://zo.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vj.nszjky.cn

[T12] Kotlin：解构声明
来源：http://qe.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://np.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://bl.nszjky.cn

val m = mapOf("a" to 1)
来源：http://nq.colortex.cn

[T14] Kotlin：循环
来源：http://qr.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://zb.asd995.cn

[T15] Kotlin：接口
来源：http://vw.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://jq.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://qc.huanxung.cn

print("Hello")
来源：http://cc.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://dv.nszjky.cn

var a = 1;  let b = 2
来源：http://yr.nicolike.cn

[T18] Swift：字符串插值
来源：http://oz.jianghongdianzi.cn

"值: \(b)"
来源：http://xn.asd995.cn

[T19] Swift：可选绑定
来源：http://hu.shtwfgs.cn

if let n = opt { print(n) }
来源：http://kc.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://sb.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rw.huixiangedu.cn

[T21] Swift：遍历
来源：http://gm.szxytkj.cn

for x in a { print(x) }
来源：http://hj.wgjwhj.cn

[T22] Swift：字典
来源：http://rc.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lf.newstarts.cn

[T23] Swift：函数
来源：http://rk.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zm.bookmarksfly.cn

[T24] Swift：闭包
来源：http://tv.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://os.muxihuayi.cn

[T25] Swift：结构体
来源：http://hb.szsharing.cn

struct P { var x: Int }
来源：http://dt.haigaiapp.cn

[T26] Swift：类与重写
来源：http://hx.nicolike.cn

class A: Base { override func f() {} }
来源：http://eu.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://oz.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://qc.lnxyls.cn

[T28] Swift：枚举
来源：http://qy.9csxet.cn

enum Color { case red, green }
来源：http://vx.asd995.cn

[T29] Swift：guard 提前返回
来源：http://la.colortex.cn

guard let x = opt else { return }
来源：http://qw.jctech888.com.cn

[T30] Swift：协议
来源：http://lu.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://zd.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://lt.nicolike.cn

print("Hello")
来源：http://if.lnxyls.cn

[T32] Lua：局部变量
来源：http://ty.asd995.cn

local a = 1
来源：http://gy.nszjky.cn

[T33] Lua：表（数组）
来源：http://nf.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://so.wgjwhj.cn

[T34] Lua：遍历表
来源：http://aq.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sa.chemitech.net.cn

[T35] Lua：字典表
来源：http://ob.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://rg.jianghongdianzi.cn

[T36] Lua：函数
来源：http://en.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://pv.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://vo.bookmarksfly.cn

"a" .. "b"
来源：http://cu.hahajie.cn

[T38] Lua：条件
来源：http://ol.asd995.cn

if x > 0 then print("正") end
来源：http://oi.shxzukj.cn

[T39] Lua：模式匹配
来源：http://jy.shtwfgs.cn

string.find(s, "%d+")
来源：http://ar.yuexingan06.cn

[T40] Lua：元表
来源：http://ds.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://yw.9csxet.cn

[T41] Perl：Hello World
来源：http://jl.yuntaijiaju.cn

print "Hello\n";
来源：http://wh.szsharing.cn

[T42] Perl：变量类型
来源：http://jn.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kv.colortex.cn

[T43] Perl：字符串插值
来源：http://pu.huanxung.cn

"值: $a"
来源：http://ng.nszjky.cn

[T44] Perl：条件
来源：http://ft.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://fd.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://de.colortex.cn

for my $x (@arr) { print $x; }
来源：http://at.521024.cn

[T46] Perl：哈希操作
来源：http://qw.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yq.huanxung.cn

[T47] Perl：正则捕获
来源：http://lq.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sz.9csxet.cn

[T48] Perl：正则替换
来源：http://yn.shxzukj.cn

$s =~ s/old/new/g;
来源：http://ny.muxihuayi.cn

[T49] Perl：函数
来源：http://ms.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yr.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://be.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oa.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://ak.haigaiapp.cn

[T51] Scala：Hello World
来源：http://mt.shtwfgs.cn

println("Hello")
来源：http://am.gzmigu.cn

[T52] Scala：变量
来源：http://as.asd995.cn

val a = 1;  var b = 2
来源：http://yq.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://yl.nszjky.cn

s"值: $b"
来源：http://kj.9csxet.cn

[T54] Scala：集合映射
来源：http://sq.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://ai.asd995.cn

[T55] Scala：集合过滤
来源：http://lu.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mh.lnxyls.cn

[T56] Scala：样例类
来源：http://bi.shxzskj.cn

case class User(name: String, age: Int)
来源：http://rf.nicolike.cn

[T57] Scala：模式匹配
来源：http://nt.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ze.newstarts.cn

[T58] Scala：函数定义
来源：http://eu.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bg.bjjhwx.cn

[T59] Scala：循环
来源：http://yn.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://pr.hnjuh.cn

[T60] Scala：折叠
来源：http://qi.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tv.yuexingan06.cn

================================================================================
来源：http://wb.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xk.lnxyls.cn

================================================================================
来源：http://mo.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://db.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jr.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://xv.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ca.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://ov.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xh.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://kd.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xy.hahajie.cn

[U05] Py：列表去重且保序
来源：http://xu.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://de.nicolike.cn

[U06] Py：合并两个字典
来源：http://sg.shtwfgs.cn

{**a, **b}
来源：http://wk.lnxyls.cn

[U07] Py：反转字典键值
来源：http://gk.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://kr.hahajie.cn

[U08] Py：展平二维列表
来源：http://ty.jctech888.com.cn

[y for x in nested for y in x]
来源：http://ge.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://ls.shtwfgs.cn

max(d, key=d.get)
来源：http://vz.newstarts.cn

[U10] Py：按值排序字典
来源：http://pq.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uz.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://rj.colortex.cn

(x * 2 for x in arr)
来源：http://vf.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fw.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://yb.shxzskj.cn

[U13] Py：固定长度队列
来源：http://yh.szsharing.cn

deque(maxlen=10)
来源：http://zz.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://jv.asd995.cn

defaultdict(list)
来源：http://vl.haigaiapp.cn

[U15] Py：高精度计时
来源：http://gz.huixiangedu.cn

t = time.perf_counter()
来源：http://gn.nszjky.cn

[U16] Py：命令行参数解析
来源：http://af.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://av.nicolike.cn

[U17] Py：初始化日志
来源：http://of.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://sr.newstarts.cn

[U18] Py：预编译正则
来源：http://qo.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://cv.asd995.cn

[U19] Py：正则替换带回调
来源：http://li.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qd.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://rr.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://tq.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://vb.huixiangedu.cn

@contextlib.contextmanager
来源：http://ws.9csxet.cn

[U22] Py：矩阵转置
来源：http://yx.shxzskj.cn

list(zip(*m))
来源：http://hj.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://ni.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eu.szsharing.cn

[U24] Py：路径操作
来源：http://eh.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://et.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://fj.colortex.cn

csv.DictReader(f)
来源：http://qu.shxzskj.cn

[U26] Py：并发下载
来源：http://av.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ho.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://ww.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://ji.lnxyls.cn

[U28] Py：类型别名
来源：http://vk.nszjky.cn

UserId = int
来源：http://sk.bookmarksfly.cn

[U29] Py：属性校验
来源：http://oo.asd995.cn

@property 与 @x.setter 配合
来源：http://fy.jctech888.com.cn

[U30] Py：数据类
来源：http://bn.haigaiapp.cn

@dataclass(slots=True)
来源：http://wh.nicolike.cn

[U31] Py：单测
来源：http://iz.nicolike.cn

python -m pytest -q
来源：http://eb.shxzukj.cn

[U32] Py：代码格式化
来源：http://hw.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://wf.bjjhwx.cn

[U33] Py：打包发布
来源：http://qi.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://bq.chemitech.net.cn

[U34] Py：判断编码
来源：http://ng.9csxet.cn

chardet.detect(raw)
来源：http://vx.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://te.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yb.haigaiapp.cn

[U36] Py：定时任务
来源：http://xi.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://rw.newstarts.cn

[U37] Py：读写 Excel
来源：http://av.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ss.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://ys.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://jh.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://wf.shtwfgs.cn

sys.stdout.isatty()
来源：http://ww.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://je.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://pv.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://qa.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://il.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://sn.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aw.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://rd.panjiajie.cn

namespace App\Http;
来源：http://im.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://mt.colortex.cn

declare(strict_types=1);
来源：http://jw.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://rw.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ro.9csxet.cn

[U46] PHP：可空类型
来源：http://ag.panjiajie.cn

?string $name = null
来源：http://vc.jctech888.com.cn

[U47] PHP：联合类型
来源：http://en.hahajie.cn

int|string $id
来源：http://af.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://bv.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://et.huixiangedu.cn

[U49] PHP：只读属性
来源：http://mv.shtwfgs.cn

public readonly string $name
来源：http://ub.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://dk.newstarts.cn

public function __construct(private int $id) {}
来源：http://my.muxihuayi.cn

[U51] PHP：数组解构
来源：http://tn.hahajie.cn

[$a, $b] = $arr;
来源：http://nu.shxzskj.cn

[U52] PHP：箭头函数
来源：http://zw.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://ij.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://eo.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://yi.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://zj.yuexingan06.cn

$obj?->method()
来源：http://em.hahajie.cn


<!-- 参考信息 -->