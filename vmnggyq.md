代发 wailian999

static int counter = 0;
来源：http://jj.muxihuayi.cn

[S29] C：变参函数
来源：http://ez.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ob.huanxung.cn

[S30] C：头文件保护
来源：http://nk.wgjwhj.cn

#ifndef X_H
来源：http://ye.jctech888.com.cn

#define X_H
来源：http://ck.szsharing.cn

#endif
来源：http://ta.chemitech.net.cn

[S31] C++：Hello World
来源：http://uv.huixiangedu.cn

#include <iostream>
来源：http://xq.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://fs.szsharing.cn

[S32] C++：字符串
来源：http://de.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://if.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://pv.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ul.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://nm.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://ya.lnxyls.cn

[S35] C++：map
来源：http://pt.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wu.shxzskj.cn

[S36] C++：unordered_map
来源：http://wj.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yt.asd995.cn

[S37] C++：set
来源：http://hh.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://if.yuexingan06.cn

[S38] C++：排序
来源：http://lm.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://og.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://ql.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pb.huixiangedu.cn

[S40] C++：查找元素
来源：http://wi.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yo.shxzskj.cn

[S41] C++：类与构造函数
来源：http://rx.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mo.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://va.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://qt.shxzskj.cn

[S43] C++：智能指针
来源：http://qv.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://qw.wgjwhj.cn

[S44] C++：引用传参
来源：http://yc.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://bj.jctech888.com.cn

[S45] C++：lambda
来源：http://rb.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bs.huanxung.cn

[S46] C++：函数模板
来源：http://xq.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cb.521024.cn

[S47] C++：结构化绑定遍历
来源：http://sc.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ta.panjiajie.cn

[S48] C++：逐行读文件
来源：http://zx.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fj.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://dc.szxytkj.cn

[S49] C++：写文件
来源：http://wy.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qd.newstarts.cn

[S50] C++：格式化数字
来源：http://on.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://os.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://rf.9csxet.cn

static_cast<double>(a) / b
来源：http://bp.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://pf.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://hb.newstarts.cn

[S53] C++：移动语义
来源：http://cl.asd995.cn

std::vector<int> w = std::move(v);
来源：http://sv.wgjwhj.cn

[S54] C++：异常处理
来源：http://au.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://db.nszjky.cn

[S55] C++：结构化绑定
来源：http://vp.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sy.muxihuayi.cn

[S56] C++：optional
来源：http://vs.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bz.hnjuh.cn

[S57] C++：编译期常量
来源：http://bv.jctech888.com.cn

constexpr int N = 10;
来源：http://bm.shtwfgs.cn

[S58] C++：命名空间
来源：http://wk.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://tb.yuexingan06.cn

[S59] C++：静态断言
来源：http://be.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wy.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://bk.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hs.bookmarksfly.cn

================================================================================
来源：http://ln.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zx.colortex.cn

================================================================================
来源：http://ve.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://xk.jianghongdianzi.cn

println("Hello")
来源：http://yk.colortex.cn

[T02] Kotlin：变量
来源：http://rb.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://al.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://jx.bookmarksfly.cn

"值: $b"
来源：http://fy.nicolike.cn

[T04] Kotlin：空安全
来源：http://wo.shxzskj.cn

val n: String? = null;  n?.length
来源：http://nv.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://kk.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mk.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://tf.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pp.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://pn.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mm.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://eb.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://dy.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://sf.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://ar.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://re.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rr.shxzskj.cn

[T11] Kotlin：协程
来源：http://pl.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ya.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://rp.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://vk.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://sy.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://wo.shxzskj.cn

[T14] Kotlin：循环
来源：http://ua.panjiajie.cn

for (i in 1..10) println(i)
来源：http://bg.nszjky.cn

[T15] Kotlin：接口
来源：http://wd.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://vu.wgjwhj.cn

[T16] Swift：Hello World
来源：http://us.bjjhwx.cn

print("Hello")
来源：http://oh.colortex.cn

[T17] Swift：变量与常量
来源：http://no.huanxung.cn

var a = 1;  let b = 2
来源：http://ez.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://bg.yuntaijiaju.cn

"值: \(b)"
来源：http://az.asd995.cn

[T19] Swift：可选绑定
来源：http://dg.wgjwhj.cn

