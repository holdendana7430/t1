代发 wailian999

memset(a, 0, sizeof a);
来源：http://fv.szsharing.cn

[S27] C：定义常量
来源：http://mx.panjiajie.cn

const double PI = 3.14159;
来源：http://xx.hnjuh.cn

[S28] C：静态变量
来源：http://xn.newstarts.cn

static int counter = 0;
来源：http://sv.hahajie.cn

[S29] C：变参函数
来源：http://gl.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xy.nicolike.cn

[S30] C：头文件保护
来源：http://qt.colortex.cn

#ifndef X_H
来源：http://ws.gzmigu.cn

#define X_H
来源：http://ws.shtwfgs.cn

#endif
来源：http://hh.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://kg.newstarts.cn

#include <iostream>
来源：http://jz.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://pe.shxzskj.cn

[S32] C++：字符串
来源：http://lf.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://et.newstarts.cn

[S33] C++：vector 增删
来源：http://ob.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wm.gzmigu.cn

[S34] C++：遍历 vector
来源：http://tl.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://zt.shxzskj.cn

[S35] C++：map
来源：http://gr.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jv.nszjky.cn

[S36] C++：unordered_map
来源：http://fi.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bg.9csxet.cn

[S37] C++：set
来源：http://ql.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nr.newstarts.cn

[S38] C++：排序
来源：http://ur.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://gv.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://ed.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pl.bjjhwx.cn

[S40] C++：查找元素
来源：http://aa.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mk.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://wi.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sg.huanxung.cn

[S42] C++：继承与虚函数
来源：http://xd.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://vz.bookmarksfly.cn

[S43] C++：智能指针
来源：http://wg.521024.cn

auto p = std::make_unique<int>(5);
来源：http://lq.huanxung.cn

[S44] C++：引用传参
来源：http://fl.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://ee.gzmigu.cn

[S45] C++：lambda
来源：http://wh.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hm.lnxyls.cn

[S46] C++：函数模板
来源：http://sv.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xr.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://ua.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kg.szsharing.cn

[S48] C++：逐行读文件
来源：http://wd.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vc.hahajie.cn

while (std::getline(in, line)) { }
来源：http://gc.nszjky.cn

[S49] C++：写文件
来源：http://ze.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nf.nicolike.cn

[S50] C++：格式化数字
来源：http://jo.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dq.shxzskj.cn

[S51] C++：显式类型转换
来源：http://cm.521024.cn

static_cast<double>(a) / b
来源：http://su.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://ut.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://ed.asd995.cn

[S53] C++：移动语义
来源：http://to.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://ih.szsharing.cn

[S54] C++：异常处理
来源：http://pa.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://au.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://wb.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ph.muxihuayi.cn

[S56] C++：optional
来源：http://rf.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yv.yuexingan06.cn

[S57] C++：编译期常量
来源：http://ct.hnjuh.cn

constexpr int N = 10;
来源：http://dq.yuexingan06.cn

[S58] C++：命名空间
来源：http://rn.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://sp.huixiangedu.cn

[S59] C++：静态断言
来源：http://qb.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fo.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://xi.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ni.shxzskj.cn

================================================================================
来源：http://lv.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dl.huixiangedu.cn

================================================================================
来源：http://si.colortex.cn

[T01] Kotlin：Hello World
来源：http://dy.yuntaijiaju.cn

println("Hello")
来源：http://yq.bjjhwx.cn

[T02] Kotlin：变量
来源：http://ee.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zd.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://yi.521024.cn

"值: $b"
来源：http://sb.gzmigu.cn

[T04] Kotlin：空安全
来源：http://ik.shxzskj.cn

val n: String? = null;  n?.length
来源：http://vv.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://gu.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ze.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://fl.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ue.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://sc.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://no.huanxung.cn

[T08] Kotlin：数据类
来源：http://yn.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://vg.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://ks.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://uw.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://ad.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pk.szxytkj.cn

[T11] Kotlin：协程
来源：http://kv.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ws.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://kg.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://va.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://ko.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://sn.hahajie.cn

[T14] Kotlin：循环
来源：http://do.szxytkj.cn

for (i in 1..10) println(i)
来源：http://fg.szsharing.cn

[T15] Kotlin：接口
来源：http://vv.nszjky.cn

