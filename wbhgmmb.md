代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mi.9csxet.cn

[S25] C：内存拷贝
来源：http://oj.hnjuh.cn

memcpy(dst, src, n);
来源：http://un.shxzukj.cn

[S26] C：内存清零
来源：http://fo.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://qx.colortex.cn

[S27] C：定义常量
来源：http://ak.huanxung.cn

const double PI = 3.14159;
来源：http://ws.haigaiapp.cn

[S28] C：静态变量
来源：http://ql.hnjuh.cn

static int counter = 0;
来源：http://eg.haigaiapp.cn

[S29] C：变参函数
来源：http://hc.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ib.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://tr.jctech888.com.cn

#ifndef X_H
来源：http://ed.huixiangedu.cn

#define X_H
来源：http://nt.colortex.cn

#endif
来源：http://av.shtwfgs.cn

[S31] C++：Hello World
来源：http://dx.lnxyls.cn

#include <iostream>
来源：http://kg.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://fi.nicolike.cn

[S32] C++：字符串
来源：http://by.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://br.lnxyls.cn

[S33] C++：vector 增删
来源：http://br.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://il.lnxyls.cn

[S34] C++：遍历 vector
来源：http://jm.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://fz.hnjuh.cn

[S35] C++：map
来源：http://yt.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vd.muxihuayi.cn

[S36] C++：unordered_map
来源：http://bg.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wv.521024.cn

[S37] C++：set
来源：http://vo.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sa.szxytkj.cn

[S38] C++：排序
来源：http://ak.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://hj.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://rs.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gv.huixiangedu.cn

[S40] C++：查找元素
来源：http://by.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zn.nicolike.cn

[S41] C++：类与构造函数
来源：http://iw.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aj.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://qz.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://jc.nicolike.cn

[S43] C++：智能指针
来源：http://ln.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://ss.shxzukj.cn

[S44] C++：引用传参
来源：http://jg.huanxung.cn

void inc(int &x) { ++x; }
来源：http://bh.jianghongdianzi.cn

[S45] C++：lambda
来源：http://qp.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tq.hnjuh.cn

[S46] C++：函数模板
来源：http://kt.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lu.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://dt.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qd.nicolike.cn

[S48] C++：逐行读文件
来源：http://pp.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wz.colortex.cn

while (std::getline(in, line)) { }
来源：http://ji.gzmigu.cn

[S49] C++：写文件
来源：http://fk.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oc.lnxyls.cn

[S50] C++：格式化数字
来源：http://tq.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ev.shxzskj.cn

[S51] C++：显式类型转换
来源：http://wy.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://ol.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://ra.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://ov.gzmigu.cn

[S53] C++：移动语义
来源：http://uw.colortex.cn

std::vector<int> w = std::move(v);
来源：http://yb.chemitech.net.cn

[S54] C++：异常处理
来源：http://qi.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cv.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://fh.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yt.nicolike.cn

[S56] C++：optional
来源：http://mr.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xk.colortex.cn

[S57] C++：编译期常量
来源：http://lh.colortex.cn

constexpr int N = 10;
来源：http://cf.jctech888.com.cn

[S58] C++：命名空间
来源：http://tz.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://pb.asd995.cn

[S59] C++：静态断言
来源：http://ug.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://be.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://pu.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ho.szxytkj.cn

================================================================================
来源：http://tu.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ul.gzmigu.cn

================================================================================
来源：http://yc.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://rs.bookmarksfly.cn

println("Hello")
来源：http://fi.hahajie.cn

[T02] Kotlin：变量
来源：http://ke.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ug.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://bv.shtwfgs.cn

"值: $b"
来源：http://tp.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://mm.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://od.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://uz.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kk.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://pm.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kj.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://kb.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lr.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://og.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://hs.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://eo.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://td.newstarts.cn

[T10] Kotlin：默认参数
来源：http://ox.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oa.wgjwhj.cn

[T11] Kotlin：协程
来源：http://wd.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gb.nszjky.cn

[T12] Kotlin：解构声明
来源：http://xu.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://vy.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://yz.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://mf.hahajie.cn

[T14] Kotlin：循环
来源：http://po.asd995.cn

for (i in 1..10) println(i)
来源：http://yk.lnxyls.cn

[T15] Kotlin：接口
来源：http://pr.newstarts.cn

