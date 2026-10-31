代发 wailian999

static int counter = 0;
来源：http://jy.szsharing.cn

[S29] C：变参函数
来源：http://im.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ga.asd995.cn

[S30] C：头文件保护
来源：http://ug.shxzskj.cn

#ifndef X_H
来源：http://io.huixinmuqiang.cn

#define X_H
来源：http://pk.yuexingan06.cn

#endif
来源：http://ua.9csxet.cn

[S31] C++：Hello World
来源：http://rg.jianghongdianzi.cn

#include <iostream>
来源：http://lq.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://fs.bookmarksfly.cn

[S32] C++：字符串
来源：http://ep.colortex.cn

std::string s = "hi";  s += "!";
来源：http://hw.colortex.cn

[S33] C++：vector 增删
来源：http://se.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ai.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://tm.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://xg.huixinmuqiang.cn

[S35] C++：map
来源：http://mh.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://da.huanxung.cn

[S36] C++：unordered_map
来源：http://ql.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fl.huixiangedu.cn

[S37] C++：set
来源：http://yq.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://to.hnjuh.cn

[S38] C++：排序
来源：http://hu.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://kq.asd995.cn

[S39] C++：自定义比较器排序
来源：http://xb.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ey.bookmarksfly.cn

[S40] C++：查找元素
来源：http://yz.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xc.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://kp.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cv.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://ym.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://zd.panjiajie.cn

[S43] C++：智能指针
来源：http://kq.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://zk.bookmarksfly.cn

[S44] C++：引用传参
来源：http://wm.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://jo.lnxyls.cn

[S45] C++：lambda
来源：http://ev.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kl.lnxyls.cn

[S46] C++：函数模板
来源：http://lm.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aw.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://eh.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sg.9csxet.cn

[S48] C++：逐行读文件
来源：http://um.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mo.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://ap.521024.cn

[S49] C++：写文件
来源：http://rb.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ld.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://ia.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oa.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://rv.lnxyls.cn

static_cast<double>(a) / b
来源：http://ry.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://vh.9csxet.cn

int size() const noexcept { return n_; }
来源：http://fu.haigaiapp.cn

[S53] C++：移动语义
来源：http://yo.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://lv.9csxet.cn

[S54] C++：异常处理
来源：http://wd.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mq.gzmigu.cn

[S55] C++：结构化绑定
来源：http://uh.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://np.9csxet.cn

[S56] C++：optional
来源：http://bj.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qg.huanxung.cn

[S57] C++：编译期常量
来源：http://sz.yuntaijiaju.cn

constexpr int N = 10;
来源：http://rl.lnxyls.cn

[S58] C++：命名空间
来源：http://pc.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://mh.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://cm.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qn.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://ur.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iy.gzmigu.cn

================================================================================
来源：http://ef.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bq.jctech888.com.cn

================================================================================
来源：http://gp.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://ow.shxzukj.cn

println("Hello")
来源：http://jx.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://cv.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oz.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://cb.shtwfgs.cn

"值: $b"
来源：http://hv.newstarts.cn

[T04] Kotlin：空安全
来源：http://fw.shxzskj.cn

val n: String? = null;  n?.length
来源：http://ka.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://wn.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://po.9csxet.cn

[T06] Kotlin：集合映射
来源：http://an.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ml.colortex.cn

[T07] Kotlin：集合过滤
来源：http://vn.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qp.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://va.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://bz.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://gr.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://mh.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://bn.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lk.muxihuayi.cn

[T11] Kotlin：协程
来源：http://jl.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yr.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://yx.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://zp.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://nc.newstarts.cn

val m = mapOf("a" to 1)
来源：http://dq.9csxet.cn

[T14] Kotlin：循环
来源：http://rn.hahajie.cn

for (i in 1..10) println(i)
来源：http://xv.wgjwhj.cn

[T15] Kotlin：接口
来源：http://ax.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://zk.521024.cn

[T16] Swift：Hello World
来源：http://dk.huixinmuqiang.cn

print("Hello")
来源：http://ox.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://bp.haigaiapp.cn

var a = 1;  let b = 2
来源：http://rt.hnjuh.cn

[T18] Swift：字符串插值
来源：http://sh.colortex.cn

"值: \(b)"
来源：http://nl.szsharing.cn

