代发 wailian999

#ifndef X_H
来源：http://jd.gzmigu.cn

#define X_H
来源：http://od.szsharing.cn

#endif
来源：http://xi.bookmarksfly.cn

[S31] C++：Hello World
来源：http://ta.jianghongdianzi.cn

#include <iostream>
来源：http://cx.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://wv.asd995.cn

[S32] C++：字符串
来源：http://pv.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://hi.shtwfgs.cn

[S33] C++：vector 增删
来源：http://qa.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pv.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://dn.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://ft.hnjuh.cn

[S35] C++：map
来源：http://ul.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qj.nszjky.cn

[S36] C++：unordered_map
来源：http://dn.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jt.bjjhwx.cn

[S37] C++：set
来源：http://vy.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ya.bookmarksfly.cn

[S38] C++：排序
来源：http://na.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://uw.521024.cn

[S39] C++：自定义比较器排序
来源：http://wz.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ta.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://go.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zz.panjiajie.cn

[S41] C++：类与构造函数
来源：http://vu.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ln.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://xa.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://mf.huixiangedu.cn

[S43] C++：智能指针
来源：http://rx.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://tb.gzmigu.cn

[S44] C++：引用传参
来源：http://nu.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://pp.bookmarksfly.cn

[S45] C++：lambda
来源：http://bq.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mx.nicolike.cn

[S46] C++：函数模板
来源：http://zl.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ft.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://sw.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hk.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://gq.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pj.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://sz.huixinmuqiang.cn

[S49] C++：写文件
来源：http://lo.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hh.newstarts.cn

[S50] C++：格式化数字
来源：http://ua.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hx.shxzukj.cn

[S51] C++：显式类型转换
来源：http://he.panjiajie.cn

static_cast<double>(a) / b
来源：http://to.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://vg.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://by.panjiajie.cn

[S53] C++：移动语义
来源：http://px.colortex.cn

std::vector<int> w = std::move(v);
来源：http://qs.huanxung.cn

[S54] C++：异常处理
来源：http://iv.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hg.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://up.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bi.9csxet.cn

[S56] C++：optional
来源：http://yt.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mb.newstarts.cn

[S57] C++：编译期常量
来源：http://yn.huanxung.cn

constexpr int N = 10;
来源：http://jh.hnjuh.cn

[S58] C++：命名空间
来源：http://rp.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://ci.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://je.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lv.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://tq.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vn.huixiangedu.cn

================================================================================
来源：http://so.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://br.muxihuayi.cn

================================================================================
来源：http://vc.asd995.cn

[T01] Kotlin：Hello World
来源：http://be.huanxung.cn

println("Hello")
来源：http://mb.huixiangedu.cn

[T02] Kotlin：变量
来源：http://ot.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tm.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://yw.jctech888.com.cn

"值: $b"
来源：http://ku.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://is.newstarts.cn

val n: String? = null;  n?.length
来源：http://mv.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://dv.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qs.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://zg.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dl.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://vk.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nx.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://dw.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://ch.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://bb.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://pg.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://hf.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hx.hahajie.cn

[T11] Kotlin：协程
来源：http://la.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qa.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://ua.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://fg.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://ho.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://qf.muxihuayi.cn

[T14] Kotlin：循环
来源：http://ce.panjiajie.cn

for (i in 1..10) println(i)
来源：http://yj.9csxet.cn

[T15] Kotlin：接口
来源：http://lu.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://jd.huixiangedu.cn

[T16] Swift：Hello World
来源：http://zl.szsharing.cn

print("Hello")
来源：http://gq.shxzskj.cn

[T17] Swift：变量与常量
来源：http://jn.hahajie.cn

var a = 1;  let b = 2
来源：http://jx.gzmigu.cn

[T18] Swift：字符串插值
来源：http://nb.muxihuayi.cn

"值: \(b)"
来源：http://jq.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://ql.shxzskj.cn

if let n = opt { print(n) }
来源：http://to.asd995.cn

[T20] Swift：数组操作
来源：http://ao.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jq.shtwfgs.cn

[T21] Swift：遍历
来源：http://pr.huanxung.cn

for x in a { print(x) }
来源：http://fb.gzmigu.cn

