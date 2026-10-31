代发 wailian999

memset(a, 0, sizeof a);
来源：http://pi.hnjuh.cn

[S27] C：定义常量
来源：http://aa.hahajie.cn

const double PI = 3.14159;
来源：http://wd.newstarts.cn

[S28] C：静态变量
来源：http://rn.szsharing.cn

static int counter = 0;
来源：http://oj.szxytkj.cn

[S29] C：变参函数
来源：http://ha.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xb.jctech888.com.cn

[S30] C：头文件保护
来源：http://nr.shtwfgs.cn

#ifndef X_H
来源：http://hp.nszjky.cn

#define X_H
来源：http://qz.shxzskj.cn

#endif
来源：http://bw.yuexingan06.cn

[S31] C++：Hello World
来源：http://ph.lnxyls.cn

#include <iostream>
来源：http://ub.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://hd.yuntaijiaju.cn

[S32] C++：字符串
来源：http://pd.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://af.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://ye.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rj.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://zr.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://fe.lnxyls.cn

[S35] C++：map
来源：http://yu.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yl.muxihuayi.cn

[S36] C++：unordered_map
来源：http://za.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vo.bjjhwx.cn

[S37] C++：set
来源：http://hr.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cc.huanxung.cn

[S38] C++：排序
来源：http://yx.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://ds.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://ln.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lk.huixiangedu.cn

[S40] C++：查找元素
来源：http://gj.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fa.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://bf.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zo.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://lt.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://zy.asd995.cn

[S43] C++：智能指针
来源：http://br.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://aq.shxzskj.cn

[S44] C++：引用传参
来源：http://it.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://zt.asd995.cn

[S45] C++：lambda
来源：http://bc.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kq.shxzukj.cn

[S46] C++：函数模板
来源：http://nf.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gd.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://vz.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jk.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://ku.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zd.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://ik.colortex.cn

[S49] C++：写文件
来源：http://sb.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pu.shtwfgs.cn

[S50] C++：格式化数字
来源：http://uv.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pd.hahajie.cn

[S51] C++：显式类型转换
来源：http://ul.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://ne.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://ho.nicolike.cn

int size() const noexcept { return n_; }
来源：http://tz.haigaiapp.cn

[S53] C++：移动语义
来源：http://id.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://ag.wgjwhj.cn

[S54] C++：异常处理
来源：http://bp.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xv.9csxet.cn

[S55] C++：结构化绑定
来源：http://ib.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sb.szsharing.cn

[S56] C++：optional
来源：http://nt.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gq.nszjky.cn

[S57] C++：编译期常量
来源：http://mn.nszjky.cn

constexpr int N = 10;
来源：http://sa.bookmarksfly.cn

[S58] C++：命名空间
来源：http://pp.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://ge.wgjwhj.cn

[S59] C++：静态断言
来源：http://ky.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ea.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://se.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cb.huixinmuqiang.cn

================================================================================
来源：http://oj.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sr.nszjky.cn

================================================================================
来源：http://pe.nszjky.cn

[T01] Kotlin：Hello World
来源：http://ia.shxzskj.cn

println("Hello")
来源：http://qk.shxzukj.cn

[T02] Kotlin：变量
来源：http://rc.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://my.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://xu.shtwfgs.cn

"值: $b"
来源：http://kv.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://dp.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://ej.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://ny.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qg.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://bc.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://al.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://vm.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zf.shxzukj.cn

[T08] Kotlin：数据类
来源：http://sg.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://cg.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://hf.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://yp.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://uf.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://di.shtwfgs.cn

[T11] Kotlin：协程
来源：http://lw.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eo.9csxet.cn

[T12] Kotlin：解构声明
来源：http://fk.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://bb.521024.cn

[T13] Kotlin：只读 Map
来源：http://zv.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://cc.shtwfgs.cn

[T14] Kotlin：循环
来源：http://wz.asd995.cn

for (i in 1..10) println(i)
来源：http://og.szsharing.cn

[T15] Kotlin：接口
来源：http://dh.nszjky.cn

interface Shape { fun area(): Double }
来源：http://lk.muxihuayi.cn

[T16] Swift：Hello World
来源：http://nc.chemitech.net.cn

print("Hello")
来源：http://va.huanxung.cn

[T17] Swift：变量与常量
来源：http://ip.nicolike.cn

var a = 1;  let b = 2
来源：http://ph.9csxet.cn

