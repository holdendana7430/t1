代发 wailian999

#ifndef X_H
来源：http://ee.521024.cn

#define X_H
来源：http://rw.bjjhwx.cn

#endif
来源：http://em.521024.cn

[S31] C++：Hello World
来源：http://ep.newstarts.cn

#include <iostream>
来源：http://zm.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://yr.panjiajie.cn

[S32] C++：字符串
来源：http://da.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://vp.asd995.cn

[S33] C++：vector 增删
来源：http://sl.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://do.panjiajie.cn

[S34] C++：遍历 vector
来源：http://tr.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://jv.szsharing.cn

[S35] C++：map
来源：http://lw.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ua.gzmigu.cn

[S36] C++：unordered_map
来源：http://rn.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://de.hahajie.cn

[S37] C++：set
来源：http://ae.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kg.hnjuh.cn

[S38] C++：排序
来源：http://yk.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://wg.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://gy.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yj.newstarts.cn

[S40] C++：查找元素
来源：http://pf.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dt.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://qi.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gu.521024.cn

[S42] C++：继承与虚函数
来源：http://yu.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://sc.panjiajie.cn

[S43] C++：智能指针
来源：http://se.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://yg.huanxung.cn

[S44] C++：引用传参
来源：http://uy.521024.cn

void inc(int &x) { ++x; }
来源：http://iz.wgjwhj.cn

[S45] C++：lambda
来源：http://ee.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wo.nicolike.cn

[S46] C++：函数模板
来源：http://jv.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ua.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://pk.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://al.shxzukj.cn

[S48] C++：逐行读文件
来源：http://dq.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ay.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://rb.jctech888.com.cn

[S49] C++：写文件
来源：http://ea.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://do.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://ip.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mv.panjiajie.cn

[S51] C++：显式类型转换
来源：http://rs.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://wq.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://xd.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://ax.szsharing.cn

[S53] C++：移动语义
来源：http://zp.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://rz.nszjky.cn

[S54] C++：异常处理
来源：http://yb.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ge.newstarts.cn

[S55] C++：结构化绑定
来源：http://gj.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wx.jctech888.com.cn

[S56] C++：optional
来源：http://ru.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://of.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://wr.colortex.cn

constexpr int N = 10;
来源：http://ta.muxihuayi.cn

[S58] C++：命名空间
来源：http://wr.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://me.bookmarksfly.cn

[S59] C++：静态断言
来源：http://js.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tt.asd995.cn

[S60] C++：遍历并删除元素
来源：http://tl.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ks.chemitech.net.cn

================================================================================
来源：http://un.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ot.szsharing.cn

================================================================================
来源：http://vc.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://pg.chemitech.net.cn

println("Hello")
来源：http://oc.hahajie.cn

[T02] Kotlin：变量
来源：http://rh.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://du.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://sz.huixiangedu.cn

"值: $b"
来源：http://xg.newstarts.cn

[T04] Kotlin：空安全
来源：http://ea.newstarts.cn

val n: String? = null;  n?.length
来源：http://jp.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://ki.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://al.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://kc.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eb.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://ng.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cm.newstarts.cn

[T08] Kotlin：数据类
来源：http://tk.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://sw.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://rx.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://dr.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://ye.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fe.newstarts.cn

[T11] Kotlin：协程
来源：http://rt.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dr.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://ba.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://el.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://of.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://us.nszjky.cn

[T14] Kotlin：循环
来源：http://oi.shxzukj.cn

for (i in 1..10) println(i)
来源：http://lu.newstarts.cn

[T15] Kotlin：接口
来源：http://ne.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://ch.haigaiapp.cn

[T16] Swift：Hello World
来源：http://rg.panjiajie.cn

print("Hello")
来源：http://pr.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://gq.hnjuh.cn

var a = 1;  let b = 2
来源：http://ms.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://ho.jctech888.com.cn

"值: \(b)"
来源：http://jk.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://la.newstarts.cn

if let n = opt { print(n) }
来源：http://su.szxytkj.cn

[T20] Swift：数组操作
来源：http://pq.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ao.chemitech.net.cn

[T21] Swift：遍历
来源：http://hn.nicolike.cn

for x in a { print(x) }
来源：http://ay.colortex.cn

