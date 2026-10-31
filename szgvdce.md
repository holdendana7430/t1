代发 wailian999

#ifndef X_H
来源：http://fh.gzmigu.cn

#define X_H
来源：http://vs.asd995.cn

#endif
来源：http://eq.lnxyls.cn

[S31] C++：Hello World
来源：http://fm.9csxet.cn

#include <iostream>
来源：http://gx.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://bh.hahajie.cn

[S32] C++：字符串
来源：http://zi.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://mz.hnjuh.cn

[S33] C++：vector 增删
来源：http://ja.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sn.colortex.cn

[S34] C++：遍历 vector
来源：http://df.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://ue.yuexingan06.cn

[S35] C++：map
来源：http://ac.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sa.panjiajie.cn

[S36] C++：unordered_map
来源：http://ir.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wf.newstarts.cn

[S37] C++：set
来源：http://sk.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yo.muxihuayi.cn

[S38] C++：排序
来源：http://qn.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://xm.asd995.cn

[S39] C++：自定义比较器排序
来源：http://nk.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ok.9csxet.cn

[S40] C++：查找元素
来源：http://ys.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zt.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://oz.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fh.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://di.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://ol.szxytkj.cn

[S43] C++：智能指针
来源：http://zy.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://of.wgjwhj.cn

[S44] C++：引用传参
来源：http://hh.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://td.chemitech.net.cn

[S45] C++：lambda
来源：http://as.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vf.huixiangedu.cn

[S46] C++：函数模板
来源：http://io.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kf.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://yg.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ig.newstarts.cn

[S48] C++：逐行读文件
来源：http://qi.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lu.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://yp.9csxet.cn

[S49] C++：写文件
来源：http://gz.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nn.szsharing.cn

[S50] C++：格式化数字
来源：http://ev.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pf.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://ge.szsharing.cn

static_cast<double>(a) / b
来源：http://bt.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://ih.colortex.cn

int size() const noexcept { return n_; }
来源：http://bf.hahajie.cn

[S53] C++：移动语义
来源：http://wl.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://mi.szsharing.cn

[S54] C++：异常处理
来源：http://zd.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rr.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://iv.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://in.shxzukj.cn

[S56] C++：optional
来源：http://fk.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gk.szsharing.cn

[S57] C++：编译期常量
来源：http://sa.nicolike.cn

constexpr int N = 10;
来源：http://rc.huixiangedu.cn

[S58] C++：命名空间
来源：http://rj.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://pa.huixiangedu.cn

[S59] C++：静态断言
来源：http://gu.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yy.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://oe.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mr.yuntaijiaju.cn

================================================================================
来源：http://zh.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yv.nszjky.cn

================================================================================
来源：http://dd.szsharing.cn

[T01] Kotlin：Hello World
来源：http://pt.haigaiapp.cn

println("Hello")
来源：http://uz.muxihuayi.cn

[T02] Kotlin：变量
来源：http://ai.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xt.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://jw.panjiajie.cn

"值: $b"
来源：http://vf.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://ai.gzmigu.cn

val n: String? = null;  n?.length
来源：http://xb.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://eg.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lo.9csxet.cn

[T06] Kotlin：集合映射
来源：http://wl.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bz.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://qu.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://am.shxzukj.cn

[T08] Kotlin：数据类
来源：http://ix.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://kn.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://eu.colortex.cn

fun String.exclaim() = this + "!"
来源：http://sh.asd995.cn

[T10] Kotlin：默认参数
来源：http://lp.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ep.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://di.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eb.hahajie.cn

[T12] Kotlin：解构声明
来源：http://hn.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://ek.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://ap.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://qw.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://zz.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://cm.521024.cn

[T15] Kotlin：接口
来源：http://sx.szsharing.cn

interface Shape { fun area(): Double }
来源：http://lg.asd995.cn

[T16] Swift：Hello World
来源：http://sq.lnxyls.cn

print("Hello")
来源：http://li.nszjky.cn

[T17] Swift：变量与常量
来源：http://ts.szxytkj.cn

var a = 1;  let b = 2
来源：http://ox.newstarts.cn

[T18] Swift：字符串插值
来源：http://wm.huixinmuqiang.cn