[T18] Swift：字符串插值
来源：http://ik.panjiajie.cn

"值: \(b)"
来源：http://do.hahajie.cn

[T19] Swift：可选绑定
来源：http://nr.colortex.cn

if let n = opt { print(n) }
来源：http://zx.nszjky.cn

[T20] Swift：数组操作
来源：http://fe.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xc.hnjuh.cn

[T21] Swift：遍历
来源：http://ud.huixinmuqiang.cn

for x in a { print(x) }
来源：http://ep.shxzskj.cn

[T22] Swift：字典
来源：http://id.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wx.shtwfgs.cn

[T23] Swift：函数
来源：http://mt.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://al.bookmarksfly.cn

[T24] Swift：闭包
来源：http://vv.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dt.bjjhwx.cn

[T25] Swift：结构体
来源：http://dl.muxihuayi.cn

struct P { var x: Int }
来源：http://bw.newstarts.cn

[T26] Swift：类与重写
来源：http://si.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://ff.chemitech.net.cn

[T27] Swift：错误处理
来源：http://hh.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://iw.asd995.cn

[T28] Swift：枚举
来源：http://zt.shtwfgs.cn

enum Color { case red, green }
来源：http://uu.colortex.cn

[T29] Swift：guard 提前返回
来源：http://dj.gzmigu.cn

guard let x = opt else { return }
来源：http://fc.huixiangedu.cn

[T30] Swift：协议
来源：http://el.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://ho.muxihuayi.cn

[T31] Lua：Hello World
来源：http://fe.nszjky.cn

print("Hello")
来源：http://hc.colortex.cn

[T32] Lua：局部变量
来源：http://jd.szxytkj.cn

local a = 1
来源：http://nz.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://ed.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nh.huanxung.cn

[T34] Lua：遍历表
来源：http://sm.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lr.9csxet.cn

[T35] Lua：字典表
来源：http://iz.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://pw.panjiajie.cn

[T36] Lua：函数
来源：http://wl.wgjwhj.cn

function add(a, b) return a + b end
来源：http://ue.nicolike.cn

[T37] Lua：字符串拼接
来源：http://ym.nicolike.cn

"a" .. "b"
来源：http://kf.panjiajie.cn

[T38] Lua：条件
来源：http://ks.chemitech.net.cn

if x > 0 then print("正") end
来源：http://uf.9csxet.cn

[T39] Lua：模式匹配
来源：http://dx.yuexingan06.cn

string.find(s, "%d+")
来源：http://pf.bjjhwx.cn

[T40] Lua：元表
来源：http://xb.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://zf.huanxung.cn

[T41] Perl：Hello World
来源：http://dx.wgjwhj.cn

print "Hello\n";
来源：http://kn.gzmigu.cn

[T42] Perl：变量类型
来源：http://xg.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zc.hnjuh.cn

[T43] Perl：字符串插值
来源：http://dn.newstarts.cn

"值: $a"
来源：http://lw.yuntaijiaju.cn

[T44] Perl：条件
来源：http://cd.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://kh.huanxung.cn

[T45] Perl：数组遍历
来源：http://ts.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://bg.nicolike.cn

[T46] Perl：哈希操作
来源：http://jt.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oh.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://rw.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://km.huanxung.cn

[T48] Perl：正则替换
来源：http://cb.asd995.cn

$s =~ s/old/new/g;
来源：http://qj.shtwfgs.cn

[T49] Perl：函数
来源：http://yh.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hs.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://wz.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://ve.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://pt.chemitech.net.cn

println("Hello")
来源：http://zh.jctech888.com.cn

[T52] Scala：变量
来源：http://xt.panjiajie.cn

val a = 1;  var b = 2
来源：http://dv.colortex.cn

[T53] Scala：字符串插值
来源：http://bu.nszjky.cn

s"值: $b"
来源：http://sq.hahajie.cn

[T54] Scala：集合映射
来源：http://jl.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://od.szsharing.cn

[T55] Scala：集合过滤
来源：http://zk.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zx.hnjuh.cn

[T56] Scala：样例类
来源：http://do.colortex.cn

case class User(name: String, age: Int)
来源：http://ib.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://qy.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ka.shxzskj.cn

[T58] Scala：函数定义
来源：http://rk.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vy.chemitech.net.cn

[T59] Scala：循环
来源：http://dl.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://kq.huixiangedu.cn

