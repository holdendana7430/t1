代发 wailian999

#ifndef X_H
来源：http://gu.haigaiapp.cn

#define X_H
来源：http://xi.haigaiapp.cn

#endif
来源：http://gz.shxzukj.cn

[S31] C++：Hello World
来源：http://fk.newstarts.cn

#include <iostream>
来源：http://aa.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://xz.newstarts.cn

[S32] C++：字符串
来源：http://uv.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://hp.newstarts.cn

[S33] C++：vector 增删
来源：http://hf.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wf.huanxung.cn

[S34] C++：遍历 vector
来源：http://jo.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://qf.panjiajie.cn

[S35] C++：map
来源：http://kd.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cv.wgjwhj.cn

[S36] C++：unordered_map
来源：http://mm.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://im.muxihuayi.cn

[S37] C++：set
来源：http://pl.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iq.yuntaijiaju.cn

[S38] C++：排序
来源：http://mf.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://lz.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://id.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jy.shxzskj.cn

[S40] C++：查找元素
来源：http://tq.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ch.hnjuh.cn

[S41] C++：类与构造函数
来源：http://cu.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vr.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://pd.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://ha.yuexingan06.cn

[S43] C++：智能指针
来源：http://yf.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://rk.jctech888.com.cn

[S44] C++：引用传参
来源：http://xl.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://dz.nszjky.cn

[S45] C++：lambda
来源：http://sr.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://va.bjjhwx.cn

[S46] C++：函数模板
来源：http://ge.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zk.521024.cn

[S47] C++：结构化绑定遍历
来源：http://ds.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sp.gzmigu.cn

[S48] C++：逐行读文件
来源：http://fl.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fk.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://qk.huanxung.cn

[S49] C++：写文件
来源：http://rx.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qk.shtwfgs.cn

[S50] C++：格式化数字
来源：http://pm.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gh.szsharing.cn

[S51] C++：显式类型转换
来源：http://lo.bjjhwx.cn

static_cast<double>(a) / b
来源：http://ac.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://tl.asd995.cn

int size() const noexcept { return n_; }
来源：http://va.521024.cn

[S53] C++：移动语义
来源：http://gs.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://vo.521024.cn

[S54] C++：异常处理
来源：http://jj.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oi.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://ij.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mv.yuexingan06.cn

[S56] C++：optional
来源：http://if.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ep.haigaiapp.cn

[S57] C++：编译期常量
来源：http://pm.newstarts.cn

constexpr int N = 10;
来源：http://jl.521024.cn

[S58] C++：命名空间
来源：http://vk.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://qw.asd995.cn

[S59] C++：静态断言
来源：http://xm.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tz.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://aa.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bg.bjjhwx.cn

================================================================================
来源：http://xk.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nv.szsharing.cn

================================================================================
来源：http://sp.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://tz.haigaiapp.cn

println("Hello")
来源：http://hc.shxzukj.cn

[T02] Kotlin：变量
来源：http://kz.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ma.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://iv.9csxet.cn

"值: $b"
来源：http://jb.nicolike.cn

[T04] Kotlin：空安全
来源：http://pl.nszjky.cn

val n: String? = null;  n?.length
来源：http://co.colortex.cn

[T05] Kotlin：when 表达式
来源：http://mw.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gt.huanxung.cn

[T06] Kotlin：集合映射
来源：http://xp.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wt.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://re.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://np.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://it.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://sw.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://cn.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://km.colortex.cn

[T10] Kotlin：默认参数
来源：http://ei.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qd.huanxung.cn

[T11] Kotlin：协程
来源：http://xf.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dt.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://mf.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://au.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://tv.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://qh.colortex.cn

[T14] Kotlin：循环
来源：http://aq.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://bn.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://gu.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://iz.huixiangedu.cn

[T16] Swift：Hello World
来源：http://pl.shxzskj.cn

print("Hello")
来源：http://ao.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://go.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://ra.szsharing.cn

[T18] Swift：字符串插值
来源：http://mv.panjiajie.cn

"值: \(b)"
来源：http://zi.521024.cn

[T19] Swift：可选绑定
来源：http://xx.panjiajie.cn

if let n = opt { print(n) }
来源：http://io.szxytkj.cn

[T20] Swift：数组操作
来源：http://ta.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cx.lnxyls.cn

[T21] Swift：遍历
来源：http://jy.lnxyls.cn