[T19] Swift：可选绑定
来源：http://ky.huixiangedu.cn

if let n = opt { print(n) }
来源：http://ei.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://cd.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tr.521024.cn

[T21] Swift：遍历
来源：http://ib.huixinmuqiang.cn

for x in a { print(x) }
来源：http://qu.bjjhwx.cn

[T22] Swift：字典
来源：http://io.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zc.newstarts.cn

[T23] Swift：函数
来源：http://dk.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sj.asd995.cn

[T24] Swift：闭包
来源：http://co.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xl.bookmarksfly.cn

[T25] Swift：结构体
来源：http://kl.shtwfgs.cn

struct P { var x: Int }
来源：http://sa.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://eh.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://re.haigaiapp.cn

[T27] Swift：错误处理
来源：http://nk.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://bx.nicolike.cn

[T28] Swift：枚举
来源：http://na.lnxyls.cn

enum Color { case red, green }
来源：http://sh.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://wf.jctech888.com.cn

guard let x = opt else { return }
来源：http://ji.lnxyls.cn

[T30] Swift：协议
来源：http://gb.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://ku.asd995.cn

[T31] Lua：Hello World
来源：http://qx.yuntaijiaju.cn

print("Hello")
来源：http://qu.shtwfgs.cn

[T32] Lua：局部变量
来源：http://ai.hnjuh.cn

local a = 1
来源：http://qj.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://qe.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yp.hnjuh.cn

[T34] Lua：遍历表
来源：http://hq.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gs.colortex.cn

[T35] Lua：字典表
来源：http://my.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://jr.muxihuayi.cn

[T36] Lua：函数
来源：http://nc.szxytkj.cn

function add(a, b) return a + b end
来源：http://kz.colortex.cn

[T37] Lua：字符串拼接
来源：http://gv.jianghongdianzi.cn

"a" .. "b"
来源：http://pb.yuntaijiaju.cn

[T38] Lua：条件
来源：http://ld.bjjhwx.cn

if x > 0 then print("正") end
来源：http://gd.szsharing.cn

[T39] Lua：模式匹配
来源：http://es.gzmigu.cn

string.find(s, "%d+")
来源：http://pv.lnxyls.cn

[T40] Lua：元表
来源：http://og.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://af.haigaiapp.cn

[T41] Perl：Hello World
来源：http://gr.hnjuh.cn

print "Hello\n";
来源：http://nc.haigaiapp.cn

[T42] Perl：变量类型
来源：http://af.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ag.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://at.lnxyls.cn

"值: $a"
来源：http://og.bjjhwx.cn

[T44] Perl：条件
来源：http://od.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://qz.521024.cn

[T45] Perl：数组遍历
来源：http://tm.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://ea.asd995.cn

[T46] Perl：哈希操作
来源：http://lu.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kx.9csxet.cn

[T47] Perl：正则捕获
来源：http://ra.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bo.huixinmuqiang.cn

[T48] Perl：正则替换
来源：http://sx.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://lv.jctech888.com.cn

[T49] Perl：函数
来源：http://tr.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ts.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://sk.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fg.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://kh.colortex.cn

[T51] Scala：Hello World
来源：http://ex.shtwfgs.cn

println("Hello")
来源：http://ex.nszjky.cn

[T52] Scala：变量
来源：http://ib.wgjwhj.cn

val a = 1;  var b = 2
来源：http://rl.panjiajie.cn

[T53] Scala：字符串插值
来源：http://as.panjiajie.cn

s"值: $b"
来源：http://bn.panjiajie.cn

[T54] Scala：集合映射
来源：http://pz.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://ku.gzmigu.cn

[T55] Scala：集合过滤
来源：http://kz.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uy.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://tz.hnjuh.cn

case class User(name: String, age: Int)
来源：http://hn.szxytkj.cn

[T57] Scala：模式匹配
来源：http://ri.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mv.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://hk.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hy.chemitech.net.cn

[T59] Scala：循环
来源：http://zo.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://wd.jctech888.com.cn

[T60] Scala：折叠
来源：http://lj.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cq.haigaiapp.cn

================================================================================
来源：http://ux.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vm.shxzukj.cn

================================================================================
来源：http://hr.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://pa.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://aw.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://zk.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tr.521024.cn

