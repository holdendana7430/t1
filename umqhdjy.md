代发 wailian999

static int counter = 0;
来源：http://la.9csxet.cn

[S29] C：变参函数
来源：http://cp.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://su.huixiangedu.cn

[S30] C：头文件保护
来源：http://bx.lnxyls.cn

#ifndef X_H
来源：http://un.bjjhwx.cn

#define X_H
来源：http://qq.nicolike.cn

#endif
来源：http://ed.wgjwhj.cn

[S31] C++：Hello World
来源：http://qd.huanxung.cn

#include <iostream>
来源：http://ow.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://am.521024.cn

[S32] C++：字符串
来源：http://gw.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://ew.chemitech.net.cn

[S33] C++：vector 增删
来源：http://nm.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gu.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://ry.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://tv.shxzukj.cn

[S35] C++：map
来源：http://fe.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uz.9csxet.cn

[S36] C++：unordered_map
来源：http://ew.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sj.yuntaijiaju.cn

[S37] C++：set
来源：http://ur.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tt.yuexingan06.cn

[S38] C++：排序
来源：http://dr.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://jp.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://fn.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ls.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://kq.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kw.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://vh.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vp.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://hf.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://qc.huanxung.cn

[S43] C++：智能指针
来源：http://rv.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://uk.szxytkj.cn

[S44] C++：引用传参
来源：http://qj.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://pe.nszjky.cn

[S45] C++：lambda
来源：http://wl.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://eg.szsharing.cn

[S46] C++：函数模板
来源：http://qr.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cn.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://tz.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ip.hnjuh.cn

[S48] C++：逐行读文件
来源：http://kw.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ww.521024.cn

while (std::getline(in, line)) { }
来源：http://im.9csxet.cn

[S49] C++：写文件
来源：http://ef.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uq.nicolike.cn

[S50] C++：格式化数字
来源：http://ty.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ig.newstarts.cn

[S51] C++：显式类型转换
来源：http://xo.shxzskj.cn

static_cast<double>(a) / b
来源：http://hb.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://kt.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://qv.huixiangedu.cn

[S53] C++：移动语义
来源：http://bk.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://dn.colortex.cn

[S54] C++：异常处理
来源：http://wd.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://it.9csxet.cn

[S55] C++：结构化绑定
来源：http://ox.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ao.newstarts.cn

[S56] C++：optional
来源：http://jf.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sj.9csxet.cn

[S57] C++：编译期常量
来源：http://ng.asd995.cn

constexpr int N = 10;
来源：http://mb.shtwfgs.cn

[S58] C++：命名空间
来源：http://dg.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://cr.muxihuayi.cn

[S59] C++：静态断言
来源：http://hr.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://to.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://sa.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vl.haigaiapp.cn

================================================================================
来源：http://ta.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rv.huixiangedu.cn

================================================================================
来源：http://cl.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://ul.szsharing.cn

println("Hello")
来源：http://zx.jctech888.com.cn

[T02] Kotlin：变量
来源：http://qg.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qz.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://rm.haigaiapp.cn

"值: $b"
来源：http://ss.asd995.cn

[T04] Kotlin：空安全
来源：http://sr.nszjky.cn

val n: String? = null;  n?.length
来源：http://pf.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://re.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ey.huanxung.cn

[T06] Kotlin：集合映射
来源：http://yl.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://go.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://wp.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gz.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://ie.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://ai.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://jj.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://li.9csxet.cn

[T10] Kotlin：默认参数
来源：http://yp.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kv.bjjhwx.cn

[T11] Kotlin：协程
来源：http://oq.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qx.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://tx.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://je.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://el.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://qi.haigaiapp.cn

[T14] Kotlin：循环
来源：http://qi.szxytkj.cn

for (i in 1..10) println(i)
来源：http://wt.panjiajie.cn

[T15] Kotlin：接口
来源：http://yo.asd995.cn

interface Shape { fun area(): Double }
来源：http://wi.hnjuh.cn

[T16] Swift：Hello World
来源：http://zr.hahajie.cn

print("Hello")
来源：http://hn.szxytkj.cn

[T17] Swift：变量与常量
来源：http://qv.shxzukj.cn

var a = 1;  let b = 2
来源：http://sh.asd995.cn

[T18] Swift：字符串插值
来源：http://wm.shtwfgs.cn

"值: \(b)"
来源：http://fg.gzmigu.cn