for x in a { print(x) }
来源：http://cn.shxzukj.cn

[T22] Swift：字典
来源：http://wg.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ib.bookmarksfly.cn

[T23] Swift：函数
来源：http://dh.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dk.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://jm.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dm.shxzskj.cn

[T25] Swift：结构体
来源：http://ti.hnjuh.cn

struct P { var x: Int }
来源：http://ac.jctech888.com.cn

[T26] Swift：类与重写
来源：http://ok.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://es.huanxung.cn

[T27] Swift：错误处理
来源：http://ih.nszjky.cn

do { try f() } catch { print(error) }
来源：http://hj.nszjky.cn

[T28] Swift：枚举
来源：http://xr.jianghongdianzi.cn

enum Color { case red, green }
来源：http://dr.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://xc.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://yk.jctech888.com.cn

[T30] Swift：协议
来源：http://zq.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://nj.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://jq.lnxyls.cn

print("Hello")
来源：http://ol.nicolike.cn

[T32] Lua：局部变量
来源：http://ub.colortex.cn

local a = 1
来源：http://xi.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://dv.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ka.shxzskj.cn

[T34] Lua：遍历表
来源：http://dm.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ww.bookmarksfly.cn

[T35] Lua：字典表
来源：http://vz.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://tk.nicolike.cn

[T36] Lua：函数
来源：http://um.asd995.cn

function add(a, b) return a + b end
来源：http://yk.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://gc.panjiajie.cn

"a" .. "b"
来源：http://iu.521024.cn

[T38] Lua：条件
来源：http://na.shxzukj.cn

if x > 0 then print("正") end
来源：http://qy.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://rf.hahajie.cn

string.find(s, "%d+")
来源：http://zg.jianghongdianzi.cn

[T40] Lua：元表
来源：http://kv.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://aj.muxihuayi.cn

[T41] Perl：Hello World
来源：http://vb.panjiajie.cn

print "Hello\n";
来源：http://gs.asd995.cn

[T42] Perl：变量类型
来源：http://ec.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bo.gzmigu.cn

[T43] Perl：字符串插值
来源：http://yc.panjiajie.cn

"值: $a"
来源：http://yq.huixinmuqiang.cn

[T44] Perl：条件
来源：http://ro.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://xu.szxytkj.cn

[T45] Perl：数组遍历
来源：http://lq.asd995.cn

for my $x (@arr) { print $x; }
来源：http://ks.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://em.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zo.9csxet.cn

[T47] Perl：正则捕获
来源：http://lf.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yj.huanxung.cn

[T48] Perl：正则替换
来源：http://fc.colortex.cn

$s =~ s/old/new/g;
来源：http://ot.nicolike.cn

[T49] Perl：函数
来源：http://vr.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mt.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://vc.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sr.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://uq.newstarts.cn

[T51] Scala：Hello World
来源：http://eo.huixiangedu.cn

println("Hello")
来源：http://if.nicolike.cn

[T52] Scala：变量
来源：http://yx.shxzskj.cn

val a = 1;  var b = 2
来源：http://cq.nicolike.cn

[T53] Scala：字符串插值
来源：http://na.gzmigu.cn

s"值: $b"
来源：http://aq.huixiangedu.cn

[T54] Scala：集合映射
来源：http://gl.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://vy.shxzukj.cn

[T55] Scala：集合过滤
来源：http://au.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iv.huixiangedu.cn

[T56] Scala：样例类
来源：http://gm.gzmigu.cn

case class User(name: String, age: Int)
来源：http://dy.colortex.cn

[T57] Scala：模式匹配
来源：http://gh.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lv.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://lm.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cz.bookmarksfly.cn

[T59] Scala：循环
来源：http://km.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://tp.jctech888.com.cn

[T60] Scala：折叠
来源：http://di.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ua.huixinmuqiang.cn

================================================================================
来源：http://sg.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cv.shxzskj.cn

================================================================================
来源：http://lo.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://fl.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qs.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://wv.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jc.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://bw.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sj.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://js.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://km.colortex.cn

[U05] Py：列表去重且保序
来源：http://yq.hnjuh.cn

list(dict.fromkeys(arr))
来源：http://zk.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://hm.nicolike.cn

{**a, **b}
来源：http://yo.huanxung.cn

