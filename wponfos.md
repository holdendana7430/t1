代发 wailian999

memset(a, 0, sizeof a);
来源：http://il.wgjwhj.cn

[S27] C：定义常量
来源：http://ne.9csxet.cn

const double PI = 3.14159;
来源：http://py.bookmarksfly.cn

[S28] C：静态变量
来源：http://zm.panjiajie.cn

static int counter = 0;
来源：http://kb.huanxung.cn

[S29] C：变参函数
来源：http://du.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://km.szsharing.cn

[S30] C：头文件保护
来源：http://vv.lnxyls.cn

#ifndef X_H
来源：http://fb.shtwfgs.cn

#define X_H
来源：http://jy.muxihuayi.cn

#endif
来源：http://ge.hnjuh.cn

[S31] C++：Hello World
来源：http://rq.huixinmuqiang.cn

#include <iostream>
来源：http://hr.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://qa.yuntaijiaju.cn

[S32] C++：字符串
来源：http://mb.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://ez.szsharing.cn

[S33] C++：vector 增删
来源：http://ww.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vt.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://tk.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://pm.gzmigu.cn

[S35] C++：map
来源：http://wb.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uc.haigaiapp.cn

[S36] C++：unordered_map
来源：http://bu.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bc.newstarts.cn

[S37] C++：set
来源：http://jn.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ak.shtwfgs.cn

[S38] C++：排序
来源：http://iy.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://eh.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://ea.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sy.wgjwhj.cn

[S40] C++：查找元素
来源：http://ov.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gu.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://xb.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wx.nszjky.cn

[S42] C++：继承与虚函数
来源：http://ar.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://qf.jctech888.com.cn

[S43] C++：智能指针
来源：http://vk.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://uj.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://uf.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://tb.asd995.cn

[S45] C++：lambda
来源：http://dj.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rr.colortex.cn

[S46] C++：函数模板
来源：http://we.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ck.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://vk.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xv.colortex.cn

[S48] C++：逐行读文件
来源：http://xv.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bf.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://gl.bjjhwx.cn

[S49] C++：写文件
来源：http://zl.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gc.chemitech.net.cn

[S50] C++：格式化数字
来源：http://vq.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yy.gzmigu.cn

[S51] C++：显式类型转换
来源：http://zu.bjjhwx.cn

static_cast<double>(a) / b
来源：http://tl.521024.cn

[S52] C++：const 与 noexcept
来源：http://xo.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://rf.yuexingan06.cn

[S53] C++：移动语义
来源：http://kf.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://pf.bookmarksfly.cn

[S54] C++：异常处理
来源：http://rj.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ar.panjiajie.cn

[S55] C++：结构化绑定
来源：http://fl.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ve.bookmarksfly.cn

[S56] C++：optional
来源：http://jq.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qw.9csxet.cn

[S57] C++：编译期常量
来源：http://et.shtwfgs.cn

constexpr int N = 10;
来源：http://bi.szxytkj.cn

[S58] C++：命名空间
来源：http://me.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://ep.nicolike.cn

[S59] C++：静态断言
来源：http://to.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ro.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://nl.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fc.asd995.cn

================================================================================
来源：http://vi.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ox.szsharing.cn

================================================================================
来源：http://bu.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://xx.yuexingan06.cn

println("Hello")
来源：http://dj.shtwfgs.cn

[T02] Kotlin：变量
来源：http://fb.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ts.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://un.bookmarksfly.cn

"值: $b"
来源：http://jp.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://aa.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://xu.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://mc.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ap.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://rd.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://aj.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://we.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sa.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://qu.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://as.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://nr.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://ca.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://yw.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://er.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://nw.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nn.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://qr.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://og.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://bi.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://pp.colortex.cn

[T14] Kotlin：循环
来源：http://ns.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://yk.colortex.cn

[T15] Kotlin：接口
来源：http://tg.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://bp.hnjuh.cn

[T16] Swift：Hello World
来源：http://fi.szxytkj.cn

print("Hello")
来源：http://se.521024.cn

[T17] Swift：变量与常量
来源：http://rj.shxzskj.cn

var a = 1;  let b = 2
来源：http://os.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://gl.bjjhwx.cn

"值: \(b)"
来源：http://ty.huanxung.cn

