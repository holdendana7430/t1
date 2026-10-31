代发 wailian999

static int counter = 0;
来源：http://gf.jianghongdianzi.cn

[S29] C：变参函数
来源：http://ju.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jw.bookmarksfly.cn

[S30] C：头文件保护
来源：http://ul.bookmarksfly.cn

#ifndef X_H
来源：http://vx.muxihuayi.cn

#define X_H
来源：http://zy.wgjwhj.cn

#endif
来源：http://um.gzmigu.cn

[S31] C++：Hello World
来源：http://kg.newstarts.cn

#include <iostream>
来源：http://ux.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://si.gzmigu.cn

[S32] C++：字符串
来源：http://lq.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://fw.hnjuh.cn

[S33] C++：vector 增删
来源：http://rq.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ml.huanxung.cn

[S34] C++：遍历 vector
来源：http://gg.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://di.huanxung.cn

[S35] C++：map
来源：http://on.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dz.nicolike.cn

[S36] C++：unordered_map
来源：http://ne.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gm.haigaiapp.cn

[S37] C++：set
来源：http://js.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://df.szsharing.cn

[S38] C++：排序
来源：http://th.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://kn.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://ai.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cx.szxytkj.cn

[S40] C++：查找元素
来源：http://sw.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ep.shxzukj.cn

[S41] C++：类与构造函数
来源：http://kl.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pc.hahajie.cn

[S42] C++：继承与虚函数
来源：http://iy.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://ta.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://dj.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://tx.bookmarksfly.cn

[S44] C++：引用传参
来源：http://dh.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://dr.hnjuh.cn

[S45] C++：lambda
来源：http://gv.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lz.yuexingan06.cn

[S46] C++：函数模板
来源：http://ob.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sz.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://nb.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bs.huanxung.cn

[S48] C++：逐行读文件
来源：http://ud.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uz.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://vp.nicolike.cn

[S49] C++：写文件
来源：http://be.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://io.wgjwhj.cn

[S50] C++：格式化数字
来源：http://st.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ux.szxytkj.cn

[S51] C++：显式类型转换
来源：http://xd.gzmigu.cn

static_cast<double>(a) / b
来源：http://lo.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://zb.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://ht.szxytkj.cn

[S53] C++：移动语义
来源：http://xb.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://zc.muxihuayi.cn

[S54] C++：异常处理
来源：http://sf.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gn.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://am.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qa.szsharing.cn

[S56] C++：optional
来源：http://xd.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qo.huanxung.cn

[S57] C++：编译期常量
来源：http://fn.lnxyls.cn

constexpr int N = 10;
来源：http://zm.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://ev.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://hh.szxytkj.cn

[S59] C++：静态断言
来源：http://cd.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fv.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://wn.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://km.newstarts.cn

================================================================================
来源：http://kz.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eh.huixiangedu.cn

================================================================================
来源：http://lu.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://hq.bjjhwx.cn

println("Hello")
来源：http://is.szsharing.cn

[T02] Kotlin：变量
来源：http://mh.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yz.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://pm.asd995.cn

"值: $b"
来源：http://pr.newstarts.cn

[T04] Kotlin：空安全
来源：http://ze.nszjky.cn

val n: String? = null;  n?.length
来源：http://lq.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://zw.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ab.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://qh.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rw.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://tt.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qn.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://su.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://gs.colortex.cn

[T09] Kotlin：扩展函数
来源：http://dp.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://bz.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://vb.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nq.huixiangedu.cn

[T11] Kotlin：协程
来源：http://ak.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bo.521024.cn

[T12] Kotlin：解构声明
来源：http://de.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://ea.colortex.cn

[T13] Kotlin：只读 Map
来源：http://co.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://tl.haigaiapp.cn

[T14] Kotlin：循环
来源：http://ss.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://ye.muxihuayi.cn

[T15] Kotlin：接口
来源：http://sk.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://kg.newstarts.cn

[T16] Swift：Hello World
来源：http://fv.shtwfgs.cn

print("Hello")
来源：http://ld.asd995.cn

[T17] Swift：变量与常量
来源：http://zi.gzmigu.cn

var a = 1;  let b = 2
来源：http://xo.shxzukj.cn

[T18] Swift：字符串插值
来源：http://ws.muxihuayi.cn

"值: \(b)"
来源：http://ai.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://gp.gzmigu.cn