interface Shape { fun area(): Double }
来源：http://gw.521024.cn

[T16] Swift：Hello World
来源：http://li.shxzskj.cn

print("Hello")
来源：http://wn.colortex.cn

[T17] Swift：变量与常量
来源：http://jf.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://xq.hahajie.cn

[T18] Swift：字符串插值
来源：http://bw.szxytkj.cn

"值: \(b)"
来源：http://cb.shxzukj.cn

[T19] Swift：可选绑定
来源：http://qb.huanxung.cn

if let n = opt { print(n) }
来源：http://rl.shxzukj.cn

[T20] Swift：数组操作
来源：http://qo.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ft.haigaiapp.cn

[T21] Swift：遍历
来源：http://yz.nicolike.cn

for x in a { print(x) }
来源：http://bf.panjiajie.cn

[T22] Swift：字典
来源：http://zf.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gu.shxzukj.cn

[T23] Swift：函数
来源：http://uj.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yn.gzmigu.cn

[T24] Swift：闭包
来源：http://mn.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bg.lnxyls.cn

[T25] Swift：结构体
来源：http://vx.huanxung.cn

struct P { var x: Int }
来源：http://qt.hahajie.cn

[T26] Swift：类与重写
来源：http://ed.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://ym.9csxet.cn

[T27] Swift：错误处理
来源：http://cy.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://eo.hnjuh.cn

[T28] Swift：枚举
来源：http://cd.colortex.cn

enum Color { case red, green }
来源：http://ot.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://tr.huanxung.cn

guard let x = opt else { return }
来源：http://js.colortex.cn

[T30] Swift：协议
来源：http://go.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://zo.nszjky.cn

[T31] Lua：Hello World
来源：http://vu.haigaiapp.cn

print("Hello")
来源：http://dr.lnxyls.cn

[T32] Lua：局部变量
来源：http://st.nszjky.cn

local a = 1
来源：http://yr.521024.cn

[T33] Lua：表（数组）
来源：http://mx.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yx.panjiajie.cn

[T34] Lua：遍历表
来源：http://pm.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cj.huixiangedu.cn

[T35] Lua：字典表
来源：http://vs.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://xk.yuexingan06.cn

[T36] Lua：函数
来源：http://dz.gzmigu.cn

function add(a, b) return a + b end
来源：http://fv.hahajie.cn

[T37] Lua：字符串拼接
来源：http://ki.colortex.cn

"a" .. "b"
来源：http://fm.chemitech.net.cn

[T38] Lua：条件
来源：http://md.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://lw.hnjuh.cn

[T39] Lua：模式匹配
来源：http://kj.shxzskj.cn

string.find(s, "%d+")
来源：http://ia.jctech888.com.cn

[T40] Lua：元表
来源：http://ou.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://ol.jctech888.com.cn

[T41] Perl：Hello World
来源：http://hb.asd995.cn

print "Hello\n";
来源：http://cj.haigaiapp.cn

[T42] Perl：变量类型
来源：http://kj.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gj.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://ad.521024.cn

"值: $a"
来源：http://wq.9csxet.cn

[T44] Perl：条件
来源：http://rb.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://lf.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://oi.521024.cn

for my $x (@arr) { print $x; }
来源：http://ft.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://ta.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nl.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://fm.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rb.chemitech.net.cn

[T48] Perl：正则替换
来源：http://se.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://bz.nszjky.cn

[T49] Perl：函数
来源：http://lg.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://on.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://fo.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rp.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://nu.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://hd.shxzskj.cn

println("Hello")
来源：http://vp.colortex.cn

[T52] Scala：变量
来源：http://sq.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://zy.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://ml.panjiajie.cn

s"值: $b"
来源：http://oo.huanxung.cn

[T54] Scala：集合映射
来源：http://rw.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ud.szsharing.cn

[T55] Scala：集合过滤
来源：http://wc.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dg.yuexingan06.cn

[T56] Scala：样例类
来源：http://sd.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://oa.nicolike.cn

[T57] Scala：模式匹配
来源：http://nn.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ko.huanxung.cn

[T58] Scala：函数定义
来源：http://dx.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ta.newstarts.cn

[T59] Scala：循环
来源：http://ko.521024.cn

for (i <- 1 to 10) println(i)
来源：http://sb.newstarts.cn