[T22] Swift：字典
来源：http://ub.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pl.hahajie.cn

[T23] Swift：函数
来源：http://yr.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gl.shtwfgs.cn

[T24] Swift：闭包
来源：http://qh.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rx.szsharing.cn

[T25] Swift：结构体
来源：http://ue.wgjwhj.cn

struct P { var x: Int }
来源：http://lx.haigaiapp.cn

[T26] Swift：类与重写
来源：http://iw.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://kk.haigaiapp.cn

[T27] Swift：错误处理
来源：http://rh.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://vt.chemitech.net.cn

[T28] Swift：枚举
来源：http://wd.nszjky.cn

enum Color { case red, green }
来源：http://xp.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://kx.wgjwhj.cn

guard let x = opt else { return }
来源：http://ny.newstarts.cn

[T30] Swift：协议
来源：http://kq.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://qx.9csxet.cn

[T31] Lua：Hello World
来源：http://ad.szsharing.cn

print("Hello")
来源：http://em.szxytkj.cn

[T32] Lua：局部变量
来源：http://ww.szsharing.cn

local a = 1
来源：http://tz.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://vd.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mu.wgjwhj.cn

[T34] Lua：遍历表
来源：http://fu.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wb.lnxyls.cn

[T35] Lua：字典表
来源：http://fi.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://rj.huixinmuqiang.cn

[T36] Lua：函数
来源：http://wv.panjiajie.cn

function add(a, b) return a + b end
来源：http://qf.521024.cn

[T37] Lua：字符串拼接
来源：http://rs.panjiajie.cn

"a" .. "b"
来源：http://tb.shxzukj.cn

[T38] Lua：条件
来源：http://wk.haigaiapp.cn

if x > 0 then print("正") end
来源：http://wx.hahajie.cn

[T39] Lua：模式匹配
来源：http://lr.hahajie.cn

string.find(s, "%d+")
来源：http://ir.yuntaijiaju.cn

[T40] Lua：元表
来源：http://uq.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://pi.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://qv.yuexingan06.cn

print "Hello\n";
来源：http://bo.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://yr.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xb.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://hg.wgjwhj.cn

"值: $a"
来源：http://ni.yuntaijiaju.cn

[T44] Perl：条件
来源：http://zk.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://xg.szsharing.cn

[T45] Perl：数组遍历
来源：http://uv.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://ea.9csxet.cn

[T46] Perl：哈希操作
来源：http://am.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fc.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://zn.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oo.gzmigu.cn

[T48] Perl：正则替换
来源：http://fy.gzmigu.cn

$s =~ s/old/new/g;
来源：http://zy.szsharing.cn

[T49] Perl：函数
来源：http://jm.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rq.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://og.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vl.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://gm.hnjuh.cn

[T51] Scala：Hello World
来源：http://em.panjiajie.cn

println("Hello")
来源：http://kc.nicolike.cn

[T52] Scala：变量
来源：http://xu.wgjwhj.cn

val a = 1;  var b = 2
来源：http://cd.nszjky.cn

[T53] Scala：字符串插值
来源：http://cx.wgjwhj.cn

s"值: $b"
来源：http://rf.nicolike.cn

[T54] Scala：集合映射
来源：http://vk.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://rf.hnjuh.cn

[T55] Scala：集合过滤
来源：http://jp.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tq.bookmarksfly.cn

[T56] Scala：样例类
来源：http://tr.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://sr.521024.cn

[T57] Scala：模式匹配
来源：http://xg.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tc.szxytkj.cn

[T58] Scala：函数定义
来源：http://hk.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://am.lnxyls.cn

[T59] Scala：循环
来源：http://hl.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://nq.jctech888.com.cn

[T60] Scala：折叠
来源：http://dh.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://po.shtwfgs.cn

================================================================================
来源：http://lw.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gp.jianghongdianzi.cn

================================================================================
来源：http://is.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://mg.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gx.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://sf.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pw.colortex.cn

[U03] Py：加载 .env 配置
来源：http://ws.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ue.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://pz.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ly.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://yr.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://dw.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://mx.haigaiapp.cn

{**a, **b}
来源：http://rc.szsharing.cn

