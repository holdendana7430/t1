代发 wailian999

static int counter = 0;
来源：http://ij.huanxung.cn

[S29] C：变参函数
来源：http://bd.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wj.nicolike.cn

[S30] C：头文件保护
来源：http://hx.shxzukj.cn

#ifndef X_H
来源：http://ok.szxytkj.cn

#define X_H
来源：http://oa.asd995.cn

#endif
来源：http://ec.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://jl.szxytkj.cn

#include <iostream>
来源：http://ym.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://tw.yuntaijiaju.cn

[S32] C++：字符串
来源：http://ag.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://mp.huixiangedu.cn

[S33] C++：vector 增删
来源：http://tk.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gu.szsharing.cn

[S34] C++：遍历 vector
来源：http://is.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://rl.szxytkj.cn

[S35] C++：map
来源：http://qj.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lf.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://tw.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ni.colortex.cn

[S37] C++：set
来源：http://sb.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lv.huixiangedu.cn

[S38] C++：排序
来源：http://uz.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://su.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://ja.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ss.huixiangedu.cn

[S40] C++：查找元素
来源：http://rz.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qq.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://ky.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://su.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://ef.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://nf.521024.cn

[S43] C++：智能指针
来源：http://xy.521024.cn

auto p = std::make_unique<int>(5);
来源：http://mz.szsharing.cn

[S44] C++：引用传参
来源：http://uw.colortex.cn

void inc(int &x) { ++x; }
来源：http://it.huanxung.cn

[S45] C++：lambda
来源：http://ff.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ul.gzmigu.cn

[S46] C++：函数模板
来源：http://ve.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xd.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://tg.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eg.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://hr.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://um.asd995.cn

while (std::getline(in, line)) { }
来源：http://xo.huixinmuqiang.cn

[S49] C++：写文件
来源：http://qj.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ww.colortex.cn

[S50] C++：格式化数字
来源：http://dj.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dj.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://xk.wgjwhj.cn

static_cast<double>(a) / b
来源：http://uw.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://qs.szsharing.cn

int size() const noexcept { return n_; }
来源：http://lv.asd995.cn

[S53] C++：移动语义
来源：http://yf.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://zb.colortex.cn

[S54] C++：异常处理
来源：http://tz.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tt.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://fw.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ru.chemitech.net.cn

[S56] C++：optional
来源：http://ew.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mj.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://aq.jianghongdianzi.cn

constexpr int N = 10;
来源：http://uk.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://jw.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://bh.huanxung.cn

[S59] C++：静态断言
来源：http://ac.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fx.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://pc.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aj.9csxet.cn

================================================================================
来源：http://ke.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kl.jctech888.com.cn

================================================================================
来源：http://jc.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://yk.shxzskj.cn

println("Hello")
来源：http://tw.szxytkj.cn

[T02] Kotlin：变量
来源：http://ux.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uc.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://ti.jctech888.com.cn

"值: $b"
来源：http://pg.lnxyls.cn

[T04] Kotlin：空安全
来源：http://js.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://xi.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://bn.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://in.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://mh.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sn.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://rz.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lj.521024.cn

[T08] Kotlin：数据类
来源：http://uh.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://ot.asd995.cn

[T09] Kotlin：扩展函数
来源：http://tp.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://oo.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://mz.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oz.newstarts.cn

[T11] Kotlin：协程
来源：http://mz.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.521024.cn

[T12] Kotlin：解构声明
来源：http://sb.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://ft.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://qz.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://tt.haigaiapp.cn

[T14] Kotlin：循环
来源：http://ex.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://eo.szsharing.cn

[T15] Kotlin：接口
来源：http://nd.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://io.hnjuh.cn

[T16] Swift：Hello World
来源：http://fc.hahajie.cn

print("Hello")
来源：http://ki.huanxung.cn

[T17] Swift：变量与常量
来源：http://yl.haigaiapp.cn

var a = 1;  let b = 2
来源：http://vv.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://yn.newstarts.cn

"值: \(b)"
来源：http://kb.521024.cn

[T19] Swift：可选绑定
来源：http://fb.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://js.nicolike.cn

[T20] Swift：数组操作
来源：http://gh.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://al.asd995.cn

[T21] Swift：遍历
来源：http://wr.szsharing.cn

