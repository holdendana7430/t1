代发 wailian999

[S35] C++：map
来源：http://gl.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ed.shtwfgs.cn

[S36] C++：unordered_map
来源：http://lx.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ff.9csxet.cn

[S37] C++：set
来源：http://ei.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tr.huanxung.cn

[S38] C++：排序
来源：http://yo.asd995.cn

std::sort(v.begin(), v.end());
来源：http://vp.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://hi.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pc.colortex.cn

[S40] C++：查找元素
来源：http://rq.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://em.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://qa.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zv.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://ea.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://se.jctech888.com.cn

[S43] C++：智能指针
来源：http://jf.521024.cn

auto p = std::make_unique<int>(5);
来源：http://la.lnxyls.cn

[S44] C++：引用传参
来源：http://uo.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://ca.szsharing.cn

[S45] C++：lambda
来源：http://gd.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zj.colortex.cn

[S46] C++：函数模板
来源：http://lk.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zv.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://ej.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jt.nicolike.cn

[S48] C++：逐行读文件
来源：http://jj.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gx.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://ya.wgjwhj.cn

[S49] C++：写文件
来源：http://wr.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vc.jctech888.com.cn

[S50] C++：格式化数字
来源：http://wc.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oi.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://wf.hnjuh.cn

static_cast<double>(a) / b
来源：http://vd.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://ps.huanxung.cn

int size() const noexcept { return n_; }
来源：http://na.521024.cn

[S53] C++：移动语义
来源：http://oo.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://ji.lnxyls.cn

[S54] C++：异常处理
来源：http://ci.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nf.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://vx.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zv.muxihuayi.cn

[S56] C++：optional
来源：http://ml.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nm.nszjky.cn

[S57] C++：编译期常量
来源：http://wz.haigaiapp.cn

constexpr int N = 10;
来源：http://xi.shtwfgs.cn

[S58] C++：命名空间
来源：http://tn.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://hz.hahajie.cn

[S59] C++：静态断言
来源：http://zz.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ai.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://rr.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pr.asd995.cn

================================================================================
来源：http://jf.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qt.chemitech.net.cn

================================================================================
来源：http://yx.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://uj.hnjuh.cn

println("Hello")
来源：http://xs.521024.cn

[T02] Kotlin：变量
来源：http://ym.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nh.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://nz.shtwfgs.cn

"值: $b"
来源：http://sn.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://mj.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://kz.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://bi.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fj.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://jd.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://om.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://zh.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mh.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://ua.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://ld.asd995.cn

[T09] Kotlin：扩展函数
来源：http://wr.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://bw.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://np.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://op.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://bn.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tj.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://us.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://ft.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://jc.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://zy.gzmigu.cn

[T14] Kotlin：循环
来源：http://qd.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://dv.jctech888.com.cn

[T15] Kotlin：接口
来源：http://sk.colortex.cn

interface Shape { fun area(): Double }
来源：http://jf.panjiajie.cn

[T16] Swift：Hello World
来源：http://hk.newstarts.cn

print("Hello")
来源：http://ti.gzmigu.cn

[T17] Swift：变量与常量
来源：http://fa.gzmigu.cn

var a = 1;  let b = 2
来源：http://fe.szxytkj.cn

[T18] Swift：字符串插值
来源：http://ap.huixinmuqiang.cn

"值: \(b)"
来源：http://fu.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://vo.nszjky.cn

if let n = opt { print(n) }
来源：http://sl.lnxyls.cn

[T20] Swift：数组操作
来源：http://hw.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mi.asd995.cn

[T21] Swift：遍历
来源：http://yq.huixinmuqiang.cn

for x in a { print(x) }
来源：http://tz.newstarts.cn

[T22] Swift：字典
来源：http://ld.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uw.haigaiapp.cn

[T23] Swift：函数
来源：http://nj.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qx.huanxung.cn

[T24] Swift：闭包
来源：http://wn.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://km.haigaiapp.cn

[T25] Swift：结构体
来源：http://ai.gzmigu.cn

struct P { var x: Int }
来源：http://by.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://au.shxzskj.cn

class A: Base { override func f() {} }
来源：http://wy.huixiangedu.cn

[T27] Swift：错误处理
来源：http://oc.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://vo.nszjky.cn

[T28] Swift：枚举
来源：http://so.lnxyls.cn

enum Color { case red, green }
来源：http://mp.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://ac.9csxet.cn