if let n = opt { print(n) }
来源：http://ir.bjjhwx.cn

[T20] Swift：数组操作
来源：http://jp.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cw.muxihuayi.cn

[T21] Swift：遍历
来源：http://vm.shxzukj.cn

for x in a { print(x) }
来源：http://jk.nszjky.cn

[T22] Swift：字典
来源：http://bp.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vv.panjiajie.cn

[T23] Swift：函数
来源：http://hn.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ni.hahajie.cn

[T24] Swift：闭包
来源：http://ty.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ll.panjiajie.cn

[T25] Swift：结构体
来源：http://rv.asd995.cn

struct P { var x: Int }
来源：http://ed.521024.cn

[T26] Swift：类与重写
来源：http://qg.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://yh.jctech888.com.cn

[T27] Swift：错误处理
来源：http://fq.9csxet.cn

do { try f() } catch { print(error) }
来源：http://hy.huixiangedu.cn

[T28] Swift：枚举
来源：http://af.hnjuh.cn

enum Color { case red, green }
来源：http://ei.521024.cn

[T29] Swift：guard 提前返回
来源：http://nm.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://gr.szxytkj.cn

[T30] Swift：协议
来源：http://cq.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://yc.colortex.cn

[T31] Lua：Hello World
来源：http://nw.chemitech.net.cn

print("Hello")
来源：http://au.bjjhwx.cn

[T32] Lua：局部变量
来源：http://rw.nicolike.cn

local a = 1
来源：http://cp.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://tq.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ty.haigaiapp.cn

[T34] Lua：遍历表
来源：http://nx.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://it.asd995.cn

[T35] Lua：字典表
来源：http://wz.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://cr.lnxyls.cn

[T36] Lua：函数
来源：http://vb.shxzukj.cn

function add(a, b) return a + b end
来源：http://bb.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://dt.521024.cn

"a" .. "b"
来源：http://pz.newstarts.cn

[T38] Lua：条件
来源：http://gp.hnjuh.cn

if x > 0 then print("正") end
来源：http://qd.nszjky.cn

[T39] Lua：模式匹配
来源：http://if.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://wq.lnxyls.cn

[T40] Lua：元表
来源：http://ez.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://kw.haigaiapp.cn

[T41] Perl：Hello World
来源：http://zd.panjiajie.cn

print "Hello\n";
来源：http://nx.muxihuayi.cn

[T42] Perl：变量类型
来源：http://nz.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://np.521024.cn

[T43] Perl：字符串插值
来源：http://wg.shxzskj.cn

"值: $a"
来源：http://ow.shxzukj.cn

[T44] Perl：条件
来源：http://kq.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://qy.521024.cn

[T45] Perl：数组遍历
来源：http://mh.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://nl.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://dp.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hr.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://zq.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ij.asd995.cn

[T48] Perl：正则替换
来源：http://je.colortex.cn

$s =~ s/old/new/g;
来源：http://tl.521024.cn

[T49] Perl：函数
来源：http://mg.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sd.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://ea.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sv.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://fh.shxzukj.cn

[T51] Scala：Hello World
来源：http://nk.bjjhwx.cn

println("Hello")
来源：http://mz.shtwfgs.cn

[T52] Scala：变量
来源：http://bd.9csxet.cn

val a = 1;  var b = 2
来源：http://bm.9csxet.cn

[T53] Scala：字符串插值
来源：http://gv.yuexingan06.cn

s"值: $b"
来源：http://zt.shxzskj.cn

[T54] Scala：集合映射
来源：http://li.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://nq.szsharing.cn

[T55] Scala：集合过滤
来源：http://cv.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gp.nszjky.cn

[T56] Scala：样例类
来源：http://ol.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://pc.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://qi.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ds.colortex.cn

[T58] Scala：函数定义
来源：http://pa.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ml.huixiangedu.cn

[T59] Scala：循环
来源：http://dd.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://qe.chemitech.net.cn

[T60] Scala：折叠
来源：http://ye.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tf.jianghongdianzi.cn

================================================================================
来源：http://vh.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xk.wgjwhj.cn

================================================================================
来源：http://qt.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://mu.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yz.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://zx.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yl.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://oh.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vt.panjiajie.cn

[U04] Py：变量调试打印
来源：http://ed.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fp.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://xo.nicolike.cn