for x in a { print(x) }
来源：http://dv.jianghongdianzi.cn

[T22] Swift：字典
来源：http://ri.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://it.chemitech.net.cn

[T23] Swift：函数
来源：http://wf.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ql.hnjuh.cn

[T24] Swift：闭包
来源：http://rp.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ll.jctech888.com.cn

[T25] Swift：结构体
来源：http://ur.colortex.cn

struct P { var x: Int }
来源：http://os.colortex.cn

[T26] Swift：类与重写
来源：http://zg.9csxet.cn

class A: Base { override func f() {} }
来源：http://gt.newstarts.cn

[T27] Swift：错误处理
来源：http://xq.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://ab.szxytkj.cn

[T28] Swift：枚举
来源：http://xf.panjiajie.cn

enum Color { case red, green }
来源：http://dz.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://bj.colortex.cn

guard let x = opt else { return }
来源：http://jl.shxzskj.cn

[T30] Swift：协议
来源：http://cj.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://bq.chemitech.net.cn

[T31] Lua：Hello World
来源：http://fw.bookmarksfly.cn

print("Hello")
来源：http://vr.shxzukj.cn

[T32] Lua：局部变量
来源：http://xy.bjjhwx.cn

local a = 1
来源：http://cz.shxzukj.cn

[T33] Lua：表（数组）
来源：http://db.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sh.bjjhwx.cn

[T34] Lua：遍历表
来源：http://cj.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kt.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://nf.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://il.shtwfgs.cn

[T36] Lua：函数
来源：http://nx.lnxyls.cn

function add(a, b) return a + b end
来源：http://ev.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://pv.nicolike.cn

"a" .. "b"
来源：http://nk.huixiangedu.cn

[T38] Lua：条件
来源：http://ca.panjiajie.cn

if x > 0 then print("正") end
来源：http://js.newstarts.cn

[T39] Lua：模式匹配
来源：http://lz.shxzukj.cn

string.find(s, "%d+")
来源：http://gk.gzmigu.cn

[T40] Lua：元表
来源：http://vh.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://he.huanxung.cn

[T41] Perl：Hello World
来源：http://kh.bookmarksfly.cn

print "Hello\n";
来源：http://el.wgjwhj.cn

[T42] Perl：变量类型
来源：http://bg.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nx.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://jw.nszjky.cn

"值: $a"
来源：http://an.shtwfgs.cn

[T44] Perl：条件
来源：http://bm.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://mx.gzmigu.cn

[T45] Perl：数组遍历
来源：http://tp.asd995.cn

for my $x (@arr) { print $x; }
来源：http://nf.nszjky.cn

[T46] Perl：哈希操作
来源：http://vy.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tb.hnjuh.cn

[T47] Perl：正则捕获
来源：http://wq.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lj.nicolike.cn

[T48] Perl：正则替换
来源：http://hb.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://cu.521024.cn

[T49] Perl：函数
来源：http://uo.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ox.szsharing.cn

[T50] Perl：逐行读文件
来源：http://jv.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jv.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://hm.bjjhwx.cn

[T51] Scala：Hello World
来源：http://uo.huixiangedu.cn

println("Hello")
来源：http://gs.nszjky.cn

[T52] Scala：变量
来源：http://zd.asd995.cn

val a = 1;  var b = 2
来源：http://ja.hnjuh.cn

[T53] Scala：字符串插值
来源：http://nf.huixiangedu.cn

s"值: $b"
来源：http://zt.chemitech.net.cn

[T54] Scala：集合映射
来源：http://gi.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://mw.9csxet.cn

[T55] Scala：集合过滤
来源：http://lj.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fu.gzmigu.cn

[T56] Scala：样例类
来源：http://vy.asd995.cn

case class User(name: String, age: Int)
来源：http://xq.szsharing.cn

[T57] Scala：模式匹配
来源：http://zb.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qc.jctech888.com.cn

[T58] Scala：函数定义
来源：http://lj.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://td.nszjky.cn

[T59] Scala：循环
来源：http://sr.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://mk.colortex.cn

[T60] Scala：折叠
来源：http://rx.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://na.yuntaijiaju.cn

================================================================================
来源：http://ft.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nj.newstarts.cn

