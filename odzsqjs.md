代发 wailian999

memset(a, 0, sizeof a);
来源：http://cu.jianghongdianzi.cn

[S27] C：定义常量
来源：http://pu.colortex.cn

const double PI = 3.14159;
来源：http://ah.hnjuh.cn

[S28] C：静态变量
来源：http://ug.wgjwhj.cn

static int counter = 0;
来源：http://sx.jctech888.com.cn

[S29] C：变参函数
来源：http://xm.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rl.wgjwhj.cn

[S30] C：头文件保护
来源：http://vw.colortex.cn

#ifndef X_H
来源：http://qy.panjiajie.cn

#define X_H
来源：http://yu.yuexingan06.cn

#endif
来源：http://eb.shxzukj.cn

[S31] C++：Hello World
来源：http://vn.yuexingan06.cn

#include <iostream>
来源：http://xs.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://vb.szsharing.cn

[S32] C++：字符串
来源：http://dw.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://fm.szsharing.cn

[S33] C++：vector 增删
来源：http://vj.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://es.lnxyls.cn

[S34] C++：遍历 vector
来源：http://fa.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://zq.gzmigu.cn

[S35] C++：map
来源：http://aw.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xw.szsharing.cn

[S36] C++：unordered_map
来源：http://er.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vq.9csxet.cn

[S37] C++：set
来源：http://mv.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jx.huanxung.cn

[S38] C++：排序
来源：http://xs.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://uc.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://jy.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gt.jctech888.com.cn

[S40] C++：查找元素
来源：http://np.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fo.9csxet.cn

[S41] C++：类与构造函数
来源：http://ok.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aj.huanxung.cn

[S42] C++：继承与虚函数
来源：http://tl.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://ak.newstarts.cn

[S43] C++：智能指针
来源：http://uo.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://rt.hahajie.cn

[S44] C++：引用传参
来源：http://zw.9csxet.cn

void inc(int &x) { ++x; }
来源：http://ju.huixiangedu.cn

[S45] C++：lambda
来源：http://tb.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rv.muxihuayi.cn

[S46] C++：函数模板
来源：http://wg.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fq.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://zc.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vk.nicolike.cn

[S48] C++：逐行读文件
来源：http://rj.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pj.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://cb.colortex.cn

[S49] C++：写文件
来源：http://tj.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bb.nicolike.cn

[S50] C++：格式化数字
来源：http://ua.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fy.nszjky.cn

[S51] C++：显式类型转换
来源：http://sj.shxzskj.cn

static_cast<double>(a) / b
来源：http://xp.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://bp.9csxet.cn

int size() const noexcept { return n_; }
来源：http://sy.nszjky.cn

[S53] C++：移动语义
来源：http://fv.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://ic.hnjuh.cn

[S54] C++：异常处理
来源：http://an.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rc.nszjky.cn

[S55] C++：结构化绑定
来源：http://oh.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xw.9csxet.cn

[S56] C++：optional
来源：http://iu.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mz.muxihuayi.cn

[S57] C++：编译期常量
来源：http://px.bjjhwx.cn

constexpr int N = 10;
来源：http://ig.bookmarksfly.cn

[S58] C++：命名空间
来源：http://ll.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://jm.newstarts.cn

[S59] C++：静态断言
来源：http://xg.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nu.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://yj.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hp.gzmigu.cn

================================================================================
来源：http://jz.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oz.shxzskj.cn

================================================================================
来源：http://tc.9csxet.cn

[T01] Kotlin：Hello World
来源：http://sj.yuexingan06.cn

println("Hello")
来源：http://zv.muxihuayi.cn

[T02] Kotlin：变量
来源：http://go.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ok.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://fn.huixiangedu.cn

"值: $b"
来源：http://si.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://or.9csxet.cn

val n: String? = null;  n?.length
来源：http://da.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://eo.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xw.hahajie.cn

[T06] Kotlin：集合映射
来源：http://nq.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fx.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://sb.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://om.newstarts.cn

[T08] Kotlin：数据类
来源：http://nw.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://wz.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://yg.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://zs.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://ee.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ln.shxzskj.cn

[T11] Kotlin：协程
来源：http://gf.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kt.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://sz.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://qt.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://wi.nicolike.cn

val m = mapOf("a" to 1)
来源：http://mk.shxzskj.cn

