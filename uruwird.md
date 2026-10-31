代发 wailian999

static int counter = 0;
来源：http://yu.chemitech.net.cn

[S29] C：变参函数
来源：http://hn.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gm.huixiangedu.cn

[S30] C：头文件保护
来源：http://du.huanxung.cn

#ifndef X_H
来源：http://jw.9csxet.cn

#define X_H
来源：http://gy.muxihuayi.cn

#endif
来源：http://et.asd995.cn

[S31] C++：Hello World
来源：http://gd.muxihuayi.cn

#include <iostream>
来源：http://tg.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://yd.huanxung.cn

[S32] C++：字符串
来源：http://uy.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://yc.wgjwhj.cn

[S33] C++：vector 增删
来源：http://pz.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cx.nicolike.cn

[S34] C++：遍历 vector
来源：http://bq.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://yl.muxihuayi.cn

[S35] C++：map
来源：http://rs.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oy.wgjwhj.cn

[S36] C++：unordered_map
来源：http://xq.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dr.bjjhwx.cn

[S37] C++：set
来源：http://ta.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wh.9csxet.cn

[S38] C++：排序
来源：http://av.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://fx.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://ac.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://li.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://mh.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gp.hnjuh.cn

[S41] C++：类与构造函数
来源：http://xi.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gd.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://eo.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://pr.gzmigu.cn

[S43] C++：智能指针
来源：http://jl.521024.cn

auto p = std::make_unique<int>(5);
来源：http://tj.jctech888.com.cn

[S44] C++：引用传参
来源：http://rj.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://fe.haigaiapp.cn

[S45] C++：lambda
来源：http://ai.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iy.colortex.cn

[S46] C++：函数模板
来源：http://ad.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kp.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://ry.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ix.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://se.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ek.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://mz.jianghongdianzi.cn

[S49] C++：写文件
来源：http://nf.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rh.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://yk.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rj.gzmigu.cn

[S51] C++：显式类型转换
来源：http://lh.haigaiapp.cn

static_cast<double>(a) / b
来源：http://od.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://xy.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://mr.shxzukj.cn

[S53] C++：移动语义
来源：http://us.asd995.cn

std::vector<int> w = std::move(v);
来源：http://hq.szsharing.cn

[S54] C++：异常处理
来源：http://lv.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gs.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://op.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://no.huixinmuqiang.cn

[S56] C++：optional
来源：http://st.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yy.gzmigu.cn

[S57] C++：编译期常量
来源：http://gw.haigaiapp.cn

constexpr int N = 10;
来源：http://lv.szxytkj.cn

[S58] C++：命名空间
来源：http://vo.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://mw.asd995.cn

[S59] C++：静态断言
来源：http://wg.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jm.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://qt.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rl.chemitech.net.cn

================================================================================
来源：http://mq.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kh.huixiangedu.cn

================================================================================
来源：http://gj.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://cq.newstarts.cn

println("Hello")
来源：http://tk.nszjky.cn

[T02] Kotlin：变量
来源：http://op.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ky.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://kc.haigaiapp.cn

"值: $b"
来源：http://dv.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://oz.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://hn.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://dq.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://io.hahajie.cn

[T06] Kotlin：集合映射
来源：http://za.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yz.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://lm.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mw.9csxet.cn

[T08] Kotlin：数据类
来源：http://jc.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://ub.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://ct.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://mc.colortex.cn

[T10] Kotlin：默认参数
来源：http://fe.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vh.bjjhwx.cn

[T11] Kotlin：协程
来源：http://yk.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rf.huanxung.cn

[T12] Kotlin：解构声明
来源：http://mx.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://nc.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://wt.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://gc.colortex.cn

[T14] Kotlin：循环
来源：http://pn.huanxung.cn

for (i in 1..10) println(i)
来源：http://kz.hahajie.cn

[T15] Kotlin：接口
来源：http://bc.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://zh.jctech888.com.cn

[T16] Swift：Hello World
来源：http://os.yuexingan06.cn

print("Hello")
来源：http://mp.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://an.shxzukj.cn

var a = 1;  let b = 2
来源：http://jl.panjiajie.cn

[T18] Swift：字符串插值
来源：http://xe.huixiangedu.cn

