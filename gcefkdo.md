代发 wailian999

memset(a, 0, sizeof a);
来源：http://ws.lnxyls.cn

[S27] C：定义常量
来源：http://xi.szsharing.cn

const double PI = 3.14159;
来源：http://ek.huanxung.cn

[S28] C：静态变量
来源：http://vs.szsharing.cn

static int counter = 0;
来源：http://eu.jianghongdianzi.cn

[S29] C：变参函数
来源：http://gt.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mj.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://zy.muxihuayi.cn

#ifndef X_H
来源：http://ur.521024.cn

#define X_H
来源：http://se.hnjuh.cn

#endif
来源：http://th.bjjhwx.cn

[S31] C++：Hello World
来源：http://je.wgjwhj.cn

#include <iostream>
来源：http://bu.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://sy.nszjky.cn

[S32] C++：字符串
来源：http://kz.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://wy.nicolike.cn

[S33] C++：vector 增删
来源：http://cr.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jx.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://og.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://kg.hnjuh.cn

[S35] C++：map
来源：http://hs.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xv.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://ts.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sr.colortex.cn

[S37] C++：set
来源：http://ob.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ib.newstarts.cn

[S38] C++：排序
来源：http://hm.asd995.cn

std::sort(v.begin(), v.end());
来源：http://bd.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://qe.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ki.nszjky.cn

[S40] C++：查找元素
来源：http://bp.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xr.colortex.cn

[S41] C++：类与构造函数
来源：http://ns.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vw.colortex.cn

[S42] C++：继承与虚函数
来源：http://hz.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://wc.huixiangedu.cn

[S43] C++：智能指针
来源：http://qn.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://in.muxihuayi.cn

[S44] C++：引用传参
来源：http://vv.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://xh.gzmigu.cn

[S45] C++：lambda
来源：http://oo.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lw.colortex.cn

[S46] C++：函数模板
来源：http://yr.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wl.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://dv.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jx.szxytkj.cn

[S48] C++：逐行读文件
来源：http://re.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ps.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://zc.521024.cn

[S49] C++：写文件
来源：http://zs.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ae.huanxung.cn

[S50] C++：格式化数字
来源：http://zo.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iz.gzmigu.cn

[S51] C++：显式类型转换
来源：http://sj.asd995.cn

static_cast<double>(a) / b
来源：http://bo.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://yc.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://my.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://kh.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://ax.muxihuayi.cn

[S54] C++：异常处理
来源：http://si.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fe.shxzskj.cn

[S55] C++：结构化绑定
来源：http://di.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://no.huixiangedu.cn

[S56] C++：optional
来源：http://ne.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kh.yuexingan06.cn

[S57] C++：编译期常量
来源：http://wr.newstarts.cn

constexpr int N = 10;
来源：http://lu.muxihuayi.cn

[S58] C++：命名空间
来源：http://ps.521024.cn

namespace ns { int f() { return 1; } }
来源：http://ug.shxzukj.cn

[S59] C++：静态断言
来源：http://cp.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lh.colortex.cn

[S60] C++：遍历并删除元素
来源：http://tg.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jn.yuntaijiaju.cn

================================================================================
来源：http://rm.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yj.yuntaijiaju.cn

================================================================================
来源：http://yk.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://cw.bjjhwx.cn

println("Hello")
来源：http://bf.521024.cn

[T02] Kotlin：变量
来源：http://fe.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ct.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://mm.nszjky.cn

"值: $b"
来源：http://zs.szsharing.cn

[T04] Kotlin：空安全
来源：http://ih.lnxyls.cn

val n: String? = null;  n?.length
来源：http://wh.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://im.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pm.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://kv.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ch.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://jo.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fq.shxzukj.cn

[T08] Kotlin：数据类
来源：http://bk.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://bw.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://lv.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://ua.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://nw.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uf.chemitech.net.cn

[T11] Kotlin：协程
来源：http://qs.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sa.hahajie.cn

[T12] Kotlin：解构声明
来源：http://nx.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://lb.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://ia.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://cz.hnjuh.cn

[T14] Kotlin：循环
来源：http://fa.szxytkj.cn

for (i in 1..10) println(i)
来源：http://hr.wgjwhj.cn

[T15] Kotlin：接口
来源：http://fz.521024.cn

interface Shape { fun area(): Double }
来源：http://py.jctech888.com.cn