interface Shape { fun area(): Double }
来源：http://uo.nszjky.cn

[T16] Swift：Hello World
来源：http://qb.colortex.cn

print("Hello")
来源：http://kf.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://yx.9csxet.cn

var a = 1;  let b = 2
来源：http://cd.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://eg.wgjwhj.cn

"值: \(b)"
来源：http://xh.szsharing.cn

[T19] Swift：可选绑定
来源：http://vh.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://oy.szxytkj.cn

[T20] Swift：数组操作
来源：http://re.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jc.bjjhwx.cn

[T21] Swift：遍历
来源：http://eq.wgjwhj.cn

for x in a { print(x) }
来源：http://ia.huanxung.cn

[T22] Swift：字典
来源：http://xc.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cf.jianghongdianzi.cn

[T23] Swift：函数
来源：http://dp.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ah.huixiangedu.cn

[T24] Swift：闭包
来源：http://ns.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mi.haigaiapp.cn

[T25] Swift：结构体
来源：http://ew.shxzukj.cn

struct P { var x: Int }
来源：http://wm.nszjky.cn

[T26] Swift：类与重写
来源：http://th.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://lr.shxzukj.cn

[T27] Swift：错误处理
来源：http://zz.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://xv.panjiajie.cn

[T28] Swift：枚举
来源：http://iv.yuexingan06.cn

enum Color { case red, green }
来源：http://ho.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://dd.nszjky.cn

guard let x = opt else { return }
来源：http://wq.muxihuayi.cn

[T30] Swift：协议
来源：http://tr.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://ns.521024.cn

[T31] Lua：Hello World
来源：http://zx.jianghongdianzi.cn

print("Hello")
来源：http://zw.nszjky.cn

[T32] Lua：局部变量
来源：http://em.asd995.cn

local a = 1
来源：http://sd.asd995.cn

[T33] Lua：表（数组）
来源：http://hg.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gu.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://yw.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lx.shxzskj.cn

[T35] Lua：字典表
来源：http://ze.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://yp.yuntaijiaju.cn

[T36] Lua：函数
来源：http://zk.chemitech.net.cn

function add(a, b) return a + b end
来源：http://om.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://ez.jctech888.com.cn

"a" .. "b"
来源：http://fr.panjiajie.cn

[T38] Lua：条件
来源：http://rw.szxytkj.cn

if x > 0 then print("正") end
来源：http://xz.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://lo.shxzskj.cn

string.find(s, "%d+")
来源：http://og.muxihuayi.cn

[T40] Lua：元表
来源：http://zt.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://ys.muxihuayi.cn

[T41] Perl：Hello World
来源：http://sa.nicolike.cn

print "Hello\n";
来源：http://op.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://ry.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ks.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://fg.yuexingan06.cn

"值: $a"
来源：http://wk.szxytkj.cn

[T44] Perl：条件
来源：http://om.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://ea.szxytkj.cn

[T45] Perl：数组遍历
来源：http://br.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://ki.nicolike.cn

[T46] Perl：哈希操作
来源：http://wg.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mg.nicolike.cn

[T47] Perl：正则捕获
来源：http://ze.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ee.szsharing.cn

[T48] Perl：正则替换
来源：http://xy.gzmigu.cn

$s =~ s/old/new/g;
来源：http://jn.szsharing.cn

[T49] Perl：函数
来源：http://nv.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ji.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://og.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vr.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://ag.shxzskj.cn

[T51] Scala：Hello World
来源：http://hi.szsharing.cn

println("Hello")
来源：http://fm.huanxung.cn

[T52] Scala：变量
来源：http://oy.huixiangedu.cn

val a = 1;  var b = 2
来源：http://da.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://gn.bjjhwx.cn

s"值: $b"
来源：http://mz.jctech888.com.cn

[T54] Scala：集合映射
来源：http://ae.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://rt.panjiajie.cn

[T55] Scala：集合过滤
来源：http://sl.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lj.wgjwhj.cn

[T56] Scala：样例类
来源：http://vj.nicolike.cn

case class User(name: String, age: Int)
来源：http://cl.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://ze.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gf.huanxung.cn

[T58] Scala：函数定义
来源：http://de.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lu.wgjwhj.cn

[T59] Scala：循环
来源：http://rc.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://lx.bookmarksfly.cn

