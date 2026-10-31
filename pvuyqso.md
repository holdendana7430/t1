代发 wailian999

#ifndef X_H
来源：http://ad.bookmarksfly.cn

#define X_H
来源：http://qz.9csxet.cn

#endif
来源：http://ya.haigaiapp.cn

[S31] C++：Hello World
来源：http://dz.huixinmuqiang.cn

#include <iostream>
来源：http://ll.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://zm.521024.cn

[S32] C++：字符串
来源：http://cq.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://os.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://ad.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lo.huanxung.cn

[S34] C++：遍历 vector
来源：http://jp.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://dx.asd995.cn

[S35] C++：map
来源：http://ir.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zk.shxzukj.cn

[S36] C++：unordered_map
来源：http://yb.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mm.bjjhwx.cn

[S37] C++：set
来源：http://yh.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://md.shxzskj.cn

[S38] C++：排序
来源：http://by.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://rm.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://yf.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fh.yuexingan06.cn

[S40] C++：查找元素
来源：http://fh.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xi.newstarts.cn

[S41] C++：类与构造函数
来源：http://wu.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rf.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://me.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://za.chemitech.net.cn

[S43] C++：智能指针
来源：http://dr.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://hi.shxzskj.cn

[S44] C++：引用传参
来源：http://ev.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://fg.yuntaijiaju.cn

[S45] C++：lambda
来源：http://ci.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lv.wgjwhj.cn

[S46] C++：函数模板
来源：http://ir.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gk.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://na.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ao.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://lb.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://le.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://vj.hahajie.cn

[S49] C++：写文件
来源：http://ea.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sb.bjjhwx.cn

[S50] C++：格式化数字
来源：http://xq.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fn.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://kq.nszjky.cn

static_cast<double>(a) / b
来源：http://do.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://ll.huanxung.cn

int size() const noexcept { return n_; }
来源：http://oz.gzmigu.cn

[S53] C++：移动语义
来源：http://ag.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://ks.jctech888.com.cn

[S54] C++：异常处理
来源：http://xu.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tl.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://lq.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ea.bjjhwx.cn

[S56] C++：optional
来源：http://bb.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xw.newstarts.cn

[S57] C++：编译期常量
来源：http://ij.panjiajie.cn

constexpr int N = 10;
来源：http://ql.shtwfgs.cn

[S58] C++：命名空间
来源：http://xn.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://vs.yuexingan06.cn

[S59] C++：静态断言
来源：http://ju.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yv.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://lf.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://to.bjjhwx.cn

================================================================================
来源：http://nq.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jn.hahajie.cn

================================================================================
来源：http://el.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://bs.asd995.cn

println("Hello")
来源：http://rg.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://nf.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ki.asd995.cn

[T03] Kotlin：字符串模板
来源：http://dq.yuntaijiaju.cn

"值: $b"
来源：http://cy.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://ch.huanxung.cn

val n: String? = null;  n?.length
来源：http://lz.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://cy.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://td.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://sc.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yj.521024.cn

[T07] Kotlin：集合过滤
来源：http://sp.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ib.lnxyls.cn

[T08] Kotlin：数据类
来源：http://fo.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://pt.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://by.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://ee.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://fk.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dx.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://bd.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jp.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://tt.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://bv.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://ue.asd995.cn

val m = mapOf("a" to 1)
来源：http://hr.szsharing.cn

[T14] Kotlin：循环
来源：http://xi.shxzukj.cn

for (i in 1..10) println(i)
来源：http://gv.jctech888.com.cn

[T15] Kotlin：接口
来源：http://ig.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://on.shxzskj.cn

[T16] Swift：Hello World
来源：http://rg.colortex.cn

print("Hello")
来源：http://pm.asd995.cn

[T17] Swift：变量与常量
来源：http://bl.jctech888.com.cn

var a = 1;  let b = 2
来源：http://qo.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://nu.hnjuh.cn

"值: \(b)"
来源：http://ab.shxzukj.cn

[T19] Swift：可选绑定
来源：http://bb.newstarts.cn

if let n = opt { print(n) }
来源：http://qb.huixiangedu.cn