guard let x = opt else { return }
来源：http://ut.9csxet.cn

[T30] Swift：协议
来源：http://uc.521024.cn

protocol Shape { func area() -> Double }
来源：http://go.szxytkj.cn

[T31] Lua：Hello World
来源：http://pq.szxytkj.cn

print("Hello")
来源：http://ea.huixiangedu.cn

[T32] Lua：局部变量
来源：http://tg.yuexingan06.cn

local a = 1
来源：http://zy.lnxyls.cn

[T33] Lua：表（数组）
来源：http://hz.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jv.muxihuayi.cn

[T34] Lua：遍历表
来源：http://bc.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jf.muxihuayi.cn

[T35] Lua：字典表
来源：http://sb.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://va.9csxet.cn

[T36] Lua：函数
来源：http://fz.nicolike.cn

function add(a, b) return a + b end
来源：http://ka.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://jm.9csxet.cn

"a" .. "b"
来源：http://xp.bjjhwx.cn

[T38] Lua：条件
来源：http://ay.szsharing.cn

if x > 0 then print("正") end
来源：http://jp.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://rb.bookmarksfly.cn

string.find(s, "%d+")
来源：http://jb.chemitech.net.cn

[T40] Lua：元表
来源：http://xf.9csxet.cn

setmetatable({}, { __index = base })
来源：http://aa.szsharing.cn

[T41] Perl：Hello World
来源：http://cj.shxzskj.cn

print "Hello\n";
来源：http://ar.wgjwhj.cn

[T42] Perl：变量类型
来源：http://uh.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ow.521024.cn

[T43] Perl：字符串插值
来源：http://iw.bookmarksfly.cn

"值: $a"
来源：http://vp.panjiajie.cn

[T44] Perl：条件
来源：http://hl.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://tj.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://rm.asd995.cn

for my $x (@arr) { print $x; }
来源：http://qf.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://qf.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cc.521024.cn

[T47] Perl：正则捕获
来源：http://nq.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nt.szxytkj.cn

[T48] Perl：正则替换
来源：http://fx.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://di.wgjwhj.cn

[T49] Perl：函数
来源：http://qn.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fs.hahajie.cn

[T50] Perl：逐行读文件
来源：http://jk.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ey.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://nc.yuexingan06.cn

[T51] Scala：Hello World
来源：http://kb.9csxet.cn

println("Hello")
来源：http://sj.huixinmuqiang.cn

[T52] Scala：变量
来源：http://an.muxihuayi.cn

val a = 1;  var b = 2
来源：http://mb.newstarts.cn

[T53] Scala：字符串插值
来源：http://ps.gzmigu.cn

s"值: $b"
来源：http://dt.huixiangedu.cn

[T54] Scala：集合映射
来源：http://yr.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://oi.shxzskj.cn

[T55] Scala：集合过滤
来源：http://go.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pk.yuexingan06.cn

[T56] Scala：样例类
来源：http://fs.huanxung.cn

case class User(name: String, age: Int)
来源：http://jc.hnjuh.cn

[T57] Scala：模式匹配
来源：http://ka.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dd.newstarts.cn

[T58] Scala：函数定义
来源：http://vj.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://to.521024.cn

[T59] Scala：循环
来源：http://aq.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://mw.nszjky.cn

[T60] Scala：折叠
来源：http://iv.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jc.muxihuayi.cn

================================================================================
来源：http://lr.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ql.9csxet.cn

================================================================================
来源：http://xx.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://dk.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oi.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://dh.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://om.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://ph.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qj.gzmigu.cn

[U04] Py：变量调试打印
来源：http://fk.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nu.szsharing.cn

[U05] Py：列表去重且保序
来源：http://bc.colortex.cn

list(dict.fromkeys(arr))
来源：http://hi.shxzukj.cn

[U06] Py：合并两个字典
来源：http://cm.shxzskj.cn

{**a, **b}
来源：http://pd.newstarts.cn

[U07] Py：反转字典键值
来源：http://mx.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://pb.shxzukj.cn

[U08] Py：展平二维列表
来源：http://zy.521024.cn

[y for x in nested for y in x]
来源：http://yp.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://mc.muxihuayi.cn

max(d, key=d.get)
来源：http://tb.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://sh.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qq.gzmigu.cn

[U11] Py：生成器表达式
来源：http://yp.hnjuh.cn

