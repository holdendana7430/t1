代发 wailian999

#include <iostream>
来源：http://nw.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://wt.jianghongdianzi.cn

[S32] C++：字符串
来源：http://bq.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://no.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://rw.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nr.9csxet.cn

[S34] C++：遍历 vector
来源：http://vx.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://pk.panjiajie.cn

[S35] C++：map
来源：http://wd.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fs.hahajie.cn

[S36] C++：unordered_map
来源：http://sp.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sx.jianghongdianzi.cn

[S37] C++：set
来源：http://vs.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fi.shxzukj.cn

[S38] C++：排序
来源：http://fx.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://jg.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://bu.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zv.panjiajie.cn

[S40] C++：查找元素
来源：http://fu.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cd.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://bx.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xd.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://yi.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://be.newstarts.cn

[S43] C++：智能指针
来源：http://kf.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://zz.hahajie.cn

[S44] C++：引用传参
来源：http://pj.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://op.huixinmuqiang.cn

[S45] C++：lambda
来源：http://ho.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://be.colortex.cn

[S46] C++：函数模板
来源：http://le.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rl.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://jl.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xw.szxytkj.cn

[S48] C++：逐行读文件
来源：http://ka.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hm.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://wy.gzmigu.cn

[S49] C++：写文件
来源：http://lr.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.9csxet.cn

[S50] C++：格式化数字
来源：http://vy.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ju.hahajie.cn

[S51] C++：显式类型转换
来源：http://tb.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://lv.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://ef.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://qv.hahajie.cn

[S53] C++：移动语义
来源：http://jm.asd995.cn

std::vector<int> w = std::move(v);
来源：http://ci.shtwfgs.cn

[S54] C++：异常处理
来源：http://gf.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vb.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://ji.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ys.nicolike.cn

[S56] C++：optional
来源：http://bm.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://an.huixiangedu.cn

[S57] C++：编译期常量
来源：http://xp.chemitech.net.cn

constexpr int N = 10;
来源：http://gv.huixiangedu.cn

[S58] C++：命名空间
来源：http://pr.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://yp.asd995.cn

[S59] C++：静态断言
来源：http://az.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lx.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://gv.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dg.521024.cn

================================================================================
来源：http://cf.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sh.newstarts.cn

================================================================================
来源：http://vz.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://dt.shtwfgs.cn

println("Hello")
来源：http://mu.bjjhwx.cn

[T02] Kotlin：变量
来源：http://vd.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xc.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://am.bookmarksfly.cn

"值: $b"
来源：http://kr.newstarts.cn

[T04] Kotlin：空安全
来源：http://dv.nicolike.cn

val n: String? = null;  n?.length
来源：http://qp.521024.cn

[T05] Kotlin：when 表达式
来源：http://cq.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kd.nszjky.cn

[T06] Kotlin：集合映射
来源：http://fy.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ug.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://pk.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://te.shxzskj.cn

[T08] Kotlin：数据类
来源：http://pp.521024.cn

data class User(val name: String, val age: Int)
来源：http://gj.colortex.cn

[T09] Kotlin：扩展函数
来源：http://do.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://kd.nszjky.cn

[T10] Kotlin：默认参数
来源：http://xl.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qz.lnxyls.cn

[T11] Kotlin：协程
来源：http://kw.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wy.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://yz.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://ua.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://zz.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://xu.huixiangedu.cn

[T14] Kotlin：循环
来源：http://mh.panjiajie.cn

for (i in 1..10) println(i)
来源：http://oa.colortex.cn

[T15] Kotlin：接口
来源：http://my.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://tq.bjjhwx.cn

[T16] Swift：Hello World
来源：http://uo.bjjhwx.cn

print("Hello")
来源：http://oq.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://bu.hahajie.cn

var a = 1;  let b = 2
来源：http://rl.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://cq.hahajie.cn

"值: \(b)"
来源：http://yq.nicolike.cn

[T19] Swift：可选绑定
来源：http://rf.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://pc.huixiangedu.cn

[T20] Swift：数组操作
来源：http://sb.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nf.nszjky.cn

[T21] Swift：遍历
来源：http://rm.huixinmuqiang.cn

for x in a { print(x) }
来源：http://xx.bjjhwx.cn

[T22] Swift：字典
来源：http://mb.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zt.jctech888.com.cn

