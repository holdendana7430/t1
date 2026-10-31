代发 wailian999

[S33] C++：vector 增删
来源：http://dj.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://av.shxzskj.cn

[S34] C++：遍历 vector
来源：http://vk.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://ws.jctech888.com.cn

[S35] C++：map
来源：http://vb.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aj.szsharing.cn

[S36] C++：unordered_map
来源：http://en.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rb.szxytkj.cn

[S37] C++：set
来源：http://yt.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://di.hnjuh.cn

[S38] C++：排序
来源：http://yt.521024.cn

std::sort(v.begin(), v.end());
来源：http://et.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://pf.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yl.hnjuh.cn

[S40] C++：查找元素
来源：http://ve.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vj.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://jb.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wp.colortex.cn

[S42] C++：继承与虚函数
来源：http://ly.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://rt.hahajie.cn

[S43] C++：智能指针
来源：http://kj.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://qy.colortex.cn

[S44] C++：引用传参
来源：http://ut.nszjky.cn

void inc(int &x) { ++x; }
来源：http://zt.chemitech.net.cn

[S45] C++：lambda
来源：http://ed.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fl.chemitech.net.cn

[S46] C++：函数模板
来源：http://ab.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cu.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://qc.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iq.gzmigu.cn

[S48] C++：逐行读文件
来源：http://hj.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pv.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://od.haigaiapp.cn

[S49] C++：写文件
来源：http://tg.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qn.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://oj.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ac.shxzskj.cn

[S51] C++：显式类型转换
来源：http://oa.shxzukj.cn

static_cast<double>(a) / b
来源：http://jk.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://yx.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://km.bookmarksfly.cn

[S53] C++：移动语义
来源：http://nz.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://ws.colortex.cn

[S54] C++：异常处理
来源：http://um.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mi.szsharing.cn

[S55] C++：结构化绑定
来源：http://wt.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vj.yuexingan06.cn

[S56] C++：optional
来源：http://lp.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://za.asd995.cn

[S57] C++：编译期常量
来源：http://op.jianghongdianzi.cn

constexpr int N = 10;
来源：http://xh.hahajie.cn

[S58] C++：命名空间
来源：http://oz.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://mg.lnxyls.cn

[S59] C++：静态断言
来源：http://bq.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qe.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://mt.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bh.nszjky.cn

================================================================================
来源：http://co.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tj.bjjhwx.cn

================================================================================
来源：http://so.9csxet.cn

[T01] Kotlin：Hello World
来源：http://pf.haigaiapp.cn

println("Hello")
来源：http://ym.nicolike.cn

[T02] Kotlin：变量
来源：http://ua.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rf.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://fo.yuexingan06.cn

"值: $b"
来源：http://tw.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://lu.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://we.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://cc.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wr.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://nv.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dy.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://an.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pi.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://fw.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://zh.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://rs.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://lc.newstarts.cn

[T10] Kotlin：默认参数
来源：http://rz.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hx.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://qn.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bk.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://yl.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://ea.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://fd.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://kj.haigaiapp.cn

[T14] Kotlin：循环
来源：http://gs.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://eb.nszjky.cn

[T15] Kotlin：接口
来源：http://rl.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://nw.shxzskj.cn

[T16] Swift：Hello World
来源：http://pf.shxzukj.cn

print("Hello")
来源：http://tw.szxytkj.cn

[T17] Swift：变量与常量
来源：http://pu.shtwfgs.cn

var a = 1;  let b = 2
来源：http://yb.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://qx.jctech888.com.cn

"值: \(b)"
来源：http://nl.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://ct.huixiangedu.cn

if let n = opt { print(n) }
来源：http://rx.shxzukj.cn

[T20] Swift：数组操作
来源：http://ey.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xt.nszjky.cn

[T21] Swift：遍历
来源：http://us.yuexingan06.cn

for x in a { print(x) }
来源：http://qq.bjjhwx.cn

[T22] Swift：字典
来源：http://mm.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://my.hnjuh.cn

[T23] Swift：函数
来源：http://ph.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tm.chemitech.net.cn

[T24] Swift：闭包
来源：http://pe.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://eq.gzmigu.cn