[T20] Swift：数组操作
来源：http://qy.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hg.shxzukj.cn

[T21] Swift：遍历
来源：http://pc.wgjwhj.cn

for x in a { print(x) }
来源：http://lr.lnxyls.cn

[T22] Swift：字典
来源：http://si.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zd.haigaiapp.cn

[T23] Swift：函数
来源：http://gs.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xp.panjiajie.cn

[T24] Swift：闭包
来源：http://ry.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nd.colortex.cn

[T25] Swift：结构体
来源：http://wu.huixiangedu.cn

struct P { var x: Int }
来源：http://lt.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://an.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://bp.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://sh.nicolike.cn

do { try f() } catch { print(error) }
来源：http://vp.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://eq.jctech888.com.cn

enum Color { case red, green }
来源：http://cp.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://as.wgjwhj.cn

guard let x = opt else { return }
来源：http://rh.shtwfgs.cn

[T30] Swift：协议
来源：http://pu.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://sh.gzmigu.cn

[T31] Lua：Hello World
来源：http://el.gzmigu.cn

print("Hello")
来源：http://jx.wgjwhj.cn

[T32] Lua：局部变量
来源：http://zh.wgjwhj.cn

local a = 1
来源：http://fx.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://ip.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vq.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://es.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lg.jctech888.com.cn

[T35] Lua：字典表
来源：http://dq.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://vi.asd995.cn

[T36] Lua：函数
来源：http://ux.chemitech.net.cn

function add(a, b) return a + b end
来源：http://aq.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://xg.bookmarksfly.cn

"a" .. "b"
来源：http://mi.wgjwhj.cn

[T38] Lua：条件
来源：http://mk.hahajie.cn

if x > 0 then print("正") end
来源：http://sx.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://qh.shxzukj.cn

string.find(s, "%d+")
来源：http://yh.huixinmuqiang.cn

[T40] Lua：元表
来源：http://rx.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://cr.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://xo.nszjky.cn

print "Hello\n";
来源：http://hf.shtwfgs.cn

[T42] Perl：变量类型
来源：http://ul.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://df.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://zh.bjjhwx.cn

"值: $a"
来源：http://jf.jctech888.com.cn

[T44] Perl：条件
来源：http://xt.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://ec.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://fg.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://wm.szxytkj.cn

[T46] Perl：哈希操作
来源：http://av.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zk.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://fy.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jz.9csxet.cn

[T48] Perl：正则替换
来源：http://nw.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://vf.muxihuayi.cn

[T49] Perl：函数
来源：http://cy.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tl.newstarts.cn

[T50] Perl：逐行读文件
来源：http://tf.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vr.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://dh.jctech888.com.cn

[T51] Scala：Hello World
来源：http://to.gzmigu.cn

println("Hello")
来源：http://pm.jianghongdianzi.cn

[T52] Scala：变量
来源：http://qo.newstarts.cn

val a = 1;  var b = 2
来源：http://rx.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://oe.bjjhwx.cn

s"值: $b"
来源：http://kr.shxzskj.cn

[T54] Scala：集合映射
来源：http://ro.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://it.newstarts.cn

[T55] Scala：集合过滤
来源：http://mr.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yi.haigaiapp.cn

[T56] Scala：样例类
来源：http://la.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://kx.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://ex.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hi.shxzukj.cn

[T58] Scala：函数定义
来源：http://gi.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://as.jianghongdianzi.cn

[T59] Scala：循环
来源：http://vv.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://kl.colortex.cn

[T60] Scala：折叠
来源：http://tz.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://do.huanxung.cn

================================================================================
来源：http://dw.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kn.huixiangedu.cn

================================================================================
来源：http://dr.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://wl.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cp.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://tx.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://om.521024.cn

[U03] Py：加载 .env 配置
来源：http://mm.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gu.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://my.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://di.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://yz.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://ok.nszjky.cn

[U06] Py：合并两个字典
来源：http://lg.9csxet.cn

{**a, **b}
来源：http://cc.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://im.nicolike.cn

{v: k for k, v in d.items()}
来源：http://wh.newstarts.cn

[U08] Py：展平二维列表
来源：http://ra.colortex.cn