[T22] Swift：字典
来源：http://mc.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ln.huixinmuqiang.cn

[T23] Swift：函数
来源：http://ki.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wb.shxzukj.cn

[T24] Swift：闭包
来源：http://fv.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wv.panjiajie.cn

[T25] Swift：结构体
来源：http://ht.yuntaijiaju.cn

struct P { var x: Int }
来源：http://mc.jctech888.com.cn

[T26] Swift：类与重写
来源：http://lc.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://aj.szxytkj.cn

[T27] Swift：错误处理
来源：http://bq.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://bu.shxzukj.cn

[T28] Swift：枚举
来源：http://ro.yuexingan06.cn

enum Color { case red, green }
来源：http://as.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://ph.jctech888.com.cn

guard let x = opt else { return }
来源：http://bt.yuntaijiaju.cn

[T30] Swift：协议
来源：http://fs.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://pf.nszjky.cn

[T31] Lua：Hello World
来源：http://ee.gzmigu.cn

print("Hello")
来源：http://zc.asd995.cn

[T32] Lua：局部变量
来源：http://js.shtwfgs.cn

local a = 1
来源：http://af.hahajie.cn

[T33] Lua：表（数组）
来源：http://cd.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cq.yuexingan06.cn

[T34] Lua：遍历表
来源：http://to.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yp.newstarts.cn

[T35] Lua：字典表
来源：http://oc.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://bq.shtwfgs.cn

[T36] Lua：函数
来源：http://qo.chemitech.net.cn

function add(a, b) return a + b end
来源：http://kh.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://sr.shxzukj.cn

"a" .. "b"
来源：http://xm.lnxyls.cn

[T38] Lua：条件
来源：http://ln.521024.cn

if x > 0 then print("正") end
来源：http://dz.nicolike.cn

[T39] Lua：模式匹配
来源：http://aa.9csxet.cn

string.find(s, "%d+")
来源：http://zq.huixiangedu.cn

[T40] Lua：元表
来源：http://pm.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://hh.bjjhwx.cn

[T41] Perl：Hello World
来源：http://qr.521024.cn

print "Hello\n";
来源：http://yb.szxytkj.cn

[T42] Perl：变量类型
来源：http://yh.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ya.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://uq.hnjuh.cn

"值: $a"
来源：http://jy.wgjwhj.cn

[T44] Perl：条件
来源：http://vd.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://bf.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://dj.colortex.cn

for my $x (@arr) { print $x; }
来源：http://cj.hahajie.cn

[T46] Perl：哈希操作
来源：http://ng.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hm.huanxung.cn

[T47] Perl：正则捕获
来源：http://ia.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qo.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://wb.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://wi.shtwfgs.cn

[T49] Perl：函数
来源：http://em.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lg.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://om.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rr.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://am.colortex.cn

[T51] Scala：Hello World
来源：http://ew.colortex.cn

println("Hello")
来源：http://ep.jianghongdianzi.cn

[T52] Scala：变量
来源：http://rj.huanxung.cn

val a = 1;  var b = 2
来源：http://ix.hnjuh.cn

[T53] Scala：字符串插值
来源：http://ws.shtwfgs.cn

s"值: $b"
来源：http://fs.szsharing.cn

[T54] Scala：集合映射
来源：http://jh.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://hn.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://kp.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ar.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://jg.lnxyls.cn

case class User(name: String, age: Int)
来源：http://vy.shxzukj.cn

[T57] Scala：模式匹配
来源：http://vt.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ix.shxzukj.cn

[T58] Scala：函数定义
来源：http://dz.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://an.nszjky.cn

[T59] Scala：循环
来源：http://ib.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://kx.newstarts.cn

[T60] Scala：折叠
来源：http://hm.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wm.shtwfgs.cn

================================================================================
来源：http://ol.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wo.huanxung.cn

================================================================================
来源：http://ds.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://bq.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ep.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://xv.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://br.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://oc.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ye.szsharing.cn

[U04] Py：变量调试打印
来源：http://op.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lp.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://hv.nicolike.cn

list(dict.fromkeys(arr))
来源：http://de.nszjky.cn