"值: \(b)"
来源：http://hx.9csxet.cn

[T19] Swift：可选绑定
来源：http://qr.lnxyls.cn

if let n = opt { print(n) }
来源：http://wd.szsharing.cn

[T20] Swift：数组操作
来源：http://sc.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pm.asd995.cn

[T21] Swift：遍历
来源：http://no.huanxung.cn

for x in a { print(x) }
来源：http://lp.jctech888.com.cn

[T22] Swift：字典
来源：http://sq.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xx.muxihuayi.cn

[T23] Swift：函数
来源：http://pe.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sj.muxihuayi.cn

[T24] Swift：闭包
来源：http://kd.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jf.hnjuh.cn

[T25] Swift：结构体
来源：http://rw.szsharing.cn

struct P { var x: Int }
来源：http://ve.9csxet.cn

[T26] Swift：类与重写
来源：http://os.shxzskj.cn

class A: Base { override func f() {} }
来源：http://dp.nszjky.cn

[T27] Swift：错误处理
来源：http://ok.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://ef.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://fy.521024.cn

enum Color { case red, green }
来源：http://ci.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://bt.nszjky.cn

guard let x = opt else { return }
来源：http://pu.nszjky.cn

[T30] Swift：协议
来源：http://ch.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://yb.szsharing.cn

[T31] Lua：Hello World
来源：http://jc.colortex.cn

print("Hello")
来源：http://ph.wgjwhj.cn

[T32] Lua：局部变量
来源：http://sq.bjjhwx.cn

local a = 1
来源：http://oa.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://xe.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vr.hnjuh.cn

[T34] Lua：遍历表
来源：http://ka.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cv.nszjky.cn

[T35] Lua：字典表
来源：http://hg.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://id.hnjuh.cn

[T36] Lua：函数
来源：http://xx.colortex.cn

function add(a, b) return a + b end
来源：http://so.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://mb.colortex.cn

"a" .. "b"
来源：http://jx.yuntaijiaju.cn

[T38] Lua：条件
来源：http://jm.nicolike.cn

if x > 0 then print("正") end
来源：http://oc.521024.cn

[T39] Lua：模式匹配
来源：http://cx.huixiangedu.cn

string.find(s, "%d+")
来源：http://si.huixiangedu.cn

[T40] Lua：元表
来源：http://wt.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://hp.9csxet.cn

[T41] Perl：Hello World
来源：http://vg.panjiajie.cn

print "Hello\n";
来源：http://gb.asd995.cn

[T42] Perl：变量类型
来源：http://mx.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jw.gzmigu.cn

[T43] Perl：字符串插值
来源：http://vc.szsharing.cn

"值: $a"
来源：http://lo.jctech888.com.cn

[T44] Perl：条件
来源：http://lr.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://pf.shxzskj.cn

[T45] Perl：数组遍历
来源：http://uo.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://fa.hahajie.cn

[T46] Perl：哈希操作
来源：http://if.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cu.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://qf.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hj.shxzukj.cn

[T48] Perl：正则替换
来源：http://bt.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://tc.bjjhwx.cn

[T49] Perl：函数
来源：http://mf.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fn.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://ws.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wv.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://os.newstarts.cn

[T51] Scala：Hello World
来源：http://wd.shxzskj.cn

println("Hello")
来源：http://vd.szxytkj.cn

[T52] Scala：变量
来源：http://xr.hnjuh.cn

val a = 1;  var b = 2
来源：http://rx.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://dt.szsharing.cn

s"值: $b"
来源：http://yk.huanxung.cn

[T54] Scala：集合映射
来源：http://gx.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://gf.szxytkj.cn

[T55] Scala：集合过滤
来源：http://at.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dv.hahajie.cn

[T56] Scala：样例类
来源：http://kl.colortex.cn

case class User(name: String, age: Int)
来源：http://aw.shxzskj.cn

[T57] Scala：模式匹配
来源：http://gy.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wo.wgjwhj.cn

[T58] Scala：函数定义
来源：http://cy.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ld.szxytkj.cn

[T59] Scala：循环
来源：http://cc.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://rc.asd995.cn