[T60] Scala：折叠
来源：http://pp.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ak.lnxyls.cn

================================================================================
来源：http://vr.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://is.shtwfgs.cn

================================================================================
来源：http://bz.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://fj.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qh.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://vj.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ke.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://wd.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ac.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://tq.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ca.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://oh.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://wy.szsharing.cn

[U06] Py：合并两个字典
来源：http://pd.jianghongdianzi.cn

{**a, **b}
来源：http://uv.szxytkj.cn

[U07] Py：反转字典键值
来源：http://ob.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://rk.hahajie.cn

[U08] Py：展平二维列表
来源：http://ke.yuexingan06.cn

[y for x in nested for y in x]
来源：http://tf.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://ye.jctech888.com.cn

max(d, key=d.get)
来源：http://hk.newstarts.cn

[U10] Py：按值排序字典
来源：http://ut.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uy.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://wl.hnjuh.cn

(x * 2 for x in arr)
来源：http://ro.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oi.shxzukj.cn

Counter(arr).most_common(3)
来源：http://bo.panjiajie.cn

[U13] Py：固定长度队列
来源：http://kq.hahajie.cn

deque(maxlen=10)
来源：http://sl.hahajie.cn

[U14] Py：分组收集到列表
来源：http://tf.muxihuayi.cn

defaultdict(list)
来源：http://xa.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://fj.jianghongdianzi.cn

t = time.perf_counter()
来源：http://om.521024.cn

[U16] Py：命令行参数解析
来源：http://yi.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mq.nicolike.cn

[U17] Py：初始化日志
来源：http://as.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://xf.szxytkj.cn

[U18] Py：预编译正则
来源：http://cq.huanxung.cn

pat = re.compile(r"\d+")
来源：http://tn.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://pi.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kq.newstarts.cn

[U20] Py：缓存函数结果
来源：http://cr.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://ys.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://hv.bjjhwx.cn

@contextlib.contextmanager
来源：http://jx.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://sn.huanxung.cn

list(zip(*m))
来源：http://jh.asd995.cn

[U23] Py：分块读取大文件
来源：http://ta.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tl.521024.cn

[U24] Py：路径操作
来源：http://ux.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ct.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://fm.asd995.cn

csv.DictReader(f)
来源：http://it.asd995.cn

[U26] Py：并发下载
来源：http://jg.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lt.newstarts.cn

[U27] Py：异步 HTTP
来源：http://ic.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://qp.yuexingan06.cn

[U28] Py：类型别名
来源：http://tr.shxzskj.cn

UserId = int
来源：http://mk.yuexingan06.cn

[U29] Py：属性校验
来源：http://er.nicolike.cn

@property 与 @x.setter 配合
来源：http://ct.huixiangedu.cn

[U30] Py：数据类
来源：http://gc.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://cl.huixiangedu.cn

[U31] Py：单测
来源：http://oq.nszjky.cn

python -m pytest -q
来源：http://kt.nicolike.cn

[U32] Py：代码格式化
来源：http://wu.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://ry.chemitech.net.cn

[U33] Py：打包发布
来源：http://gu.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://kg.gzmigu.cn

[U34] Py：判断编码
来源：http://rs.muxihuayi.cn

chardet.detect(raw)
来源：http://ry.haigaiapp.cn

[U35] Py：发送邮件
来源：http://gd.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://co.nicolike.cn

[U36] Py：定时任务
来源：http://ux.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://bp.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://ad.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iw.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://vj.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://yk.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://fk.bookmarksfly.cn

sys.stdout.isatty()
来源：http://gp.nszjky.cn

[U40] Py：打印到标准错误
来源：http://th.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://vu.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://xh.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jm.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://yl.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jn.colortex.cn

[U43] PHP：声明命名空间
来源：http://ct.jianghongdianzi.cn

namespace App\Http;
来源：http://yv.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://hd.huanxung.cn

declare(strict_types=1);
来源：http://zj.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://by.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ix.shxzskj.cn

[U46] PHP：可空类型
来源：http://oq.521024.cn

?string $name = null
来源：http://nr.hnjuh.cn

[U47] PHP：联合类型
来源：http://ve.newstarts.cn

int|string $id
来源：http://ng.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://tz.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gj.shxzukj.cn


<!-- 参考信息 -->