[U03] Py：加载 .env 配置
来源：http://lv.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://he.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://ok.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ip.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://yn.hnjuh.cn

list(dict.fromkeys(arr))
来源：http://ga.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://ht.shtwfgs.cn

{**a, **b}
来源：http://wd.colortex.cn

[U07] Py：反转字典键值
来源：http://pa.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://ob.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://qr.huixiangedu.cn

[y for x in nested for y in x]
来源：http://wn.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://kt.chemitech.net.cn

max(d, key=d.get)
来源：http://dq.newstarts.cn

[U10] Py：按值排序字典
来源：http://zj.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yd.asd995.cn

[U11] Py：生成器表达式
来源：http://yc.shtwfgs.cn

(x * 2 for x in arr)
来源：http://ri.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nr.szsharing.cn

Counter(arr).most_common(3)
来源：http://ey.nszjky.cn

[U13] Py：固定长度队列
来源：http://el.szxytkj.cn

deque(maxlen=10)
来源：http://vc.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://la.szsharing.cn

defaultdict(list)
来源：http://hx.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://zo.muxihuayi.cn

t = time.perf_counter()
来源：http://ic.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://za.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cm.huanxung.cn

[U17] Py：初始化日志
来源：http://jf.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://xv.muxihuayi.cn

[U18] Py：预编译正则
来源：http://ph.asd995.cn

pat = re.compile(r"\d+")
来源：http://co.nszjky.cn

[U19] Py：正则替换带回调
来源：http://fe.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ew.colortex.cn

[U20] Py：缓存函数结果
来源：http://ck.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://pg.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://lh.bookmarksfly.cn

@contextlib.contextmanager
来源：http://dl.shxzskj.cn

[U22] Py：矩阵转置
来源：http://zj.haigaiapp.cn

list(zip(*m))
来源：http://py.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://xb.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bp.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://sr.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gp.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://ld.lnxyls.cn

csv.DictReader(f)
来源：http://yw.huixiangedu.cn

[U26] Py：并发下载
来源：http://zm.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://px.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://nc.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://rj.wgjwhj.cn

[U28] Py：类型别名
来源：http://qs.huixinmuqiang.cn

UserId = int
来源：http://qp.szxytkj.cn

[U29] Py：属性校验
来源：http://nk.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://bn.asd995.cn

[U30] Py：数据类
来源：http://sl.9csxet.cn

@dataclass(slots=True)
来源：http://dg.yuntaijiaju.cn

[U31] Py：单测
来源：http://ve.asd995.cn

python -m pytest -q
来源：http://ef.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://wm.nicolike.cn

ruff format . && ruff check --fix .
来源：http://qg.gzmigu.cn

[U33] Py：打包发布
来源：http://cv.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://av.gzmigu.cn

[U34] Py：判断编码
来源：http://fl.asd995.cn

chardet.detect(raw)
来源：http://pz.szsharing.cn

[U35] Py：发送邮件
来源：http://kj.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fb.shxzskj.cn

[U36] Py：定时任务
来源：http://au.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://nb.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://gv.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ay.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://yj.gzmigu.cn

Path(__file__).resolve().parent
来源：http://xv.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://qb.haigaiapp.cn

sys.stdout.isatty()
来源：http://ao.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://ya.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://ai.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://af.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xl.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://yn.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ub.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://fo.huixinmuqiang.cn

namespace App\Http;
来源：http://ib.huanxung.cn

[U44] PHP：开启严格类型
来源：http://mi.haigaiapp.cn

declare(strict_types=1);
来源：http://ka.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://hm.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fz.panjiajie.cn

[U46] PHP：可空类型
来源：http://cn.9csxet.cn

?string $name = null
来源：http://uq.bjjhwx.cn

[U47] PHP：联合类型
来源：http://ok.colortex.cn

int|string $id
来源：http://cf.9csxet.cn

[U48] PHP：纯枚举
来源：http://vu.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hw.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://ed.wgjwhj.cn

public readonly string $name
来源：http://bp.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://tz.nszjky.cn

public function __construct(private int $id) {}
来源：http://nj.huixiangedu.cn

[U51] PHP：数组解构
来源：http://uv.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://mf.nicolike.cn

[U52] PHP：箭头函数
来源：http://rb.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://yr.hnjuh.cn


<!-- 参考信息 -->