[T60] Scala：折叠
来源：http://ih.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cb.jctech888.com.cn

================================================================================
来源：http://za.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tv.muxihuayi.cn

================================================================================
来源：http://ol.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://db.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ei.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://rf.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tz.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://sp.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iw.asd995.cn

[U04] Py：变量调试打印
来源：http://ez.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pm.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://cm.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://xz.szsharing.cn

[U06] Py：合并两个字典
来源：http://jh.szsharing.cn

{**a, **b}
来源：http://nv.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://bd.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://uz.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://zt.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://mt.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://ao.bookmarksfly.cn

max(d, key=d.get)
来源：http://pn.521024.cn

[U10] Py：按值排序字典
来源：http://uq.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dd.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://ku.wgjwhj.cn

(x * 2 for x in arr)
来源：http://fk.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://re.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://wc.shxzukj.cn

[U13] Py：固定长度队列
来源：http://tx.chemitech.net.cn

deque(maxlen=10)
来源：http://bx.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://yf.bookmarksfly.cn

defaultdict(list)
来源：http://hv.jctech888.com.cn

[U15] Py：高精度计时
来源：http://te.panjiajie.cn

t = time.perf_counter()
来源：http://eb.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://ah.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bn.newstarts.cn

[U17] Py：初始化日志
来源：http://af.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://yh.hnjuh.cn

[U18] Py：预编译正则
来源：http://jy.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://jr.szsharing.cn

[U19] Py：正则替换带回调
来源：http://sx.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://in.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://ls.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://xd.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://xn.lnxyls.cn

@contextlib.contextmanager
来源：http://ow.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://er.muxihuayi.cn

list(zip(*m))
来源：http://tk.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://ga.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ll.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://oz.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://as.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://tq.jctech888.com.cn

csv.DictReader(f)
来源：http://yd.nicolike.cn

[U26] Py：并发下载
来源：http://om.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fs.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://vk.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://gg.bjjhwx.cn

[U28] Py：类型别名
来源：http://hv.521024.cn

UserId = int
来源：http://db.jctech888.com.cn

[U29] Py：属性校验
来源：http://ud.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://rg.yuntaijiaju.cn

[U30] Py：数据类
来源：http://ew.hahajie.cn

@dataclass(slots=True)
来源：http://im.panjiajie.cn

[U31] Py：单测
来源：http://yu.szsharing.cn

python -m pytest -q
来源：http://qr.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://sg.chemitech.net.cn

ruff format . && ruff check --fix .
来源：http://pi.colortex.cn

[U33] Py：打包发布
来源：http://gv.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://yo.gzmigu.cn

[U34] Py：判断编码
来源：http://sa.9csxet.cn

chardet.detect(raw)
来源：http://wc.shxzukj.cn

[U35] Py：发送邮件
来源：http://wd.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jp.huixiangedu.cn

[U36] Py：定时任务
来源：http://xx.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://ne.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://xk.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://is.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://xj.szxytkj.cn

Path(__file__).resolve().parent
来源：http://ec.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://md.nicolike.cn

sys.stdout.isatty()
来源：http://ek.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://vb.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://dx.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://hy.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ke.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://ku.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ny.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://nm.9csxet.cn

namespace App\Http;
来源：http://kq.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://em.huixinmuqiang.cn

declare(strict_types=1);
来源：http://uz.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://ls.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://og.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://hp.shtwfgs.cn

?string $name = null
来源：http://kp.9csxet.cn

[U47] PHP：联合类型
来源：http://qm.muxihuayi.cn

int|string $id
来源：http://bo.szxytkj.cn

[U48] PHP：纯枚举
来源：http://ys.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ww.asd995.cn

[U49] PHP：只读属性
来源：http://kz.huixiangedu.cn

public readonly string $name
来源：http://sa.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://hg.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://hj.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://gq.nicolike.cn

[$a, $b] = $arr;
来源：http://ri.newstarts.cn

[U52] PHP：箭头函数
来源：http://au.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://dg.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://ch.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://az.szxytkj.cn

[U54] PHP：空安全调用
来源：http://av.bjjhwx.cn

$obj?->method()
来源：http://xs.huixinmuqiang.cn


<!-- 参考信息 -->