[U07] Py：反转字典键值
来源：http://ek.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://my.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://az.szsharing.cn

[y for x in nested for y in x]
来源：http://uh.asd995.cn

[U09] Py：字典取最大值的键
来源：http://jp.bjjhwx.cn

max(d, key=d.get)
来源：http://kt.lnxyls.cn

[U10] Py：按值排序字典
来源：http://sb.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jn.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://zp.colortex.cn

(x * 2 for x in arr)
来源：http://yp.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hm.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://cj.szsharing.cn

[U13] Py：固定长度队列
来源：http://wh.yuexingan06.cn

deque(maxlen=10)
来源：http://ch.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://ms.wgjwhj.cn

defaultdict(list)
来源：http://hl.wgjwhj.cn

[U15] Py：高精度计时
来源：http://do.wgjwhj.cn

t = time.perf_counter()
来源：http://zz.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://ft.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://np.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://ah.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://nq.muxihuayi.cn

[U18] Py：预编译正则
来源：http://vy.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://xc.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://wc.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ai.nszjky.cn

[U20] Py：缓存函数结果
来源：http://um.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://su.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://xf.chemitech.net.cn

@contextlib.contextmanager
来源：http://im.gzmigu.cn

[U22] Py：矩阵转置
来源：http://gs.gzmigu.cn

list(zip(*m))
来源：http://td.newstarts.cn

[U23] Py：分块读取大文件
来源：http://uu.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://le.nszjky.cn

[U24] Py：路径操作
来源：http://zv.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ft.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://zz.szxytkj.cn

csv.DictReader(f)
来源：http://ph.muxihuayi.cn

[U26] Py：并发下载
来源：http://qx.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ho.nicolike.cn

[U27] Py：异步 HTTP
来源：http://zq.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://hl.nszjky.cn

[U28] Py：类型别名
来源：http://xk.asd995.cn

UserId = int
来源：http://ce.bjjhwx.cn

[U29] Py：属性校验
来源：http://qi.shxzukj.cn

@property 与 @x.setter 配合
来源：http://cu.bjjhwx.cn

[U30] Py：数据类
来源：http://zw.bookmarksfly.cn

@dataclass(slots=True)
来源：http://qf.huixiangedu.cn

[U31] Py：单测
来源：http://hf.hahajie.cn

python -m pytest -q
来源：http://hk.yuexingan06.cn

[U32] Py：代码格式化
来源：http://dt.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://ly.bookmarksfly.cn

[U33] Py：打包发布
来源：http://fr.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://ix.huixiangedu.cn

[U34] Py：判断编码
来源：http://qy.asd995.cn

chardet.detect(raw)
来源：http://vc.huixiangedu.cn

[U35] Py：发送邮件
来源：http://gy.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aw.huanxung.cn

[U36] Py：定时任务
来源：http://iu.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://ey.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://cb.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ql.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://kl.hnjuh.cn

Path(__file__).resolve().parent
来源：http://dv.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://vh.521024.cn

sys.stdout.isatty()
来源：http://pn.newstarts.cn

[U40] Py：打印到标准错误
来源：http://bh.asd995.cn

print("err", file=sys.stderr)
来源：http://io.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://gn.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fx.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://si.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dc.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://tl.huixinmuqiang.cn

namespace App\Http;
来源：http://ea.521024.cn

[U44] PHP：开启严格类型
来源：http://tc.nszjky.cn

declare(strict_types=1);
来源：http://en.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://cq.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ex.521024.cn

[U46] PHP：可空类型
来源：http://gc.muxihuayi.cn

?string $name = null
来源：http://hf.haigaiapp.cn

[U47] PHP：联合类型
来源：http://ga.chemitech.net.cn

int|string $id
来源：http://uj.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://wn.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xn.chemitech.net.cn

[U49] PHP：只读属性
来源：http://wm.wgjwhj.cn

public readonly string $name
来源：http://rn.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://tx.gzmigu.cn

public function __construct(private int $id) {}
来源：http://nj.gzmigu.cn

[U51] PHP：数组解构
来源：http://hb.nicolike.cn

[$a, $b] = $arr;
来源：http://al.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://jw.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://md.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://dt.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://gv.colortex.cn

[U54] PHP：空安全调用
来源：http://mc.shxzukj.cn

$obj?->method()
来源：http://gg.jctech888.com.cn


<!-- 参考信息 -->