"值: \(b)"
来源：http://lu.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://go.shxzskj.cn

if let n = opt { print(n) }
来源：http://aw.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://jj.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ha.muxihuayi.cn

[T21] Swift：遍历
来源：http://zq.newstarts.cn

for x in a { print(x) }
来源：http://ie.szsharing.cn

[T22] Swift：字典
来源：http://un.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ae.nszjky.cn

[T23] Swift：函数
来源：http://gj.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cl.hnjuh.cn

[T24] Swift：闭包
来源：http://il.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ea.hahajie.cn

[T25] Swift：结构体
来源：http://bc.nicolike.cn

struct P { var x: Int }
来源：http://dw.shxzskj.cn

[T26] Swift：类与重写
来源：http://ht.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://yp.chemitech.net.cn

[T27] Swift：错误处理
来源：http://wr.9csxet.cn

do { try f() } catch { print(error) }
来源：http://zy.jctech888.com.cn

[T28] Swift：枚举
来源：http://xz.szsharing.cn

enum Color { case red, green }
来源：http://jm.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://em.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://cb.huixinmuqiang.cn

[T30] Swift：协议
来源：http://ak.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://yr.nicolike.cn

[T31] Lua：Hello World
来源：http://ns.yuexingan06.cn

print("Hello")
来源：http://lj.wgjwhj.cn

[T32] Lua：局部变量
来源：http://cx.huixiangedu.cn

local a = 1
来源：http://gn.lnxyls.cn

[T33] Lua：表（数组）
来源：http://tc.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lr.hahajie.cn

[T34] Lua：遍历表
来源：http://pz.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ri.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://td.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://lv.muxihuayi.cn

[T36] Lua：函数
来源：http://vw.gzmigu.cn

function add(a, b) return a + b end
来源：http://sk.nszjky.cn

[T37] Lua：字符串拼接
来源：http://un.shxzskj.cn

"a" .. "b"
来源：http://jq.newstarts.cn

[T38] Lua：条件
来源：http://ou.nszjky.cn

if x > 0 then print("正") end
来源：http://xc.szxytkj.cn

[T39] Lua：模式匹配
来源：http://ae.bookmarksfly.cn

string.find(s, "%d+")
来源：http://bl.bookmarksfly.cn

[T40] Lua：元表
来源：http://sv.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://qw.yuexingan06.cn

[T41] Perl：Hello World
来源：http://rv.gzmigu.cn

print "Hello\n";
来源：http://ko.asd995.cn

[T42] Perl：变量类型
来源：http://to.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ow.newstarts.cn

[T43] Perl：字符串插值
来源：http://jv.hnjuh.cn

"值: $a"
来源：http://gk.nszjky.cn

[T44] Perl：条件
来源：http://wa.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://jv.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://ic.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://yq.szxytkj.cn

[T46] Perl：哈希操作
来源：http://ea.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kv.hahajie.cn

[T47] Perl：正则捕获
来源：http://rv.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kj.nszjky.cn

[T48] Perl：正则替换
来源：http://ll.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://og.lnxyls.cn

[T49] Perl：函数
来源：http://gf.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wl.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://wf.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jw.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ad.colortex.cn

[T51] Scala：Hello World
来源：http://ze.yuntaijiaju.cn

println("Hello")
来源：http://oj.shxzskj.cn

[T52] Scala：变量
来源：http://dg.huixiangedu.cn

val a = 1;  var b = 2
来源：http://pz.hahajie.cn

[T53] Scala：字符串插值
来源：http://vy.nszjky.cn

s"值: $b"
来源：http://zr.bjjhwx.cn

[T54] Scala：集合映射
来源：http://il.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://nh.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://ae.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://me.haigaiapp.cn

[T56] Scala：样例类
来源：http://np.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://qp.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://ld.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lw.chemitech.net.cn

[T58] Scala：函数定义
来源：http://kb.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bv.szsharing.cn

[T59] Scala：循环
来源：http://cu.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://ul.bookmarksfly.cn

[T60] Scala：折叠
来源：http://mf.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ig.nicolike.cn

================================================================================
来源：http://xh.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://td.yuntaijiaju.cn

================================================================================
来源：http://it.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://gj.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://og.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://bp.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://np.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://sf.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://am.9csxet.cn