[T23] Swift：函数
来源：http://dq.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pn.shxzskj.cn

[T24] Swift：闭包
来源：http://ut.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uk.newstarts.cn

[T25] Swift：结构体
来源：http://nz.newstarts.cn

struct P { var x: Int }
来源：http://vw.newstarts.cn

[T26] Swift：类与重写
来源：http://gz.hahajie.cn

class A: Base { override func f() {} }
来源：http://mt.nicolike.cn

[T27] Swift：错误处理
来源：http://xf.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://ah.hnjuh.cn

[T28] Swift：枚举
来源：http://gp.wgjwhj.cn

enum Color { case red, green }
来源：http://ax.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://xv.shxzukj.cn

guard let x = opt else { return }
来源：http://vs.haigaiapp.cn

[T30] Swift：协议
来源：http://zk.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://hz.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://vw.wgjwhj.cn

print("Hello")
来源：http://cs.hahajie.cn

[T32] Lua：局部变量
来源：http://nx.asd995.cn

local a = 1
来源：http://pj.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://fn.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lf.hahajie.cn

[T34] Lua：遍历表
来源：http://ns.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ck.bookmarksfly.cn

[T35] Lua：字典表
来源：http://vg.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://dr.wgjwhj.cn

[T36] Lua：函数
来源：http://bh.9csxet.cn

function add(a, b) return a + b end
来源：http://ft.newstarts.cn

[T37] Lua：字符串拼接
来源：http://yg.huixinmuqiang.cn

"a" .. "b"
来源：http://ka.521024.cn

[T38] Lua：条件
来源：http://mf.hahajie.cn

if x > 0 then print("正") end
来源：http://qt.nicolike.cn

[T39] Lua：模式匹配
来源：http://cx.521024.cn

string.find(s, "%d+")
来源：http://zp.huixinmuqiang.cn

[T40] Lua：元表
来源：http://wz.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://qr.9csxet.cn

[T41] Perl：Hello World
来源：http://mm.9csxet.cn

print "Hello\n";
来源：http://wc.haigaiapp.cn

[T42] Perl：变量类型
来源：http://il.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xd.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://hg.shxzskj.cn

"值: $a"
来源：http://uo.521024.cn

[T44] Perl：条件
来源：http://dq.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://mb.shxzukj.cn

[T45] Perl：数组遍历
来源：http://vd.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://yp.nszjky.cn

[T46] Perl：哈希操作
来源：http://wp.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jd.szxytkj.cn

[T47] Perl：正则捕获
来源：http://hr.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://le.9csxet.cn

[T48] Perl：正则替换
来源：http://is.colortex.cn

$s =~ s/old/new/g;
来源：http://lv.yuntaijiaju.cn

[T49] Perl：函数
来源：http://xb.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gw.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://ol.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tj.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://hx.muxihuayi.cn

[T51] Scala：Hello World
来源：http://py.lnxyls.cn

println("Hello")
来源：http://eo.wgjwhj.cn

[T52] Scala：变量
来源：http://tf.9csxet.cn

val a = 1;  var b = 2
来源：http://hp.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://mq.muxihuayi.cn

s"值: $b"
来源：http://pd.newstarts.cn

[T54] Scala：集合映射
来源：http://ty.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://fw.lnxyls.cn

[T55] Scala：集合过滤
来源：http://gu.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sm.huanxung.cn

[T56] Scala：样例类
来源：http://pn.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://wc.panjiajie.cn

[T57] Scala：模式匹配
来源：http://kl.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wk.shxzskj.cn

[T58] Scala：函数定义
来源：http://qz.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ma.colortex.cn

[T59] Scala：循环
来源：http://lx.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://uw.panjiajie.cn

[T60] Scala：折叠
来源：http://yn.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gj.panjiajie.cn

================================================================================
来源：http://ep.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fg.jctech888.com.cn

================================================================================
来源：http://sr.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://ph.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ey.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://pu.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vj.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://ny.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ic.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://nv.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hx.szsharing.cn

[U05] Py：列表去重且保序
来源：http://fe.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://xq.asd995.cn

[U06] Py：合并两个字典
来源：http://xv.newstarts.cn

{**a, **b}
来源：http://sb.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://wc.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://ga.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://fr.panjiajie.cn

[y for x in nested for y in x]
来源：http://ri.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://yk.521024.cn