[U07] Py：反转字典键值
来源：http://ro.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://en.asd995.cn

[U08] Py：展平二维列表
来源：http://ep.lnxyls.cn

[y for x in nested for y in x]
来源：http://cn.asd995.cn

[U09] Py：字典取最大值的键
来源：http://jj.haigaiapp.cn

max(d, key=d.get)
来源：http://uu.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://pr.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ky.hahajie.cn

[U11] Py：生成器表达式
来源：http://pk.hahajie.cn

(x * 2 for x in arr)
来源：http://bn.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qv.szsharing.cn

Counter(arr).most_common(3)
来源：http://av.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://xm.szxytkj.cn

deque(maxlen=10)
来源：http://bg.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://iu.lnxyls.cn

defaultdict(list)
来源：http://ab.nszjky.cn

[U15] Py：高精度计时
来源：http://zt.hahajie.cn

t = time.perf_counter()
来源：http://vx.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://fr.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jx.panjiajie.cn

[U17] Py：初始化日志
来源：http://hb.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ji.jctech888.com.cn

[U18] Py：预编译正则
来源：http://xo.szsharing.cn

pat = re.compile(r"\d+")
来源：http://pc.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://co.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cw.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://fm.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://sn.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://rg.9csxet.cn

@contextlib.contextmanager
来源：http://qu.gzmigu.cn

[U22] Py：矩阵转置
来源：http://ue.nszjky.cn

list(zip(*m))
来源：http://in.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://uu.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ya.szxytkj.cn

[U24] Py：路径操作
来源：http://xu.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fv.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://zb.gzmigu.cn

csv.DictReader(f)
来源：http://pb.wgjwhj.cn

[U26] Py：并发下载
来源：http://cz.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fp.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://cj.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://if.newstarts.cn

[U28] Py：类型别名
来源：http://ex.colortex.cn

UserId = int
来源：http://qt.hahajie.cn

[U29] Py：属性校验
来源：http://vq.lnxyls.cn

@property 与 @x.setter 配合
来源：http://fm.shtwfgs.cn

[U30] Py：数据类
来源：http://yt.szxytkj.cn

@dataclass(slots=True)
来源：http://ei.haigaiapp.cn

[U31] Py：单测
来源：http://zu.nszjky.cn

python -m pytest -q
来源：http://ez.lnxyls.cn

[U32] Py：代码格式化
来源：http://vk.asd995.cn

ruff format . && ruff check --fix .
来源：http://ww.shtwfgs.cn

[U33] Py：打包发布
来源：http://ba.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://mm.nicolike.cn

[U34] Py：判断编码
来源：http://hy.yuexingan06.cn

chardet.detect(raw)
来源：http://hz.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://ym.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wz.shtwfgs.cn

[U36] Py：定时任务
来源：http://uk.521024.cn

schedule.every(10).minutes.do(job)
来源：http://fs.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://eb.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://du.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://mc.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://so.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://pw.nszjky.cn

sys.stdout.isatty()
来源：http://el.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://ai.hnjuh.cn

print("err", file=sys.stderr)
来源：http://jb.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://xe.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rf.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://ql.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yd.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://eh.bookmarksfly.cn

namespace App\Http;
来源：http://lp.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://lh.bookmarksfly.cn

declare(strict_types=1);
来源：http://dp.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://sg.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tq.nszjky.cn

[U46] PHP：可空类型
来源：http://au.asd995.cn

?string $name = null
来源：http://kz.newstarts.cn

[U47] PHP：联合类型
来源：http://on.newstarts.cn

int|string $id
来源：http://ac.bookmarksfly.cn

[U48] PHP：纯枚举
来源：http://vw.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://id.wgjwhj.cn

[U49] PHP：只读属性
来源：http://pa.nszjky.cn

public readonly string $name
来源：http://xd.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://ix.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://os.huixiangedu.cn

[U51] PHP：数组解构
来源：http://os.szxytkj.cn

[$a, $b] = $arr;
来源：http://sk.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://wx.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://gi.szsharing.cn

[U53] PHP：空合并运算符
来源：http://gm.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://ms.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://vx.yuexingan06.cn

$obj?->method()
来源：http://kr.szxytkj.cn


<!-- 参考信息 -->