[T19] Swift：可选绑定
来源：http://zc.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://ec.9csxet.cn

[T20] Swift：数组操作
来源：http://wh.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bw.huixiangedu.cn

[T21] Swift：遍历
来源：http://pi.yuexingan06.cn

for x in a { print(x) }
来源：http://gh.newstarts.cn

[T22] Swift：字典
来源：http://dh.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tk.yuntaijiaju.cn

[T23] Swift：函数
来源：http://hx.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ln.shxzskj.cn

[T24] Swift：闭包
来源：http://my.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nz.lnxyls.cn

[T25] Swift：结构体
来源：http://md.shxzukj.cn

struct P { var x: Int }
来源：http://ic.asd995.cn

[T26] Swift：类与重写
来源：http://ia.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://wo.szxytkj.cn

[T27] Swift：错误处理
来源：http://pb.9csxet.cn

do { try f() } catch { print(error) }
来源：http://on.shxzskj.cn

[T28] Swift：枚举
来源：http://ax.asd995.cn

enum Color { case red, green }
来源：http://im.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://tj.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://uh.muxihuayi.cn

[T30] Swift：协议
来源：http://gl.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://fr.nicolike.cn

[T31] Lua：Hello World
来源：http://ef.colortex.cn

print("Hello")
来源：http://ri.yuexingan06.cn

[T32] Lua：局部变量
来源：http://eb.hnjuh.cn

local a = 1
来源：http://yt.panjiajie.cn

[T33] Lua：表（数组）
来源：http://ob.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hv.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://yh.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wd.newstarts.cn

[T35] Lua：字典表
来源：http://hq.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://pv.szsharing.cn

[T36] Lua：函数
来源：http://fz.shxzukj.cn

function add(a, b) return a + b end
来源：http://ld.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://ft.huanxung.cn

"a" .. "b"
来源：http://pb.lnxyls.cn

[T38] Lua：条件
来源：http://jj.bjjhwx.cn

if x > 0 then print("正") end
来源：http://nm.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://gc.szxytkj.cn

string.find(s, "%d+")
来源：http://lb.szxytkj.cn

[T40] Lua：元表
来源：http://mx.asd995.cn

setmetatable({}, { __index = base })
来源：http://fj.chemitech.net.cn

[T41] Perl：Hello World
来源：http://ui.newstarts.cn

print "Hello\n";
来源：http://ml.huixiangedu.cn

[T42] Perl：变量类型
来源：http://dp.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ql.colortex.cn

[T43] Perl：字符串插值
来源：http://io.shxzukj.cn

"值: $a"
来源：http://qx.nszjky.cn

[T44] Perl：条件
来源：http://xo.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://mz.hahajie.cn

[T45] Perl：数组遍历
来源：http://kp.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://yw.szsharing.cn

[T46] Perl：哈希操作
来源：http://az.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zn.hnjuh.cn

[T47] Perl：正则捕获
来源：http://cu.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://no.newstarts.cn

[T48] Perl：正则替换
来源：http://xq.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://zi.hnjuh.cn

[T49] Perl：函数
来源：http://kr.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nj.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://ow.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ae.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://ss.lnxyls.cn

[T51] Scala：Hello World
来源：http://dt.asd995.cn

println("Hello")
来源：http://ov.shtwfgs.cn

[T52] Scala：变量
来源：http://xw.shxzskj.cn

val a = 1;  var b = 2
来源：http://oq.lnxyls.cn

[T53] Scala：字符串插值
来源：http://at.jctech888.com.cn

s"值: $b"
来源：http://zk.shtwfgs.cn

[T54] Scala：集合映射
来源：http://ga.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://hd.hahajie.cn

[T55] Scala：集合过滤
来源：http://ka.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tt.haigaiapp.cn

[T56] Scala：样例类
来源：http://bg.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://gq.nszjky.cn

[T57] Scala：模式匹配
来源：http://lt.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ua.lnxyls.cn

[T58] Scala：函数定义
来源：http://cf.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sk.nicolike.cn

[T59] Scala：循环
来源：http://kx.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://qe.panjiajie.cn

[T60] Scala：折叠
来源：http://tl.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xj.huixiangedu.cn

================================================================================
来源：http://na.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://al.huixiangedu.cn

================================================================================
来源：http://gz.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://ma.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kg.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://tv.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bf.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://bv.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iu.lnxyls.cn

[U04] Py：变量调试打印
来源：http://ss.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://be.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://zl.asd995.cn