max(d, key=d.get)
来源：http://sv.nicolike.cn

[U10] Py：按值排序字典
来源：http://yg.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://de.newstarts.cn

[U11] Py：生成器表达式
来源：http://jj.newstarts.cn

(x * 2 for x in arr)
来源：http://mz.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kw.nicolike.cn

Counter(arr).most_common(3)
来源：http://rd.shxzukj.cn

[U13] Py：固定长度队列
来源：http://na.szsharing.cn

deque(maxlen=10)
来源：http://oe.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://ci.jctech888.com.cn

defaultdict(list)
来源：http://ft.shxzskj.cn

[U15] Py：高精度计时
来源：http://qj.newstarts.cn

t = time.perf_counter()
来源：http://wh.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://wj.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kf.shxzukj.cn

[U17] Py：初始化日志
来源：http://pm.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://ry.panjiajie.cn

[U18] Py：预编译正则
来源：http://zu.hahajie.cn

pat = re.compile(r"\d+")
来源：http://ge.newstarts.cn

[U19] Py：正则替换带回调
来源：http://ek.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://in.521024.cn

[U20] Py：缓存函数结果
来源：http://rl.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://qn.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://el.huixiangedu.cn

@contextlib.contextmanager
来源：http://dg.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://qa.jctech888.com.cn

list(zip(*m))
来源：http://oy.colortex.cn

[U23] Py：分块读取大文件
来源：http://ze.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ug.yuexingan06.cn

[U24] Py：路径操作
来源：http://qu.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://of.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://ex.hahajie.cn

csv.DictReader(f)
来源：http://uv.lnxyls.cn

[U26] Py：并发下载
来源：http://nx.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://la.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://xp.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://tm.wgjwhj.cn

[U28] Py：类型别名
来源：http://ls.nicolike.cn

UserId = int
来源：http://wu.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://kw.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://pp.shxzskj.cn

[U30] Py：数据类
来源：http://si.wgjwhj.cn

@dataclass(slots=True)
来源：http://au.szxytkj.cn

[U31] Py：单测
来源：http://an.wgjwhj.cn

python -m pytest -q
来源：http://xn.muxihuayi.cn

[U32] Py：代码格式化
来源：http://ge.nicolike.cn

ruff format . && ruff check --fix .
来源：http://gp.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://qd.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://ky.nszjky.cn

[U34] Py：判断编码
来源：http://eq.colortex.cn

chardet.detect(raw)
来源：http://zb.newstarts.cn

[U35] Py：发送邮件
来源：http://sq.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ls.colortex.cn

[U36] Py：定时任务
来源：http://hc.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://fy.nicolike.cn

[U37] Py：读写 Excel
来源：http://ek.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vk.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://ms.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://ms.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://uo.shxzukj.cn

sys.stdout.isatty()
来源：http://ce.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://zz.hnjuh.cn

print("err", file=sys.stderr)
来源：http://pc.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://bz.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lx.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://yq.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nn.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://if.huanxung.cn

namespace App\Http;
来源：http://wj.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://ia.bjjhwx.cn

declare(strict_types=1);
来源：http://ii.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://wf.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dh.hahajie.cn

[U46] PHP：可空类型
来源：http://fr.yuexingan06.cn

?string $name = null
来源：http://jw.yuexingan06.cn

[U47] PHP：联合类型
来源：http://xv.hnjuh.cn

int|string $id
来源：http://gh.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://jo.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ao.9csxet.cn

[U49] PHP：只读属性
来源：http://gu.jianghongdianzi.cn

public readonly string $name
来源：http://wk.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://gl.hnjuh.cn

public function __construct(private int $id) {}
来源：http://ng.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://yx.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://es.nicolike.cn

[U52] PHP：箭头函数
来源：http://lk.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://og.huanxung.cn

[U53] PHP：空合并运算符
来源：http://dn.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://nz.asd995.cn

[U54] PHP：空安全调用
来源：http://zl.colortex.cn

$obj?->method()
来源：http://mq.hnjuh.cn

[U55] PHP：match 表达式
来源：http://sj.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://te.hnjuh.cn

[U56] PHP：命名参数
来源：http://ro.bjjhwx.cn

f(a: 1, b: 2)
来源：http://dv.gzmigu.cn


<!-- 参考信息 -->