[T14] Kotlin：循环
来源：http://pf.hahajie.cn

for (i in 1..10) println(i)
来源：http://ju.panjiajie.cn

[T15] Kotlin：接口
来源：http://pa.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://ny.haigaiapp.cn

[T16] Swift：Hello World
来源：http://wz.gzmigu.cn

print("Hello")
来源：http://sp.lnxyls.cn

[T17] Swift：变量与常量
来源：http://dw.nicolike.cn

var a = 1;  let b = 2
来源：http://ah.nicolike.cn

[T18] Swift：字符串插值
来源：http://ew.muxihuayi.cn

"值: \(b)"
来源：http://hl.hnjuh.cn

[T19] Swift：可选绑定
来源：http://lo.shxzukj.cn

if let n = opt { print(n) }
来源：http://tk.9csxet.cn

[T20] Swift：数组操作
来源：http://tm.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ux.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://gw.shtwfgs.cn

for x in a { print(x) }
来源：http://nm.huixiangedu.cn

[T22] Swift：字典
来源：http://ev.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vv.newstarts.cn

[T23] Swift：函数
来源：http://ri.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lj.yuexingan06.cn

[T24] Swift：闭包
来源：http://mh.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cb.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://ma.shxzskj.cn

struct P { var x: Int }
来源：http://mw.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://yq.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://ii.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://fi.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://nv.huixiangedu.cn

[T28] Swift：枚举
来源：http://db.shxzukj.cn

enum Color { case red, green }
来源：http://gr.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://pg.hnjuh.cn

guard let x = opt else { return }
来源：http://dr.521024.cn

[T30] Swift：协议
来源：http://se.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://nv.asd995.cn

[T31] Lua：Hello World
来源：http://je.bookmarksfly.cn

print("Hello")
来源：http://ad.shxzskj.cn

[T32] Lua：局部变量
来源：http://rt.nszjky.cn

local a = 1
来源：http://qn.gzmigu.cn

[T33] Lua：表（数组）
来源：http://zo.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lv.chemitech.net.cn

[T34] Lua：遍历表
来源：http://vo.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://go.hahajie.cn

[T35] Lua：字典表
来源：http://we.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://ed.muxihuayi.cn

[T36] Lua：函数
来源：http://fe.huanxung.cn

function add(a, b) return a + b end
来源：http://sm.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://wl.huixiangedu.cn

"a" .. "b"
来源：http://su.wgjwhj.cn

[T38] Lua：条件
来源：http://ox.haigaiapp.cn

if x > 0 then print("正") end
来源：http://hl.521024.cn

[T39] Lua：模式匹配
来源：http://nr.hahajie.cn

string.find(s, "%d+")
来源：http://ls.newstarts.cn

[T40] Lua：元表
来源：http://jq.szsharing.cn

setmetatable({}, { __index = base })
来源：http://ti.newstarts.cn

[T41] Perl：Hello World
来源：http://is.bookmarksfly.cn

print "Hello\n";
来源：http://nt.hnjuh.cn

[T42] Perl：变量类型
来源：http://hm.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rj.asd995.cn

[T43] Perl：字符串插值
来源：http://ii.huixiangedu.cn

"值: $a"
来源：http://pu.shxzskj.cn

[T44] Perl：条件
来源：http://jr.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://nb.hnjuh.cn

[T45] Perl：数组遍历
来源：http://cw.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://vb.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://bg.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pn.521024.cn

[T47] Perl：正则捕获
来源：http://tc.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lb.wgjwhj.cn

[T48] Perl：正则替换
来源：http://mp.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://ma.yuexingan06.cn

[T49] Perl：函数
来源：http://vu.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ox.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://nu.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ko.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://ni.shtwfgs.cn

[T51] Scala：Hello World
来源：http://wb.jianghongdianzi.cn

println("Hello")
来源：http://sf.huanxung.cn

[T52] Scala：变量
来源：http://vw.huanxung.cn

val a = 1;  var b = 2
来源：http://mk.huanxung.cn

[T53] Scala：字符串插值
来源：http://ju.jianghongdianzi.cn

s"值: $b"
来源：http://dz.jctech888.com.cn

[T54] Scala：集合映射
来源：http://hh.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://ag.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://xy.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ju.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://tf.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://gh.gzmigu.cn