[T16] Swift：Hello World
来源：http://eg.hahajie.cn

print("Hello")
来源：http://ni.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://ck.colortex.cn

var a = 1;  let b = 2
来源：http://mj.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://qg.jctech888.com.cn

"值: \(b)"
来源：http://ro.newstarts.cn

[T19] Swift：可选绑定
来源：http://gt.hahajie.cn

if let n = opt { print(n) }
来源：http://fj.colortex.cn

[T20] Swift：数组操作
来源：http://ka.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vn.shxzukj.cn

[T21] Swift：遍历
来源：http://vf.hahajie.cn

for x in a { print(x) }
来源：http://cg.muxihuayi.cn

[T22] Swift：字典
来源：http://fi.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xt.shxzskj.cn

[T23] Swift：函数
来源：http://of.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://em.chemitech.net.cn

[T24] Swift：闭包
来源：http://sj.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://te.nszjky.cn

[T25] Swift：结构体
来源：http://ov.colortex.cn

struct P { var x: Int }
来源：http://yb.521024.cn

[T26] Swift：类与重写
来源：http://wp.nicolike.cn

class A: Base { override func f() {} }
来源：http://vk.nszjky.cn

[T27] Swift：错误处理
来源：http://rj.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://iq.jctech888.com.cn

[T28] Swift：枚举
来源：http://tc.9csxet.cn

enum Color { case red, green }
来源：http://dl.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://jd.panjiajie.cn

guard let x = opt else { return }
来源：http://uw.huixinmuqiang.cn

[T30] Swift：协议
来源：http://ms.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://gs.shxzukj.cn

[T31] Lua：Hello World
来源：http://pi.gzmigu.cn

print("Hello")
来源：http://vz.shtwfgs.cn

[T32] Lua：局部变量
来源：http://zp.newstarts.cn

local a = 1
来源：http://nv.hahajie.cn

[T33] Lua：表（数组）
来源：http://lj.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://on.shxzskj.cn

[T34] Lua：遍历表
来源：http://aq.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://st.panjiajie.cn

[T35] Lua：字典表
来源：http://ux.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://ga.haigaiapp.cn

[T36] Lua：函数
来源：http://qy.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://rk.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://ds.bjjhwx.cn

"a" .. "b"
来源：http://gg.haigaiapp.cn

[T38] Lua：条件
来源：http://ai.hahajie.cn

if x > 0 then print("正") end
来源：http://yx.hnjuh.cn

[T39] Lua：模式匹配
来源：http://ll.panjiajie.cn

string.find(s, "%d+")
来源：http://eu.wgjwhj.cn

[T40] Lua：元表
来源：http://ki.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://zk.gzmigu.cn

[T41] Perl：Hello World
来源：http://iv.shxzskj.cn

print "Hello\n";
来源：http://cf.chemitech.net.cn

[T42] Perl：变量类型
来源：http://dp.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pa.hnjuh.cn

[T43] Perl：字符串插值
来源：http://pv.yuexingan06.cn

"值: $a"
来源：http://tq.lnxyls.cn

[T44] Perl：条件
来源：http://ma.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://tv.hnjuh.cn

[T45] Perl：数组遍历
来源：http://hh.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://hr.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://rs.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xt.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://qy.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lj.hnjuh.cn

[T48] Perl：正则替换
来源：http://iv.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://ko.hnjuh.cn

[T49] Perl：函数
来源：http://se.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mf.hahajie.cn

[T50] Perl：逐行读文件
来源：http://dc.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ne.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://fc.muxihuayi.cn

[T51] Scala：Hello World
来源：http://rh.wgjwhj.cn

println("Hello")
来源：http://qw.colortex.cn

[T52] Scala：变量
来源：http://wj.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://hs.gzmigu.cn

[T53] Scala：字符串插值
来源：http://pc.yuntaijiaju.cn

s"值: $b"
来源：http://oc.colortex.cn

[T54] Scala：集合映射
来源：http://bj.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://sg.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://mc.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gi.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://jp.szxytkj.cn

case class User(name: String, age: Int)
来源：http://mc.panjiajie.cn

[T57] Scala：模式匹配
来源：http://cf.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sl.nicolike.cn

[T58] Scala：函数定义
来源：http://pe.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zs.bookmarksfly.cn

[T59] Scala：循环
来源：http://rd.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://bt.hnjuh.cn

[T60] Scala：折叠
来源：http://yd.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yt.jianghongdianzi.cn