(x * 2 for x in arr)
来源：http://vz.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qm.panjiajie.cn

Counter(arr).most_common(3)
来源：http://pq.521024.cn

[U13] Py：固定长度队列
来源：http://cv.hnjuh.cn

deque(maxlen=10)
来源：http://yq.huanxung.cn

[U14] Py：分组收集到列表
来源：http://te.huanxung.cn

defaultdict(list)
来源：http://xe.wgjwhj.cn

[U15] Py：高精度计时
来源：http://qo.huixiangedu.cn

t = time.perf_counter()
来源：http://ld.nszjky.cn

[U16] Py：命令行参数解析
来源：http://on.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ie.hahajie.cn

[U17] Py：初始化日志
来源：http://nv.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://ap.huanxung.cn

[U18] Py：预编译正则
来源：http://cr.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://lw.colortex.cn

[U19] Py：正则替换带回调
来源：http://hs.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vh.nicolike.cn

[U20] Py：缓存函数结果
来源：http://fu.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://iv.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://pn.nicolike.cn

@contextlib.contextmanager
来源：http://yt.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://xw.yuntaijiaju.cn

list(zip(*m))
来源：http://ub.nszjky.cn

[U23] Py：分块读取大文件
来源：http://ux.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ta.panjiajie.cn

[U24] Py：路径操作
来源：http://mk.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rt.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://ti.bookmarksfly.cn

csv.DictReader(f)
来源：http://ok.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://mw.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mo.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://vb.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://fl.jctech888.com.cn

[U28] Py：类型别名
来源：http://fn.hahajie.cn

UserId = int
来源：http://hd.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://ys.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://of.asd995.cn

[U30] Py：数据类
来源：http://gl.newstarts.cn

@dataclass(slots=True)
来源：http://cb.newstarts.cn

[U31] Py：单测
来源：http://lo.nicolike.cn

python -m pytest -q
来源：http://ne.wgjwhj.cn

[U32] Py：代码格式化
来源：http://mw.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://lt.bookmarksfly.cn

[U33] Py：打包发布
来源：http://up.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://va.gzmigu.cn

[U34] Py：判断编码
来源：http://xo.yuexingan06.cn

chardet.detect(raw)
来源：http://do.lnxyls.cn

[U35] Py：发送邮件
来源：http://qz.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zv.nicolike.cn

[U36] Py：定时任务
来源：http://hz.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://yd.colortex.cn

[U37] Py：读写 Excel
来源：http://wz.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lr.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://zv.521024.cn

Path(__file__).resolve().parent
来源：http://dx.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://mi.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://oy.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://st.shxzskj.cn

print("err", file=sys.stderr)
来源：http://xl.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://wu.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://us.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://zl.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yg.szsharing.cn

[U43] PHP：声明命名空间
来源：http://ub.huixinmuqiang.cn

namespace App\Http;
来源：http://qc.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://az.shtwfgs.cn

declare(strict_types=1);
来源：http://vj.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://yj.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://on.huixiangedu.cn

[U46] PHP：可空类型
来源：http://ro.asd995.cn

?string $name = null
来源：http://dm.muxihuayi.cn

[U47] PHP：联合类型
来源：http://pe.jctech888.com.cn

int|string $id
来源：http://av.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://pa.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ch.bjjhwx.cn

[U49] PHP：只读属性
来源：http://kn.521024.cn

public readonly string $name
来源：http://th.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://hn.hahajie.cn

public function __construct(private int $id) {}
来源：http://eu.shxzskj.cn

[U51] PHP：数组解构
来源：http://pz.nszjky.cn

[$a, $b] = $arr;
来源：http://ws.huanxung.cn

[U52] PHP：箭头函数
来源：http://ic.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://yf.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://pq.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://mp.gzmigu.cn

[U54] PHP：空安全调用
来源：http://yv.nszjky.cn

$obj?->method()
来源：http://uw.shxzskj.cn

[U55] PHP：match 表达式
来源：http://pz.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ga.newstarts.cn

[U56] PHP：命名参数
来源：http://og.shxzukj.cn

f(a: 1, b: 2)
来源：http://cv.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://kw.huanxung.cn

"值: {$a}"
来源：http://nm.521024.cn

[U58] PHP：数组三件套
来源：http://rv.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bw.colortex.cn

[U59] PHP：自定义排序
来源：http://wl.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nw.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://ur.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ev.bjjhwx.cn


<!-- 参考信息 -->