if let n = opt { print(n) }
来源：http://rg.wgjwhj.cn

[T20] Swift：数组操作
来源：http://wz.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pu.wgjwhj.cn

[T21] Swift：遍历
来源：http://aw.huixinmuqiang.cn

for x in a { print(x) }
来源：http://lp.shtwfgs.cn

[T22] Swift：字典
来源：http://rl.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wz.lnxyls.cn

[T23] Swift：函数
来源：http://ch.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yd.lnxyls.cn

[T24] Swift：闭包
来源：http://yo.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xj.bjjhwx.cn

[T25] Swift：结构体
来源：http://nd.haigaiapp.cn

struct P { var x: Int }
来源：http://ol.nicolike.cn

[T26] Swift：类与重写
来源：http://ps.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://gx.gzmigu.cn

[T27] Swift：错误处理
来源：http://fn.nicolike.cn

do { try f() } catch { print(error) }
来源：http://pv.huanxung.cn

[T28] Swift：枚举
来源：http://fw.9csxet.cn

enum Color { case red, green }
来源：http://ht.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://cw.9csxet.cn

guard let x = opt else { return }
来源：http://ct.lnxyls.cn

[T30] Swift：协议
来源：http://dw.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://ru.colortex.cn

[T31] Lua：Hello World
来源：http://cz.colortex.cn

print("Hello")
来源：http://lu.panjiajie.cn

[T32] Lua：局部变量
来源：http://mh.huixinmuqiang.cn

local a = 1
来源：http://ox.nicolike.cn

[T33] Lua：表（数组）
来源：http://gf.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ii.haigaiapp.cn

[T34] Lua：遍历表
来源：http://fz.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ub.521024.cn

[T35] Lua：字典表
来源：http://ko.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://fd.huixinmuqiang.cn

[T36] Lua：函数
来源：http://vc.huanxung.cn

function add(a, b) return a + b end
来源：http://mk.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://vz.lnxyls.cn

"a" .. "b"
来源：http://gb.hahajie.cn

[T38] Lua：条件
来源：http://uf.lnxyls.cn

if x > 0 then print("正") end
来源：http://mk.asd995.cn

[T39] Lua：模式匹配
来源：http://kg.huixiangedu.cn

string.find(s, "%d+")
来源：http://rb.hnjuh.cn

[T40] Lua：元表
来源：http://jp.hahajie.cn

setmetatable({}, { __index = base })
来源：http://ll.asd995.cn

[T41] Perl：Hello World
来源：http://vt.huixiangedu.cn

print "Hello\n";
来源：http://dv.szxytkj.cn

[T42] Perl：变量类型
来源：http://xb.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yl.newstarts.cn

[T43] Perl：字符串插值
来源：http://qv.huanxung.cn

"值: $a"
来源：http://wf.szxytkj.cn

[T44] Perl：条件
来源：http://wc.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://ry.szxytkj.cn

[T45] Perl：数组遍历
来源：http://zi.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://tk.nszjky.cn

[T46] Perl：哈希操作
来源：http://yv.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://en.hahajie.cn

[T47] Perl：正则捕获
来源：http://qk.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yg.nszjky.cn

[T48] Perl：正则替换
来源：http://un.asd995.cn

$s =~ s/old/new/g;
来源：http://sp.yuntaijiaju.cn

[T49] Perl：函数
来源：http://is.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sp.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://dl.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://md.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://rs.521024.cn

[T51] Scala：Hello World
来源：http://vf.shxzukj.cn

println("Hello")
来源：http://sg.hahajie.cn

[T52] Scala：变量
来源：http://pa.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://hy.gzmigu.cn

[T53] Scala：字符串插值
来源：http://wr.yuntaijiaju.cn

s"值: $b"
来源：http://zt.newstarts.cn

[T54] Scala：集合映射
来源：http://mi.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://qo.szxytkj.cn

[T55] Scala：集合过滤
来源：http://hq.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ha.asd995.cn

[T56] Scala：样例类
来源：http://qt.shxzukj.cn

case class User(name: String, age: Int)
来源：http://uc.9csxet.cn

[T57] Scala：模式匹配
来源：http://ry.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qd.newstarts.cn

[T58] Scala：函数定义
来源：http://vn.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mf.haigaiapp.cn

[T59] Scala：循环
来源：http://ni.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://ic.hahajie.cn

[T60] Scala：折叠
来源：http://yu.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cf.9csxet.cn