[y for x in nested for y in x]
来源：http://un.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://kj.nszjky.cn

max(d, key=d.get)
来源：http://xk.panjiajie.cn

[U10] Py：按值排序字典
来源：http://tt.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://us.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://nt.9csxet.cn

(x * 2 for x in arr)
来源：http://bt.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fq.colortex.cn

Counter(arr).most_common(3)
来源：http://si.hnjuh.cn

[U13] Py：固定长度队列
来源：http://rh.521024.cn

deque(maxlen=10)
来源：http://mv.9csxet.cn

[U14] Py：分组收集到列表
来源：http://hq.yuexingan06.cn

defaultdict(list)
来源：http://rp.nszjky.cn

[U15] Py：高精度计时
来源：http://kt.newstarts.cn

t = time.perf_counter()
来源：http://sk.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://dd.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qz.521024.cn

[U17] Py：初始化日志
来源：http://fd.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://lx.bjjhwx.cn

[U18] Py：预编译正则
来源：http://ju.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://jh.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://cg.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wm.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://pm.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://hc.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://hu.bjjhwx.cn

@contextlib.contextmanager
来源：http://bd.nicolike.cn

[U22] Py：矩阵转置
来源：http://hk.szxytkj.cn

list(zip(*m))
来源：http://il.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://jt.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zi.wgjwhj.cn

[U24] Py：路径操作
来源：http://oh.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fk.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://fp.panjiajie.cn

csv.DictReader(f)
来源：http://zm.yuexingan06.cn

[U26] Py：并发下载
来源：http://og.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mq.asd995.cn

[U27] Py：异步 HTTP
来源：http://td.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://kn.szsharing.cn

[U28] Py：类型别名
来源：http://th.yuntaijiaju.cn

UserId = int
来源：http://nh.gzmigu.cn

[U29] Py：属性校验
来源：http://ot.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://yl.colortex.cn

[U30] Py：数据类
来源：http://cg.panjiajie.cn

@dataclass(slots=True)
来源：http://aw.jctech888.com.cn

[U31] Py：单测
来源：http://ux.wgjwhj.cn

python -m pytest -q
来源：http://ee.521024.cn

[U32] Py：代码格式化
来源：http://jw.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://ig.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://yj.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://pp.gzmigu.cn

[U34] Py：判断编码
来源：http://nc.521024.cn

chardet.detect(raw)
来源：http://qm.9csxet.cn

[U35] Py：发送邮件
来源：http://fa.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wp.yuexingan06.cn

[U36] Py：定时任务
来源：http://cl.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://ij.shxzskj.cn

[U37] Py：读写 Excel
来源：http://cr.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oz.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://mo.szxytkj.cn

Path(__file__).resolve().parent
来源：http://pt.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://ag.shtwfgs.cn

sys.stdout.isatty()
来源：http://lz.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://eq.shxzskj.cn

print("err", file=sys.stderr)
来源：http://or.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://ul.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vp.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://ay.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cb.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://es.szxytkj.cn

namespace App\Http;
来源：http://tw.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://hk.nszjky.cn

declare(strict_types=1);
来源：http://am.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://nl.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sr.szsharing.cn

[U46] PHP：可空类型
来源：http://mw.szsharing.cn

?string $name = null
来源：http://fr.asd995.cn

[U47] PHP：联合类型
来源：http://bq.bjjhwx.cn

int|string $id
来源：http://ik.521024.cn

[U48] PHP：纯枚举
来源：http://ki.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ul.szxytkj.cn

[U49] PHP：只读属性
来源：http://ls.hnjuh.cn

public readonly string $name
来源：http://rc.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://es.wgjwhj.cn

public function __construct(private int $id) {}
来源：http://hf.yuexingan06.cn

[U51] PHP：数组解构
来源：http://qg.nszjky.cn

[$a, $b] = $arr;
来源：http://ky.newstarts.cn

[U52] PHP：箭头函数
来源：http://yd.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://el.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://ih.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://mw.hnjuh.cn

[U54] PHP：空安全调用
来源：http://tx.bookmarksfly.cn

$obj?->method()
来源：http://ap.521024.cn


<!-- 参考信息 -->