================================================================================
来源：http://vz.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xx.jctech888.com.cn

================================================================================
来源：http://vn.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://qg.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lk.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://yl.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wr.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://jg.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qw.nicolike.cn

[U04] Py：变量调试打印
来源：http://ni.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oq.hahajie.cn

[U05] Py：列表去重且保序
来源：http://rx.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://ub.panjiajie.cn

[U06] Py：合并两个字典
来源：http://kg.asd995.cn

{**a, **b}
来源：http://at.shxzskj.cn

[U07] Py：反转字典键值
来源：http://cb.szsharing.cn

{v: k for k, v in d.items()}
来源：http://mv.asd995.cn

[U08] Py：展平二维列表
来源：http://io.colortex.cn

[y for x in nested for y in x]
来源：http://nn.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://lw.shxzskj.cn

max(d, key=d.get)
来源：http://jo.lnxyls.cn

[U10] Py：按值排序字典
来源：http://us.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mq.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://ej.nicolike.cn

(x * 2 for x in arr)
来源：http://ue.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jr.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://vo.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://as.haigaiapp.cn

deque(maxlen=10)
来源：http://tz.521024.cn

[U14] Py：分组收集到列表
来源：http://xr.nicolike.cn

defaultdict(list)
来源：http://xi.gzmigu.cn

[U15] Py：高精度计时
来源：http://ox.colortex.cn

t = time.perf_counter()
来源：http://ln.huanxung.cn

[U16] Py：命令行参数解析
来源：http://vw.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sr.huanxung.cn

[U17] Py：初始化日志
来源：http://ex.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://rn.panjiajie.cn

[U18] Py：预编译正则
来源：http://yb.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://lc.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://ub.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xy.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://mc.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://jh.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://zc.colortex.cn

@contextlib.contextmanager
来源：http://mu.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://qx.hahajie.cn

list(zip(*m))
来源：http://jk.nicolike.cn

[U23] Py：分块读取大文件
来源：http://pa.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aq.newstarts.cn

[U24] Py：路径操作
来源：http://aw.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yv.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://tl.shtwfgs.cn

csv.DictReader(f)
来源：http://nz.huanxung.cn

[U26] Py：并发下载
来源：http://sq.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vs.asd995.cn

[U27] Py：异步 HTTP
来源：http://jg.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://vf.hahajie.cn

[U28] Py：类型别名
来源：http://pu.shxzukj.cn

UserId = int
来源：http://lq.shxzukj.cn

[U29] Py：属性校验
来源：http://va.nszjky.cn

@property 与 @x.setter 配合
来源：http://wc.huixiangedu.cn

[U30] Py：数据类
来源：http://in.nicolike.cn

@dataclass(slots=True)
来源：http://fj.huixinmuqiang.cn

[U31] Py：单测
来源：http://wo.lnxyls.cn

python -m pytest -q
来源：http://lo.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://jt.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://tf.panjiajie.cn

[U33] Py：打包发布
来源：http://nr.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://db.colortex.cn

[U34] Py：判断编码
来源：http://uv.shxzukj.cn

chardet.detect(raw)
来源：http://as.shtwfgs.cn

[U35] Py：发送邮件
来源：http://qc.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tf.gzmigu.cn

[U36] Py：定时任务
来源：http://ob.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://bv.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://zh.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wt.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://bt.colortex.cn

Path(__file__).resolve().parent
来源：http://bm.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://lx.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://xv.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://nl.szsharing.cn

print("err", file=sys.stderr)
来源：http://ld.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://on.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sl.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://os.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ab.asd995.cn

[U43] PHP：声明命名空间
来源：http://zn.newstarts.cn

namespace App\Http;
来源：http://df.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://nn.gzmigu.cn

declare(strict_types=1);
来源：http://hx.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://tg.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rk.nicolike.cn

[U46] PHP：可空类型
来源：http://uh.yuntaijiaju.cn

?string $name = null
来源：http://wv.gzmigu.cn

[U47] PHP：联合类型
来源：http://xr.bookmarksfly.cn

int|string $id
来源：http://qx.huanxung.cn

[U48] PHP：纯枚举
来源：http://io.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zt.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://ls.panjiajie.cn

public readonly string $name
来源：http://cc.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://cy.colortex.cn

public function __construct(private int $id) {}
来源：http://ga.chemitech.net.cn


<!-- 参考信息 -->