================================================================================
来源：http://tl.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sd.szsharing.cn

================================================================================
来源：http://ow.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://nu.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pu.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://bf.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dm.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://lu.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wz.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://od.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zt.hahajie.cn

[U05] Py：列表去重且保序
来源：http://qx.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://hr.shxzskj.cn

[U06] Py：合并两个字典
来源：http://mj.huixinmuqiang.cn

{**a, **b}
来源：http://kb.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://gj.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://rq.colortex.cn

[U08] Py：展平二维列表
来源：http://cj.newstarts.cn

[y for x in nested for y in x]
来源：http://tj.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://gs.shtwfgs.cn

max(d, key=d.get)
来源：http://wr.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://fj.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sw.panjiajie.cn

[U11] Py：生成器表达式
来源：http://xs.jctech888.com.cn

(x * 2 for x in arr)
来源：http://rr.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lb.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://ov.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://yv.wgjwhj.cn

deque(maxlen=10)
来源：http://jc.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://vs.huanxung.cn

defaultdict(list)
来源：http://of.jctech888.com.cn

[U15] Py：高精度计时
来源：http://pa.newstarts.cn

t = time.perf_counter()
来源：http://uj.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://pn.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kt.yuexingan06.cn

[U17] Py：初始化日志
来源：http://kw.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://mp.bjjhwx.cn

[U18] Py：预编译正则
来源：http://dl.colortex.cn

pat = re.compile(r"\d+")
来源：http://ry.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://ch.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://up.9csxet.cn

[U20] Py：缓存函数结果
来源：http://vy.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://vh.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://wf.asd995.cn

@contextlib.contextmanager
来源：http://pv.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://kg.huixinmuqiang.cn

list(zip(*m))
来源：http://yr.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://uc.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ds.szxytkj.cn

[U24] Py：路径操作
来源：http://gx.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fh.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://cv.bjjhwx.cn

csv.DictReader(f)
来源：http://zx.lnxyls.cn

[U26] Py：并发下载
来源：http://gf.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aq.colortex.cn

[U27] Py：异步 HTTP
来源：http://nh.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://nb.haigaiapp.cn

[U28] Py：类型别名
来源：http://as.jianghongdianzi.cn

UserId = int
来源：http://hy.521024.cn

[U29] Py：属性校验
来源：http://gl.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://it.9csxet.cn

[U30] Py：数据类
来源：http://wy.bjjhwx.cn

@dataclass(slots=True)
来源：http://gt.newstarts.cn

[U31] Py：单测
来源：http://kv.muxihuayi.cn

python -m pytest -q
来源：http://te.panjiajie.cn

[U32] Py：代码格式化
来源：http://qi.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://yq.colortex.cn

[U33] Py：打包发布
来源：http://ox.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://gu.szxytkj.cn

[U34] Py：判断编码
来源：http://gu.huixiangedu.cn

chardet.detect(raw)
来源：http://vs.haigaiapp.cn

[U35] Py：发送邮件
来源：http://dz.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mp.huanxung.cn

[U36] Py：定时任务
来源：http://vg.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://zz.hahajie.cn

[U37] Py：读写 Excel
来源：http://zf.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kq.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://ui.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://xc.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://ll.nicolike.cn

sys.stdout.isatty()
来源：http://qu.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://ez.hahajie.cn

print("err", file=sys.stderr)
来源：http://ra.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://at.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bn.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://fk.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ff.huanxung.cn

[U43] PHP：声明命名空间
来源：http://ud.szxytkj.cn

namespace App\Http;
来源：http://ys.huanxung.cn

[U44] PHP：开启严格类型
来源：http://lv.yuexingan06.cn

declare(strict_types=1);
来源：http://ye.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://xk.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yd.colortex.cn

[U46] PHP：可空类型
来源：http://td.asd995.cn

?string $name = null
来源：http://be.wgjwhj.cn

[U47] PHP：联合类型
来源：http://nf.chemitech.net.cn

int|string $id
来源：http://bi.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://iz.szsharing.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cp.panjiajie.cn

[U49] PHP：只读属性
来源：http://hm.shxzukj.cn

public readonly string $name
来源：http://it.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://fz.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://ow.hahajie.cn

[U51] PHP：数组解构
来源：http://zq.lnxyls.cn

[$a, $b] = $arr;
来源：http://gy.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://qr.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://vj.nszjky.cn


<!-- 参考信息 -->