================================================================================
来源：http://pm.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://vl.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gg.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://be.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ie.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://rx.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ha.hahajie.cn

[U04] Py：变量调试打印
来源：http://nu.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ov.hahajie.cn

[U05] Py：列表去重且保序
来源：http://hk.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://hz.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://cl.wgjwhj.cn

{**a, **b}
来源：http://ue.colortex.cn

[U07] Py：反转字典键值
来源：http://sb.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://nk.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://iw.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://sk.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://ia.newstarts.cn

max(d, key=d.get)
来源：http://qg.hahajie.cn

[U10] Py：按值排序字典
来源：http://od.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yy.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://in.9csxet.cn

(x * 2 for x in arr)
来源：http://yy.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lm.lnxyls.cn

Counter(arr).most_common(3)
来源：http://hh.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://kk.bookmarksfly.cn

deque(maxlen=10)
来源：http://hl.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://jz.jianghongdianzi.cn

defaultdict(list)
来源：http://oc.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://kj.nicolike.cn

t = time.perf_counter()
来源：http://mk.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://tr.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dc.chemitech.net.cn

[U17] Py：初始化日志
来源：http://ic.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://kk.huixiangedu.cn

[U18] Py：预编译正则
来源：http://op.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://sl.nszjky.cn

[U19] Py：正则替换带回调
来源：http://pb.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sy.newstarts.cn

[U20] Py：缓存函数结果
来源：http://oo.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://pp.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://am.huanxung.cn

@contextlib.contextmanager
来源：http://yk.asd995.cn

[U22] Py：矩阵转置
来源：http://uw.szxytkj.cn

list(zip(*m))
来源：http://fx.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://re.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://si.colortex.cn

[U24] Py：路径操作
来源：http://ul.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kx.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://vg.asd995.cn

csv.DictReader(f)
来源：http://rk.9csxet.cn

[U26] Py：并发下载
来源：http://ns.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ow.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://gy.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://do.9csxet.cn

[U28] Py：类型别名
来源：http://ux.huanxung.cn

UserId = int
来源：http://tc.hnjuh.cn

[U29] Py：属性校验
来源：http://dk.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://bu.hahajie.cn

[U30] Py：数据类
来源：http://dm.haigaiapp.cn

@dataclass(slots=True)
来源：http://ns.bjjhwx.cn

[U31] Py：单测
来源：http://sp.szxytkj.cn

python -m pytest -q
来源：http://fc.colortex.cn

[U32] Py：代码格式化
来源：http://rg.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://oj.muxihuayi.cn

[U33] Py：打包发布
来源：http://ce.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://te.szxytkj.cn

[U34] Py：判断编码
来源：http://ac.huixinmuqiang.cn

chardet.detect(raw)
来源：http://tb.gzmigu.cn

[U35] Py：发送邮件
来源：http://kj.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ti.521024.cn

[U36] Py：定时任务
来源：http://ak.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://wl.asd995.cn

[U37] Py：读写 Excel
来源：http://nh.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hz.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://ox.panjiajie.cn

Path(__file__).resolve().parent
来源：http://ht.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://bw.chemitech.net.cn

sys.stdout.isatty()
来源：http://zg.nszjky.cn

[U40] Py：打印到标准错误
来源：http://st.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://yp.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://bp.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ch.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://jy.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ru.newstarts.cn

[U43] PHP：声明命名空间
来源：http://vb.shxzukj.cn

namespace App\Http;
来源：http://gy.newstarts.cn

[U44] PHP：开启严格类型
来源：http://sm.bjjhwx.cn

declare(strict_types=1);
来源：http://wt.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://in.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cu.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://fw.nszjky.cn

?string $name = null
来源：http://xm.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://bt.shtwfgs.cn

int|string $id
来源：http://ky.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://xs.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sr.szxytkj.cn

[U49] PHP：只读属性
来源：http://xa.jctech888.com.cn

public readonly string $name
来源：http://yq.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://mm.shxzukj.cn

public function __construct(private int $id) {}
来源：http://yg.muxihuayi.cn

[U51] PHP：数组解构
来源：http://qq.nicolike.cn

[$a, $b] = $arr;
来源：http://cd.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://yk.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://ke.jianghongdianzi.cn


<!-- 参考信息 -->