list(dict.fromkeys(arr))
来源：http://el.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://fb.muxihuayi.cn

{**a, **b}
来源：http://yh.panjiajie.cn

[U07] Py：反转字典键值
来源：http://cc.asd995.cn

{v: k for k, v in d.items()}
来源：http://aw.szsharing.cn

[U08] Py：展平二维列表
来源：http://rz.hahajie.cn

[y for x in nested for y in x]
来源：http://xl.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://fl.panjiajie.cn

max(d, key=d.get)
来源：http://se.521024.cn

[U10] Py：按值排序字典
来源：http://vt.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rl.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://us.gzmigu.cn

(x * 2 for x in arr)
来源：http://pq.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ci.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://vz.9csxet.cn

[U13] Py：固定长度队列
来源：http://ok.shxzskj.cn

deque(maxlen=10)
来源：http://zr.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://xs.9csxet.cn

defaultdict(list)
来源：http://rw.szsharing.cn

[U15] Py：高精度计时
来源：http://wa.nszjky.cn

t = time.perf_counter()
来源：http://fo.hahajie.cn

[U16] Py：命令行参数解析
来源：http://xd.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oj.newstarts.cn

[U17] Py：初始化日志
来源：http://ud.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://ir.szsharing.cn

[U18] Py：预编译正则
来源：http://tf.huanxung.cn

pat = re.compile(r"\d+")
来源：http://rt.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://mu.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://me.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://yl.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://zu.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://ny.hahajie.cn

@contextlib.contextmanager
来源：http://uy.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://qe.haigaiapp.cn

list(zip(*m))
来源：http://px.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://kr.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://en.wgjwhj.cn

[U24] Py：路径操作
来源：http://hj.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tz.colortex.cn

[U25] Py：CSV 按字典读
来源：http://bi.szxytkj.cn

csv.DictReader(f)
来源：http://gq.asd995.cn

[U26] Py：并发下载
来源：http://ch.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ix.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://kd.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://en.shxzukj.cn

[U28] Py：类型别名
来源：http://np.huanxung.cn

UserId = int
来源：http://do.muxihuayi.cn

[U29] Py：属性校验
来源：http://sw.panjiajie.cn

@property 与 @x.setter 配合
来源：http://bu.jctech888.com.cn

[U30] Py：数据类
来源：http://qr.9csxet.cn

@dataclass(slots=True)
来源：http://qn.asd995.cn

[U31] Py：单测
来源：http://ln.newstarts.cn

python -m pytest -q
来源：http://pt.9csxet.cn

[U32] Py：代码格式化
来源：http://yj.colortex.cn

ruff format . && ruff check --fix .
来源：http://dp.jctech888.com.cn

[U33] Py：打包发布
来源：http://yb.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://ih.nicolike.cn

[U34] Py：判断编码
来源：http://qx.yuexingan06.cn

chardet.detect(raw)
来源：http://vi.gzmigu.cn

[U35] Py：发送邮件
来源：http://no.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wp.szsharing.cn

[U36] Py：定时任务
来源：http://sm.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://gh.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://zy.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gr.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://ht.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://ho.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://tn.bjjhwx.cn

sys.stdout.isatty()
来源：http://hc.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://he.huanxung.cn

print("err", file=sys.stderr)
来源：http://ky.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://rq.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qj.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://jo.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dq.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://mc.haigaiapp.cn

namespace App\Http;
来源：http://hw.nicolike.cn

[U44] PHP：开启严格类型
来源：http://xd.wgjwhj.cn

declare(strict_types=1);
来源：http://kd.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://fo.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oq.wgjwhj.cn

[U46] PHP：可空类型
来源：http://yb.asd995.cn

?string $name = null
来源：http://qh.hahajie.cn

[U47] PHP：联合类型
来源：http://gj.szxytkj.cn

int|string $id
来源：http://az.gzmigu.cn

[U48] PHP：纯枚举
来源：http://td.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wf.colortex.cn

[U49] PHP：只读属性
来源：http://kb.shtwfgs.cn

public readonly string $name
来源：http://ql.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://as.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://qz.haigaiapp.cn

[U51] PHP：数组解构
来源：http://zs.yuexingan06.cn

[$a, $b] = $arr;
来源：http://lo.hahajie.cn

[U52] PHP：箭头函数
来源：http://ti.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://og.9csxet.cn


<!-- 参考信息 -->