[T60] Scala：折叠
来源：http://we.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oj.szxytkj.cn

================================================================================
来源：http://pj.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ys.panjiajie.cn

================================================================================
来源：http://cq.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://rb.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ia.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://uz.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wj.521024.cn

[U03] Py：加载 .env 配置
来源：http://ec.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zx.panjiajie.cn

[U04] Py：变量调试打印
来源：http://oa.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dv.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://dy.hahajie.cn

list(dict.fromkeys(arr))
来源：http://qt.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://ly.shxzukj.cn

{**a, **b}
来源：http://vn.lnxyls.cn

[U07] Py：反转字典键值
来源：http://hh.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://kw.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://wd.hnjuh.cn

[y for x in nested for y in x]
来源：http://pv.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://ac.chemitech.net.cn

max(d, key=d.get)
来源：http://wc.panjiajie.cn

[U10] Py：按值排序字典
来源：http://nl.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cu.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://lf.jctech888.com.cn

(x * 2 for x in arr)
来源：http://wb.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ba.nicolike.cn

Counter(arr).most_common(3)
来源：http://xn.nicolike.cn

[U13] Py：固定长度队列
来源：http://rg.9csxet.cn

deque(maxlen=10)
来源：http://ll.colortex.cn

[U14] Py：分组收集到列表
来源：http://yq.9csxet.cn

defaultdict(list)
来源：http://ow.shxzskj.cn

[U15] Py：高精度计时
来源：http://ga.huixinmuqiang.cn

t = time.perf_counter()
来源：http://si.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://oe.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cl.colortex.cn

[U17] Py：初始化日志
来源：http://se.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://xh.huanxung.cn

[U18] Py：预编译正则
来源：http://jn.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://lk.colortex.cn

[U19] Py：正则替换带回调
来源：http://tp.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cj.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://do.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://wu.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://cl.yuexingan06.cn

@contextlib.contextmanager
来源：http://di.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://db.szxytkj.cn

list(zip(*m))
来源：http://yq.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://xg.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pk.521024.cn

[U24] Py：路径操作
来源：http://tx.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ng.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://ub.521024.cn

csv.DictReader(f)
来源：http://tv.wgjwhj.cn

[U26] Py：并发下载
来源：http://sl.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qh.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://ys.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://kv.chemitech.net.cn

[U28] Py：类型别名
来源：http://kv.muxihuayi.cn

UserId = int
来源：http://bi.shxzukj.cn

[U29] Py：属性校验
来源：http://ls.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://bw.chemitech.net.cn

[U30] Py：数据类
来源：http://dx.panjiajie.cn

@dataclass(slots=True)
来源：http://ri.jctech888.com.cn

[U31] Py：单测
来源：http://pj.shtwfgs.cn

python -m pytest -q
来源：http://ae.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://nm.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://cp.shxzskj.cn

[U33] Py：打包发布
来源：http://dt.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://yw.newstarts.cn

[U34] Py：判断编码
来源：http://se.yuexingan06.cn

chardet.detect(raw)
来源：http://zf.hahajie.cn

[U35] Py：发送邮件
来源：http://xy.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://au.shtwfgs.cn

[U36] Py：定时任务
来源：http://ol.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://gu.asd995.cn

[U37] Py：读写 Excel
来源：http://qk.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ii.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://qh.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://gc.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://qh.szxytkj.cn

sys.stdout.isatty()
来源：http://ko.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://ka.asd995.cn

print("err", file=sys.stderr)
来源：http://hz.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://nn.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qu.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://wm.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bv.huanxung.cn

[U43] PHP：声明命名空间
来源：http://wf.nicolike.cn

namespace App\Http;
来源：http://ly.huanxung.cn

[U44] PHP：开启严格类型
来源：http://pc.gzmigu.cn

declare(strict_types=1);
来源：http://xd.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://br.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://om.huixiangedu.cn

[U46] PHP：可空类型
来源：http://mi.szxytkj.cn

?string $name = null
来源：http://ev.szsharing.cn

[U47] PHP：联合类型
来源：http://ie.yuexingan06.cn

int|string $id
来源：http://we.9csxet.cn

[U48] PHP：纯枚举
来源：http://mh.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zn.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://wc.huanxung.cn

public readonly string $name
来源：http://yj.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://hi.shxzskj.cn

public function __construct(private int $id) {}
来源：http://oi.muxihuayi.cn


<!-- 参考信息 -->