[T25] Swift：结构体
来源：http://tw.9csxet.cn

struct P { var x: Int }
来源：http://cw.521024.cn

[T26] Swift：类与重写
来源：http://gp.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://fm.muxihuayi.cn

[T27] Swift：错误处理
来源：http://pt.521024.cn

do { try f() } catch { print(error) }
来源：http://zw.shxzukj.cn

[T28] Swift：枚举
来源：http://yy.521024.cn

enum Color { case red, green }
来源：http://ba.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://md.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://vu.yuexingan06.cn

[T30] Swift：协议
来源：http://ru.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://ws.huanxung.cn

[T31] Lua：Hello World
来源：http://bg.yuntaijiaju.cn

print("Hello")
来源：http://zj.nicolike.cn

[T32] Lua：局部变量
来源：http://kk.huixinmuqiang.cn

local a = 1
来源：http://jf.szxytkj.cn

[T33] Lua：表（数组）
来源：http://wg.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vq.yuexingan06.cn

[T34] Lua：遍历表
来源：http://lj.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://id.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://ni.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://kg.huixinmuqiang.cn

[T36] Lua：函数
来源：http://qz.shxzskj.cn

function add(a, b) return a + b end
来源：http://qn.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://iv.muxihuayi.cn

"a" .. "b"
来源：http://wt.yuexingan06.cn

[T38] Lua：条件
来源：http://av.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://np.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://rj.bookmarksfly.cn

string.find(s, "%d+")
来源：http://sr.panjiajie.cn

[T40] Lua：元表
来源：http://bd.521024.cn

setmetatable({}, { __index = base })
来源：http://ox.colortex.cn

[T41] Perl：Hello World
来源：http://iy.shtwfgs.cn

print "Hello\n";
来源：http://bm.nszjky.cn

[T42] Perl：变量类型
来源：http://mz.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rd.colortex.cn

[T43] Perl：字符串插值
来源：http://lp.bjjhwx.cn

"值: $a"
来源：http://vu.jianghongdianzi.cn

[T44] Perl：条件
来源：http://sm.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://wd.colortex.cn

[T45] Perl：数组遍历
来源：http://bz.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://dc.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://nw.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://en.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://kl.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sc.szxytkj.cn

[T48] Perl：正则替换
来源：http://mu.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://gu.panjiajie.cn

[T49] Perl：函数
来源：http://hg.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zg.nszjky.cn

[T50] Perl：逐行读文件
来源：http://ac.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://px.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://os.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://ti.shtwfgs.cn

println("Hello")
来源：http://kd.bookmarksfly.cn

[T52] Scala：变量
来源：http://mo.shtwfgs.cn

val a = 1;  var b = 2
来源：http://lf.gzmigu.cn

[T53] Scala：字符串插值
来源：http://tg.521024.cn

s"值: $b"
来源：http://sy.asd995.cn

[T54] Scala：集合映射
来源：http://xg.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://av.hahajie.cn

[T55] Scala：集合过滤
来源：http://uv.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ne.bjjhwx.cn

[T56] Scala：样例类
来源：http://mg.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://mu.szsharing.cn

[T57] Scala：模式匹配
来源：http://yw.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hw.shxzukj.cn

[T58] Scala：函数定义
来源：http://jm.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fp.jianghongdianzi.cn

[T59] Scala：循环
来源：http://jm.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://da.bjjhwx.cn

[T60] Scala：折叠
来源：http://lm.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mx.huixiangedu.cn

================================================================================
来源：http://yp.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ue.szsharing.cn

================================================================================
来源：http://fg.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://xs.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zq.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://xi.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hk.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://tf.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vg.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://xh.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ye.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://sl.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://lh.hnjuh.cn

[U06] Py：合并两个字典
来源：http://hg.wgjwhj.cn

{**a, **b}
来源：http://sw.huanxung.cn

[U07] Py：反转字典键值
来源：http://an.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://gd.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://fq.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://dm.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://qi.nszjky.cn

max(d, key=d.get)
来源：http://sm.szxytkj.cn

[U10] Py：按值排序字典
来源：http://po.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iy.9csxet.cn

[U11] Py：生成器表达式
来源：http://ns.hnjuh.cn