[T19] Swift：可选绑定
来源：http://rn.521024.cn

if let n = opt { print(n) }
来源：http://mt.nicolike.cn

[T20] Swift：数组操作
来源：http://sg.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wn.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://gc.9csxet.cn

for x in a { print(x) }
来源：http://go.muxihuayi.cn

[T22] Swift：字典
来源：http://ma.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yh.9csxet.cn

[T23] Swift：函数
来源：http://gu.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pb.szxytkj.cn

[T24] Swift：闭包
来源：http://yr.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yt.panjiajie.cn

[T25] Swift：结构体
来源：http://xo.szxytkj.cn

struct P { var x: Int }
来源：http://sz.bjjhwx.cn

[T26] Swift：类与重写
来源：http://kq.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://jt.nicolike.cn

[T27] Swift：错误处理
来源：http://vo.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://ls.jctech888.com.cn

[T28] Swift：枚举
来源：http://rq.asd995.cn

enum Color { case red, green }
来源：http://cp.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://me.hahajie.cn

guard let x = opt else { return }
来源：http://rl.huixiangedu.cn

[T30] Swift：协议
来源：http://xx.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://yr.wgjwhj.cn

[T31] Lua：Hello World
来源：http://mk.szsharing.cn

print("Hello")
来源：http://yh.huanxung.cn

[T32] Lua：局部变量
来源：http://un.huixinmuqiang.cn

local a = 1
来源：http://au.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://fk.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fa.lnxyls.cn

[T34] Lua：遍历表
来源：http://ez.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hi.panjiajie.cn

[T35] Lua：字典表
来源：http://fs.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://yr.nszjky.cn

[T36] Lua：函数
来源：http://ff.shxzskj.cn

function add(a, b) return a + b end
来源：http://qs.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://vg.haigaiapp.cn

"a" .. "b"
来源：http://ha.521024.cn

[T38] Lua：条件
来源：http://md.newstarts.cn

if x > 0 then print("正") end
来源：http://as.nicolike.cn

[T39] Lua：模式匹配
来源：http://vu.haigaiapp.cn

string.find(s, "%d+")
来源：http://qh.huixinmuqiang.cn

[T40] Lua：元表
来源：http://xn.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://ds.jctech888.com.cn

[T41] Perl：Hello World
来源：http://jr.szsharing.cn

print "Hello\n";
来源：http://os.shxzukj.cn

[T42] Perl：变量类型
来源：http://sl.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jl.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://hr.shxzukj.cn

"值: $a"
来源：http://mb.haigaiapp.cn

[T44] Perl：条件
来源：http://zn.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://lz.nicolike.cn

[T45] Perl：数组遍历
来源：http://jw.asd995.cn

for my $x (@arr) { print $x; }
来源：http://re.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://jg.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fi.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://zj.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qz.szsharing.cn

[T48] Perl：正则替换
来源：http://tb.nicolike.cn

$s =~ s/old/new/g;
来源：http://yn.muxihuayi.cn

[T49] Perl：函数
来源：http://ee.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wz.newstarts.cn

[T50] Perl：逐行读文件
来源：http://ov.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ju.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://eu.huanxung.cn

[T51] Scala：Hello World
来源：http://ci.521024.cn

println("Hello")
来源：http://td.yuexingan06.cn

[T52] Scala：变量
来源：http://ob.asd995.cn

val a = 1;  var b = 2
来源：http://kg.lnxyls.cn

[T53] Scala：字符串插值
来源：http://cd.yuntaijiaju.cn

s"值: $b"
来源：http://py.nszjky.cn

[T54] Scala：集合映射
来源：http://zg.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://nr.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://js.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mf.szxytkj.cn

[T56] Scala：样例类
来源：http://ry.shxzukj.cn

case class User(name: String, age: Int)
来源：http://sc.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://ut.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gt.szsharing.cn

[T58] Scala：函数定义
来源：http://it.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tz.shtwfgs.cn

[T59] Scala：循环
来源：http://iq.521024.cn

for (i <- 1 to 10) println(i)
来源：http://al.jctech888.com.cn

[T60] Scala：折叠
来源：http://pp.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cw.colortex.cn

================================================================================
来源：http://vs.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yk.jianghongdianzi.cn