[U04] Py：变量调试打印
来源：http://xu.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zx.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://um.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://qu.newstarts.cn

[U06] Py：合并两个字典
来源：http://rd.521024.cn

{**a, **b}
来源：http://bq.gzmigu.cn

[U07] Py：反转字典键值
来源：http://ud.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://ub.szsharing.cn

[U08] Py：展平二维列表
来源：http://qn.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://pb.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://ir.nicolike.cn

max(d, key=d.get)
来源：http://wp.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://dt.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xu.9csxet.cn

[U11] Py：生成器表达式
来源：http://ob.bjjhwx.cn

(x * 2 for x in arr)
来源：http://ur.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jc.szsharing.cn

Counter(arr).most_common(3)
来源：http://ro.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://mw.hnjuh.cn

deque(maxlen=10)
来源：http://xx.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://fh.hahajie.cn

defaultdict(list)
来源：http://ee.yuexingan06.cn

[U15] Py：高精度计时
来源：http://pc.szsharing.cn

t = time.perf_counter()
来源：http://nk.nszjky.cn

[U16] Py：命令行参数解析
来源：http://ew.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tt.haigaiapp.cn

[U17] Py：初始化日志
来源：http://in.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://gz.muxihuayi.cn

[U18] Py：预编译正则
来源：http://lj.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://ap.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://hs.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gu.colortex.cn

[U20] Py：缓存函数结果
来源：http://fw.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://ru.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://zo.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://vv.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://gv.521024.cn

list(zip(*m))
来源：http://eu.9csxet.cn

[U23] Py：分块读取大文件
来源：http://oy.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nt.huanxung.cn

[U24] Py：路径操作
来源：http://ry.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gc.521024.cn

[U25] Py：CSV 按字典读
来源：http://xw.huixiangedu.cn

csv.DictReader(f)
来源：http://om.bjjhwx.cn

[U26] Py：并发下载
来源：http://rk.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qx.huanxung.cn

[U27] Py：异步 HTTP
来源：http://vx.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://af.chemitech.net.cn

[U28] Py：类型别名
来源：http://zl.nszjky.cn

UserId = int
来源：http://ak.nicolike.cn

[U29] Py：属性校验
来源：http://mo.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://pa.nszjky.cn

[U30] Py：数据类
来源：http://qo.bookmarksfly.cn

@dataclass(slots=True)
来源：http://vg.newstarts.cn

[U31] Py：单测
来源：http://gp.huanxung.cn

python -m pytest -q
来源：http://rk.muxihuayi.cn

[U32] Py：代码格式化
来源：http://wi.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://fg.szxytkj.cn

[U33] Py：打包发布
来源：http://cg.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://jt.muxihuayi.cn

[U34] Py：判断编码
来源：http://gf.jianghongdianzi.cn

chardet.detect(raw)
来源：http://df.hahajie.cn

[U35] Py：发送邮件
来源：http://vl.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qe.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://fe.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://kl.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://ub.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vt.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://ty.nszjky.cn

Path(__file__).resolve().parent
来源：http://ff.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://oz.bookmarksfly.cn

sys.stdout.isatty()
来源：http://ue.newstarts.cn

[U40] Py：打印到标准错误
来源：http://pf.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://mc.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://nd.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cx.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://zz.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yd.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://ml.shtwfgs.cn

namespace App\Http;
来源：http://dt.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://pj.szxytkj.cn

declare(strict_types=1);
来源：http://yi.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://sm.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tk.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://qh.shtwfgs.cn

?string $name = null
来源：http://dq.yuexingan06.cn

[U47] PHP：联合类型
来源：http://oa.huanxung.cn

int|string $id
来源：http://fb.nszjky.cn

[U48] PHP：纯枚举
来源：http://xk.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gv.shxzukj.cn

[U49] PHP：只读属性
来源：http://tm.newstarts.cn

public readonly string $name
来源：http://ca.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://ze.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://sm.szxytkj.cn

[U51] PHP：数组解构
来源：http://st.521024.cn

[$a, $b] = $arr;
来源：http://mv.lnxyls.cn

[U52] PHP：箭头函数
来源：http://ci.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://pi.asd995.cn


<!-- 参考信息 -->