list(dict.fromkeys(arr))
来源：http://kc.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://gu.yuexingan06.cn

{**a, **b}
来源：http://ii.asd995.cn

[U07] Py：反转字典键值
来源：http://nn.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://iz.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://dy.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://it.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://aj.huixiangedu.cn

max(d, key=d.get)
来源：http://ha.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://tx.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lf.asd995.cn

[U11] Py：生成器表达式
来源：http://gq.newstarts.cn

(x * 2 for x in arr)
来源：http://jy.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oj.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://rf.lnxyls.cn

[U13] Py：固定长度队列
来源：http://zs.asd995.cn

deque(maxlen=10)
来源：http://uw.9csxet.cn

[U14] Py：分组收集到列表
来源：http://fs.hahajie.cn

defaultdict(list)
来源：http://ys.9csxet.cn

[U15] Py：高精度计时
来源：http://hm.nszjky.cn

t = time.perf_counter()
来源：http://ut.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://vq.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ft.nicolike.cn

[U17] Py：初始化日志
来源：http://fd.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://ar.muxihuayi.cn

[U18] Py：预编译正则
来源：http://ak.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://vi.asd995.cn

[U19] Py：正则替换带回调
来源：http://vk.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vi.huanxung.cn

[U20] Py：缓存函数结果
来源：http://kf.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://af.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://ua.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://kj.shxzukj.cn

[U22] Py：矩阵转置
来源：http://im.shxzskj.cn

list(zip(*m))
来源：http://zm.newstarts.cn

[U23] Py：分块读取大文件
来源：http://sf.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://id.gzmigu.cn

[U24] Py：路径操作
来源：http://ku.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rq.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://iy.lnxyls.cn

csv.DictReader(f)
来源：http://co.nszjky.cn

[U26] Py：并发下载
来源：http://ky.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fe.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://yp.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://sn.haigaiapp.cn

[U28] Py：类型别名
来源：http://lv.yuntaijiaju.cn

UserId = int
来源：http://oo.haigaiapp.cn

[U29] Py：属性校验
来源：http://yl.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://pm.shtwfgs.cn

[U30] Py：数据类
来源：http://xw.wgjwhj.cn

@dataclass(slots=True)
来源：http://th.chemitech.net.cn

[U31] Py：单测
来源：http://ne.hnjuh.cn

python -m pytest -q
来源：http://mh.9csxet.cn

[U32] Py：代码格式化
来源：http://vi.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://cc.wgjwhj.cn

[U33] Py：打包发布
来源：http://yl.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://sg.newstarts.cn

[U34] Py：判断编码
来源：http://fv.lnxyls.cn

chardet.detect(raw)
来源：http://de.hnjuh.cn

[U35] Py：发送邮件
来源：http://ec.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yz.shxzukj.cn

[U36] Py：定时任务
来源：http://ts.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://uy.nicolike.cn

[U37] Py：读写 Excel
来源：http://uu.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ba.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://fy.shxzukj.cn

Path(__file__).resolve().parent
来源：http://kf.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://lk.lnxyls.cn

sys.stdout.isatty()
来源：http://vm.hahajie.cn

[U40] Py：打印到标准错误
来源：http://qj.szsharing.cn

print("err", file=sys.stderr)
来源：http://pb.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://eh.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wq.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://xx.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qg.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://go.huixiangedu.cn

namespace App\Http;
来源：http://bd.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://bl.chemitech.net.cn

declare(strict_types=1);
来源：http://ro.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://lv.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tb.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://zt.gzmigu.cn

?string $name = null
来源：http://wk.haigaiapp.cn

[U47] PHP：联合类型
来源：http://wy.shxzskj.cn

int|string $id
来源：http://tp.panjiajie.cn

[U48] PHP：纯枚举
来源：http://ho.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dg.muxihuayi.cn

[U49] PHP：只读属性
来源：http://zn.chemitech.net.cn

public readonly string $name
来源：http://bn.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://lt.szxytkj.cn

public function __construct(private int $id) {}
来源：http://yv.lnxyls.cn

[U51] PHP：数组解构
来源：http://vq.panjiajie.cn

[$a, $b] = $arr;
来源：http://tf.shxzskj.cn

[U52] PHP：箭头函数
来源：http://hx.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://pw.huixinmuqiang.cn


<!-- 参考信息 -->