================================================================================
来源：http://wh.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://cq.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xs.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://ud.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gc.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://ki.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ur.colortex.cn

[U04] Py：变量调试打印
来源：http://zy.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lc.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://jh.colortex.cn

list(dict.fromkeys(arr))
来源：http://qr.shxzskj.cn

[U06] Py：合并两个字典
来源：http://in.wgjwhj.cn

{**a, **b}
来源：http://vb.521024.cn

[U07] Py：反转字典键值
来源：http://br.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://cu.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://lp.szxytkj.cn

[y for x in nested for y in x]
来源：http://dj.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://yh.nszjky.cn

max(d, key=d.get)
来源：http://pe.nszjky.cn

[U10] Py：按值排序字典
来源：http://ob.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ve.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://sc.shxzukj.cn

(x * 2 for x in arr)
来源：http://ss.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rq.hahajie.cn

Counter(arr).most_common(3)
来源：http://hh.lnxyls.cn

[U13] Py：固定长度队列
来源：http://xs.asd995.cn

deque(maxlen=10)
来源：http://yt.newstarts.cn

[U14] Py：分组收集到列表
来源：http://op.bookmarksfly.cn

defaultdict(list)
来源：http://mr.shtwfgs.cn

[U15] Py：高精度计时
来源：http://pi.asd995.cn

t = time.perf_counter()
来源：http://hu.huanxung.cn

[U16] Py：命令行参数解析
来源：http://hd.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yp.huixiangedu.cn

[U17] Py：初始化日志
来源：http://mv.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://ww.szsharing.cn

[U18] Py：预编译正则
来源：http://qv.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://eh.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://om.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cj.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://ov.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://ro.521024.cn

[U21] Py：自定义上下文管理器
来源：http://hb.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://uu.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://zx.huanxung.cn

list(zip(*m))
来源：http://fn.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://qf.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://re.haigaiapp.cn

[U24] Py：路径操作
来源：http://mv.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rm.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://cu.huixiangedu.cn

csv.DictReader(f)
来源：http://ti.shxzukj.cn

[U26] Py：并发下载
来源：http://re.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nb.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://ui.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://zc.shtwfgs.cn

[U28] Py：类型别名
来源：http://dj.jctech888.com.cn

UserId = int
来源：http://el.haigaiapp.cn

[U29] Py：属性校验
来源：http://wk.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://ut.shxzskj.cn

[U30] Py：数据类
来源：http://yn.muxihuayi.cn

@dataclass(slots=True)
来源：http://ac.huixiangedu.cn

[U31] Py：单测
来源：http://lg.newstarts.cn

python -m pytest -q
来源：http://hd.bjjhwx.cn

[U32] Py：代码格式化
来源：http://al.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://rd.jctech888.com.cn

[U33] Py：打包发布
来源：http://ss.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://ao.szxytkj.cn

[U34] Py：判断编码
来源：http://rv.huanxung.cn

chardet.detect(raw)
来源：http://rp.gzmigu.cn

[U35] Py：发送邮件
来源：http://fm.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dn.colortex.cn

[U36] Py：定时任务
来源：http://xq.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://bf.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://zl.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bw.521024.cn

[U38] Py：获取脚本所在目录
来源：http://ug.hahajie.cn

Path(__file__).resolve().parent
来源：http://cq.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://mk.panjiajie.cn

sys.stdout.isatty()
来源：http://mi.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://ck.huanxung.cn

print("err", file=sys.stderr)
来源：http://jx.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ia.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://za.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://qn.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rb.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://ys.huixinmuqiang.cn

namespace App\Http;
来源：http://io.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://tv.shtwfgs.cn

declare(strict_types=1);
来源：http://do.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://ih.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xu.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://ns.nicolike.cn

?string $name = null
来源：http://yf.yuexingan06.cn

[U47] PHP：联合类型
来源：http://rf.newstarts.cn

int|string $id
来源：http://pl.newstarts.cn

[U48] PHP：纯枚举
来源：http://zl.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ti.asd995.cn

[U49] PHP：只读属性
来源：http://gx.panjiajie.cn

public readonly string $name
来源：http://if.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://nx.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://jb.hnjuh.cn


<!-- 参考信息 -->