(x * 2 for x in arr)
来源：http://tt.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kq.gzmigu.cn

Counter(arr).most_common(3)
来源：http://zv.gzmigu.cn

[U13] Py：固定长度队列
来源：http://to.huanxung.cn

deque(maxlen=10)
来源：http://bl.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://es.9csxet.cn

defaultdict(list)
来源：http://rr.panjiajie.cn

[U15] Py：高精度计时
来源：http://xo.huanxung.cn

t = time.perf_counter()
来源：http://rj.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://vp.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fg.colortex.cn

[U17] Py：初始化日志
来源：http://ec.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://yt.bjjhwx.cn

[U18] Py：预编译正则
来源：http://fm.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://aq.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://wp.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zq.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://zp.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://qd.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://gc.yuexingan06.cn

@contextlib.contextmanager
来源：http://qh.szsharing.cn

[U22] Py：矩阵转置
来源：http://bx.521024.cn

list(zip(*m))
来源：http://le.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://kw.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qm.colortex.cn

[U24] Py：路径操作
来源：http://cc.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zv.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://sk.panjiajie.cn

csv.DictReader(f)
来源：http://vg.nszjky.cn

[U26] Py：并发下载
来源：http://yf.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ma.521024.cn

[U27] Py：异步 HTTP
来源：http://ha.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://mz.haigaiapp.cn

[U28] Py：类型别名
来源：http://jg.nszjky.cn

UserId = int
来源：http://dx.wgjwhj.cn

[U29] Py：属性校验
来源：http://jv.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://fd.muxihuayi.cn

[U30] Py：数据类
来源：http://va.shxzukj.cn

@dataclass(slots=True)
来源：http://qw.panjiajie.cn

[U31] Py：单测
来源：http://wg.yuntaijiaju.cn

python -m pytest -q
来源：http://ti.szsharing.cn

[U32] Py：代码格式化
来源：http://ti.colortex.cn

ruff format . && ruff check --fix .
来源：http://lr.wgjwhj.cn

[U33] Py：打包发布
来源：http://az.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://hg.panjiajie.cn

[U34] Py：判断编码
来源：http://pd.jianghongdianzi.cn

chardet.detect(raw)
来源：http://ro.shxzukj.cn

[U35] Py：发送邮件
来源：http://vf.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vv.newstarts.cn

[U36] Py：定时任务
来源：http://hb.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://ee.szsharing.cn

[U37] Py：读写 Excel
来源：http://cd.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wx.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://bw.szxytkj.cn

Path(__file__).resolve().parent
来源：http://or.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://aw.shxzskj.cn

sys.stdout.isatty()
来源：http://lt.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://xg.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://rz.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://ac.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tv.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://cu.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cq.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://mk.shxzukj.cn

namespace App\Http;
来源：http://ej.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://qw.jianghongdianzi.cn

declare(strict_types=1);
来源：http://if.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://kf.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mj.shtwfgs.cn

[U46] PHP：可空类型
来源：http://lj.chemitech.net.cn

?string $name = null
来源：http://cn.haigaiapp.cn

[U47] PHP：联合类型
来源：http://ao.nicolike.cn

int|string $id
来源：http://do.nszjky.cn

[U48] PHP：纯枚举
来源：http://tv.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ag.shxzukj.cn

[U49] PHP：只读属性
来源：http://af.muxihuayi.cn

public readonly string $name
来源：http://ja.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://bu.521024.cn

public function __construct(private int $id) {}
来源：http://gv.asd995.cn

[U51] PHP：数组解构
来源：http://ys.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://xf.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://dx.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://mx.huanxung.cn

[U53] PHP：空合并运算符
来源：http://aj.521024.cn

$v = $a ?? $b ?? "default";
来源：http://hv.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://sq.szxytkj.cn

$obj?->method()
来源：http://bq.hnjuh.cn

[U55] PHP：match 表达式
来源：http://bz.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fa.szsharing.cn

[U56] PHP：命名参数
来源：http://uv.haigaiapp.cn

f(a: 1, b: 2)
来源：http://ak.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://bm.huanxung.cn

"值: {$a}"
来源：http://oz.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://pb.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qh.nicolike.cn


<!-- 参考信息 -->