[U06] Py：合并两个字典
来源：http://uy.hahajie.cn

{**a, **b}
来源：http://jo.shxzskj.cn

[U07] Py：反转字典键值
来源：http://vu.asd995.cn

{v: k for k, v in d.items()}
来源：http://eo.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://ak.muxihuayi.cn

[y for x in nested for y in x]
来源：http://pe.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://xp.shxzskj.cn

max(d, key=d.get)
来源：http://ex.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://hs.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wr.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://rv.newstarts.cn

(x * 2 for x in arr)
来源：http://yn.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pb.szsharing.cn

Counter(arr).most_common(3)
来源：http://yd.gzmigu.cn

[U13] Py：固定长度队列
来源：http://rb.huixinmuqiang.cn

deque(maxlen=10)
来源：http://sw.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://qw.huixinmuqiang.cn

defaultdict(list)
来源：http://wc.gzmigu.cn

[U15] Py：高精度计时
来源：http://yj.szxytkj.cn

t = time.perf_counter()
来源：http://ow.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://sl.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kx.yuexingan06.cn

[U17] Py：初始化日志
来源：http://mf.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://xr.gzmigu.cn

[U18] Py：预编译正则
来源：http://nk.9csxet.cn

pat = re.compile(r"\d+")
来源：http://av.hahajie.cn

[U19] Py：正则替换带回调
来源：http://yr.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ho.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://ug.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://ml.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://us.jctech888.com.cn

@contextlib.contextmanager
来源：http://dx.hahajie.cn

[U22] Py：矩阵转置
来源：http://fq.yuntaijiaju.cn

list(zip(*m))
来源：http://vl.hahajie.cn

[U23] Py：分块读取大文件
来源：http://lk.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sx.gzmigu.cn

[U24] Py：路径操作
来源：http://hf.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hl.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://mr.jianghongdianzi.cn

csv.DictReader(f)
来源：http://lk.muxihuayi.cn

[U26] Py：并发下载
来源：http://gv.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bo.asd995.cn

[U27] Py：异步 HTTP
来源：http://bq.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://jm.shxzskj.cn

[U28] Py：类型别名
来源：http://dx.bjjhwx.cn

UserId = int
来源：http://os.shxzskj.cn

[U29] Py：属性校验
来源：http://xd.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://sg.nicolike.cn

[U30] Py：数据类
来源：http://xc.colortex.cn

@dataclass(slots=True)
来源：http://np.huixinmuqiang.cn

[U31] Py：单测
来源：http://ju.huixiangedu.cn

python -m pytest -q
来源：http://xb.szxytkj.cn

[U32] Py：代码格式化
来源：http://ip.szsharing.cn

ruff format . && ruff check --fix .
来源：http://gr.521024.cn

[U33] Py：打包发布
来源：http://ln.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://ah.nszjky.cn

[U34] Py：判断编码
来源：http://il.shxzskj.cn

chardet.detect(raw)
来源：http://vf.jctech888.com.cn

[U35] Py：发送邮件
来源：http://yj.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xh.jctech888.com.cn

[U36] Py：定时任务
来源：http://lp.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://gj.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://da.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cl.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://em.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://ks.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://ex.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://ub.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://lm.newstarts.cn

print("err", file=sys.stderr)
来源：http://xt.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://fm.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lw.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://jt.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hn.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://ys.huixinmuqiang.cn

namespace App\Http;
来源：http://kb.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://gt.hnjuh.cn

declare(strict_types=1);
来源：http://lr.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://lu.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xx.hnjuh.cn

[U46] PHP：可空类型
来源：http://vn.yuexingan06.cn

?string $name = null
来源：http://rz.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://cj.gzmigu.cn

int|string $id
来源：http://fz.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://pv.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://na.chemitech.net.cn

[U49] PHP：只读属性
来源：http://jy.9csxet.cn

public readonly string $name
来源：http://tf.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://hm.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://pd.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://ae.bjjhwx.cn

[$a, $b] = $arr;
来源：http://lr.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://dn.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://go.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://jp.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://wr.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://wv.bjjhwx.cn

$obj?->method()
来源：http://te.colortex.cn


<!-- 参考信息 -->