[T57] Scala：模式匹配
来源：http://ez.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://et.szxytkj.cn

[T58] Scala：函数定义
来源：http://tn.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fq.jctech888.com.cn

[T59] Scala：循环
来源：http://ew.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://db.szsharing.cn

[T60] Scala：折叠
来源：http://vi.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ps.muxihuayi.cn

================================================================================
来源：http://yx.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pj.hahajie.cn

================================================================================
来源：http://gi.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://wi.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wc.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://yd.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zo.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://ib.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kw.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://vd.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ps.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://bz.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://vn.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://xy.lnxyls.cn

{**a, **b}
来源：http://yd.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://pr.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://mt.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://dg.hnjuh.cn

[y for x in nested for y in x]
来源：http://th.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://we.bookmarksfly.cn

max(d, key=d.get)
来源：http://mw.panjiajie.cn

[U10] Py：按值排序字典
来源：http://ug.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tl.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://af.bjjhwx.cn

(x * 2 for x in arr)
来源：http://zv.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zm.hnjuh.cn

Counter(arr).most_common(3)
来源：http://cy.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://hv.yuntaijiaju.cn

deque(maxlen=10)
来源：http://yx.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://ju.9csxet.cn

defaultdict(list)
来源：http://hk.nszjky.cn

[U15] Py：高精度计时
来源：http://gp.9csxet.cn

t = time.perf_counter()
来源：http://kh.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://pb.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oz.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://jh.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://jb.shtwfgs.cn

[U18] Py：预编译正则
来源：http://xk.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://js.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://oe.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iw.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://mj.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://fk.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://it.colortex.cn

@contextlib.contextmanager
来源：http://po.panjiajie.cn

[U22] Py：矩阵转置
来源：http://rn.newstarts.cn

list(zip(*m))
来源：http://xw.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://gs.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ld.gzmigu.cn

[U24] Py：路径操作
来源：http://er.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cu.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://at.newstarts.cn

csv.DictReader(f)
来源：http://bm.colortex.cn

[U26] Py：并发下载
来源：http://ot.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fx.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://cx.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://eg.huanxung.cn

[U28] Py：类型别名
来源：http://ld.yuntaijiaju.cn

UserId = int
来源：http://ik.hnjuh.cn

[U29] Py：属性校验
来源：http://ev.colortex.cn

@property 与 @x.setter 配合
来源：http://wd.chemitech.net.cn

[U30] Py：数据类
来源：http://ae.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://xv.asd995.cn

[U31] Py：单测
来源：http://yd.shxzskj.cn

python -m pytest -q
来源：http://dp.huanxung.cn

[U32] Py：代码格式化
来源：http://om.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://xb.jctech888.com.cn

[U33] Py：打包发布
来源：http://hb.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://gq.9csxet.cn

[U34] Py：判断编码
来源：http://oi.panjiajie.cn

chardet.detect(raw)
来源：http://ar.haigaiapp.cn

[U35] Py：发送邮件
来源：http://ak.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sl.shtwfgs.cn

[U36] Py：定时任务
来源：http://me.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://bv.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://af.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ox.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://mp.asd995.cn

Path(__file__).resolve().parent
来源：http://bg.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://kr.nicolike.cn

sys.stdout.isatty()
来源：http://fe.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://ck.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://mq.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://gn.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pb.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://ti.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ee.newstarts.cn

[U43] PHP：声明命名空间
来源：http://uk.wgjwhj.cn

namespace App\Http;
来源：http://yr.colortex.cn

[U44] PHP：开启严格类型
来源：http://ie.colortex.cn

declare(strict_types=1);
来源：http://hs.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://ie.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zv.szxytkj.cn

[U46] PHP：可空类型
来源：http://qg.gzmigu.cn

?string $name = null
来源：http://ky.wgjwhj.cn

[U47] PHP：联合类型
来源：http://sa.9csxet.cn

int|string $id
来源：http://th.szsharing.cn

[U48] PHP：纯枚举
来源：http://pj.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mg.shxzukj.cn

[U49] PHP：只读属性
来源：http://hp.shxzskj.cn

public readonly string $name
来源：http://hh.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://kz.nszjky.cn

public function __construct(private int $id) {}
来源：http://ba.asd995.cn


<!-- 参考信息 -->