[T60] Scala：折叠
来源：http://pk.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bb.lnxyls.cn

================================================================================
来源：http://wy.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bw.jctech888.com.cn

================================================================================
来源：http://aw.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://ur.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hx.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://zl.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yu.521024.cn

[U03] Py：加载 .env 配置
来源：http://zo.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tg.nszjky.cn

[U04] Py：变量调试打印
来源：http://pv.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ox.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://im.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://cp.hahajie.cn

[U06] Py：合并两个字典
来源：http://gz.szxytkj.cn

{**a, **b}
来源：http://hl.panjiajie.cn

[U07] Py：反转字典键值
来源：http://rz.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://ay.asd995.cn

[U08] Py：展平二维列表
来源：http://ji.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://pb.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://ln.lnxyls.cn

max(d, key=d.get)
来源：http://hv.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://bb.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xk.szxytkj.cn

[U11] Py：生成器表达式
来源：http://lw.muxihuayi.cn

(x * 2 for x in arr)
来源：http://bp.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xq.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://cy.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://ho.hahajie.cn

deque(maxlen=10)
来源：http://sc.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://iq.yuexingan06.cn

defaultdict(list)
来源：http://fi.wgjwhj.cn

[U15] Py：高精度计时
来源：http://xc.shtwfgs.cn

t = time.perf_counter()
来源：http://ns.nicolike.cn

[U16] Py：命令行参数解析
来源：http://bc.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tq.szsharing.cn

[U17] Py：初始化日志
来源：http://mu.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://qe.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://ic.colortex.cn

pat = re.compile(r"\d+")
来源：http://rd.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://cl.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tj.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://yg.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://ft.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://sy.asd995.cn

@contextlib.contextmanager
来源：http://dt.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://vq.shtwfgs.cn

list(zip(*m))
来源：http://xc.nszjky.cn

[U23] Py：分块读取大文件
来源：http://et.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ho.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://lf.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hg.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://ke.521024.cn

csv.DictReader(f)
来源：http://dv.shtwfgs.cn

[U26] Py：并发下载
来源：http://sg.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tt.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://gq.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://wv.huixiangedu.cn

[U28] Py：类型别名
来源：http://ng.huanxung.cn

UserId = int
来源：http://xf.asd995.cn

[U29] Py：属性校验
来源：http://cq.asd995.cn

@property 与 @x.setter 配合
来源：http://jn.asd995.cn

[U30] Py：数据类
来源：http://gi.huixiangedu.cn

@dataclass(slots=True)
来源：http://ds.huanxung.cn

[U31] Py：单测
来源：http://ip.haigaiapp.cn

python -m pytest -q
来源：http://sk.haigaiapp.cn

[U32] Py：代码格式化
来源：http://de.szsharing.cn

ruff format . && ruff check --fix .
来源：http://qo.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://ni.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://qw.panjiajie.cn

[U34] Py：判断编码
来源：http://aj.jctech888.com.cn

chardet.detect(raw)
来源：http://ip.hahajie.cn

[U35] Py：发送邮件
来源：http://cy.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ks.colortex.cn

[U36] Py：定时任务
来源：http://nn.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://gw.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://eb.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ql.521024.cn

[U38] Py：获取脚本所在目录
来源：http://ww.lnxyls.cn

Path(__file__).resolve().parent
来源：http://ov.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://iy.nszjky.cn

sys.stdout.isatty()
来源：http://ki.hahajie.cn

[U40] Py：打印到标准错误
来源：http://jr.asd995.cn

print("err", file=sys.stderr)
来源：http://do.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://dy.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mr.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://qa.bjjhwx.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sb.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://lu.hnjuh.cn

namespace App\Http;
来源：http://ha.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://km.gzmigu.cn

declare(strict_types=1);
来源：http://yz.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://kd.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hp.huixiangedu.cn

[U46] PHP：可空类型
来源：http://gf.nicolike.cn

?string $name = null
来源：http://km.lnxyls.cn

[U47] PHP：联合类型
来源：http://pp.hnjuh.cn

int|string $id
来源：http://dl.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://yk.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ub.szxytkj.cn

[U49] PHP：只读属性
来源：http://sy.shxzukj.cn

public readonly string $name
来源：http://mq.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://hi.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://ol.panjiajie.cn


<!-- 参考信息 -->