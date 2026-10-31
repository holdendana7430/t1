代发 wailian999

[S37] C++：set
来源：http://md.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mw.hahajie.cn

[S38] C++：排序
来源：http://ze.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://em.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://qw.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dj.hahajie.cn

[S40] C++：查找元素
来源：http://zf.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://av.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://ka.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ka.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://ms.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://zk.shxzskj.cn

[S43] C++：智能指针
来源：http://eh.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://ay.asd995.cn

[S44] C++：引用传参
来源：http://hf.newstarts.cn

void inc(int &x) { ++x; }
来源：http://nt.muxihuayi.cn

[S45] C++：lambda
来源：http://wj.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://il.shxzskj.cn

[S46] C++：函数模板
来源：http://gb.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ki.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://up.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lr.gzmigu.cn

[S48] C++：逐行读文件
来源：http://tv.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://er.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://oq.szsharing.cn

[S49] C++：写文件
来源：http://oh.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://al.shxzskj.cn

[S50] C++：格式化数字
来源：http://mc.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pf.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://pp.hnjuh.cn

static_cast<double>(a) / b
来源：http://ao.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://vt.521024.cn

int size() const noexcept { return n_; }
来源：http://ak.521024.cn

[S53] C++：移动语义
来源：http://tc.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://xq.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://md.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tx.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://uq.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xd.yuntaijiaju.cn

[S56] C++：optional
来源：http://bw.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hr.nszjky.cn

[S57] C++：编译期常量
来源：http://lo.shxzskj.cn

constexpr int N = 10;
来源：http://rz.hahajie.cn

[S58] C++：命名空间
来源：http://vk.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://kf.haigaiapp.cn

[S59] C++：静态断言
来源：http://gt.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nh.asd995.cn

[S60] C++：遍历并删除元素
来源：http://nc.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vn.bookmarksfly.cn

================================================================================
来源：http://tf.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yi.haigaiapp.cn

================================================================================
来源：http://oj.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://aw.521024.cn

println("Hello")
来源：http://jc.szsharing.cn

[T02] Kotlin：变量
来源：http://lj.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ca.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://qe.nicolike.cn

"值: $b"
来源：http://eg.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://wu.521024.cn

val n: String? = null;  n?.length
来源：http://mc.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://bd.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ws.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://iq.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ti.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://xw.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hx.nicolike.cn

[T08] Kotlin：数据类
来源：http://sn.521024.cn

data class User(val name: String, val age: Int)
来源：http://ye.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://qz.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://xo.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://xe.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ez.szsharing.cn

[T11] Kotlin：协程
来源：http://pt.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xq.szsharing.cn

[T12] Kotlin：解构声明
来源：http://fs.521024.cn

val (a, b) = Pair(1, 2)
来源：http://qu.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://vi.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://oo.colortex.cn

[T14] Kotlin：循环
来源：http://ie.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://te.huixiangedu.cn

[T15] Kotlin：接口
来源：http://tl.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://kv.wgjwhj.cn

[T16] Swift：Hello World
来源：http://za.hahajie.cn

print("Hello")
来源：http://rz.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://fc.wgjwhj.cn

var a = 1;  let b = 2
来源：http://at.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://gt.9csxet.cn

"值: \(b)"
来源：http://pv.lnxyls.cn

[T19] Swift：可选绑定
来源：http://qe.521024.cn

if let n = opt { print(n) }
来源：http://gg.nicolike.cn

[T20] Swift：数组操作
来源：http://ld.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yh.shxzskj.cn

[T21] Swift：遍历
来源：http://tp.521024.cn

for x in a { print(x) }
来源：http://fv.szsharing.cn

[T22] Swift：字典
来源：http://ly.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://di.yuntaijiaju.cn

[T23] Swift：函数
来源：http://zd.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://af.hahajie.cn

[T24] Swift：闭包
来源：http://tn.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dz.chemitech.net.cn

[T25] Swift：结构体
来源：http://xi.huixinmuqiang.cn

struct P { var x: Int }
来源：http://wu.huanxung.cn

[T26] Swift：类与重写
来源：http://yq.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://mk.lnxyls.cn

[T27] Swift：错误处理
来源：http://wt.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://bs.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://fn.shxzskj.cn

enum Color { case red, green }
来源：http://cf.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://km.shtwfgs.cn

guard let x = opt else { return }
来源：http://ai.shtwfgs.cn

[T30] Swift：协议
来源：http://qs.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://us.colortex.cn

[T31] Lua：Hello World
来源：http://on.huanxung.cn

print("Hello")
来源：http://pu.9csxet.cn

[T32] Lua：局部变量
来源：http://cy.huixiangedu.cn

local a = 1
来源：http://wa.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://bw.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zb.bjjhwx.cn

[T34] Lua：遍历表
来源：http://xf.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://di.shxzukj.cn

[T35] Lua：字典表
来源：http://tn.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://pk.shtwfgs.cn

[T36] Lua：函数
来源：http://jn.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://ih.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://wr.521024.cn

"a" .. "b"
来源：http://ak.nszjky.cn

[T38] Lua：条件
来源：http://qm.panjiajie.cn

if x > 0 then print("正") end
来源：http://su.9csxet.cn

[T39] Lua：模式匹配
来源：http://zo.colortex.cn

string.find(s, "%d+")
来源：http://re.nicolike.cn

[T40] Lua：元表
来源：http://lf.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://jq.szsharing.cn

[T41] Perl：Hello World
来源：http://ws.jianghongdianzi.cn

print "Hello\n";
来源：http://cm.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://ap.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vl.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://nr.jianghongdianzi.cn

"值: $a"
来源：http://za.szxytkj.cn

[T44] Perl：条件
来源：http://ty.asd995.cn

if ($a > 0) { print "正"; }
来源：http://xr.hahajie.cn

[T45] Perl：数组遍历
来源：http://cg.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://cv.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://vk.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://li.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://kl.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bm.nicolike.cn

[T48] Perl：正则替换
来源：http://vo.szsharing.cn

$s =~ s/old/new/g;
来源：http://ik.yuntaijiaju.cn

[T49] Perl：函数
来源：http://dw.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dm.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://qc.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ks.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://oi.chemitech.net.cn

[T51] Scala：Hello World
来源：http://ec.hahajie.cn

println("Hello")
来源：http://qf.yuexingan06.cn

[T52] Scala：变量
来源：http://dj.lnxyls.cn

val a = 1;  var b = 2
来源：http://pq.hahajie.cn

[T53] Scala：字符串插值
来源：http://cs.shtwfgs.cn

s"值: $b"
来源：http://xx.chemitech.net.cn

[T54] Scala：集合映射
来源：http://io.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://so.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://kv.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gx.huanxung.cn

[T56] Scala：样例类
来源：http://hw.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://xx.nicolike.cn

[T57] Scala：模式匹配
来源：http://xu.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rf.panjiajie.cn

[T58] Scala：函数定义
来源：http://pe.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qn.gzmigu.cn

[T59] Scala：循环
来源：http://ss.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://hd.shtwfgs.cn

[T60] Scala：折叠
来源：http://rj.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kb.shxzukj.cn

================================================================================
来源：http://yv.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rr.yuntaijiaju.cn

================================================================================
来源：http://yw.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://dd.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pp.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://dr.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://us.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://lp.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fi.gzmigu.cn

[U04] Py：变量调试打印
来源：http://ck.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hh.asd995.cn

[U05] Py：列表去重且保序
来源：http://iy.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://ty.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://zv.9csxet.cn

{**a, **b}
来源：http://yj.9csxet.cn

[U07] Py：反转字典键值
来源：http://cs.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://rj.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://hi.muxihuayi.cn

[y for x in nested for y in x]
来源：http://bs.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://nz.bjjhwx.cn

max(d, key=d.get)
来源：http://rr.shxzukj.cn

[U10] Py：按值排序字典
来源：http://ug.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wh.shxzukj.cn

[U11] Py：生成器表达式
来源：http://vy.lnxyls.cn

(x * 2 for x in arr)
来源：http://xy.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://we.521024.cn

Counter(arr).most_common(3)
来源：http://ji.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://oh.9csxet.cn

deque(maxlen=10)
来源：http://dh.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://tw.colortex.cn

defaultdict(list)
来源：http://ni.lnxyls.cn

[U15] Py：高精度计时
来源：http://nx.bookmarksfly.cn

t = time.perf_counter()
来源：http://xn.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://qp.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pq.hahajie.cn

[U17] Py：初始化日志
来源：http://iu.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://nt.shxzukj.cn

[U18] Py：预编译正则
来源：http://pm.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://zs.huanxung.cn

[U19] Py：正则替换带回调
来源：http://cf.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pr.szsharing.cn

[U20] Py：缓存函数结果
来源：http://hz.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://ok.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://bb.bjjhwx.cn

@contextlib.contextmanager
来源：http://ap.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://nx.wgjwhj.cn

list(zip(*m))
来源：http://sk.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://yw.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fw.wgjwhj.cn

[U24] Py：路径操作
来源：http://oq.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bn.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://wt.jianghongdianzi.cn

csv.DictReader(f)
来源：http://cn.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://xe.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qx.521024.cn

[U27] Py：异步 HTTP
来源：http://au.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://lm.wgjwhj.cn

[U28] Py：类型别名
来源：http://zc.bjjhwx.cn

UserId = int
来源：http://br.colortex.cn

[U29] Py：属性校验
来源：http://xr.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://sl.shtwfgs.cn

[U30] Py：数据类
来源：http://ks.chemitech.net.cn

@dataclass(slots=True)
来源：http://qw.gzmigu.cn

[U31] Py：单测
来源：http://en.huanxung.cn

python -m pytest -q
来源：http://ac.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://rs.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://es.huanxung.cn

[U33] Py：打包发布
来源：http://gl.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://pz.jctech888.com.cn

[U34] Py：判断编码
来源：http://sp.haigaiapp.cn

chardet.detect(raw)
来源：http://ou.asd995.cn

[U35] Py：发送邮件
来源：http://wh.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kb.huanxung.cn

[U36] Py：定时任务
来源：http://xe.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://we.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://mn.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://no.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://pq.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://ri.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://ec.bjjhwx.cn

sys.stdout.isatty()
来源：http://oo.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://lz.gzmigu.cn

print("err", file=sys.stderr)
来源：http://vx.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://ge.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kg.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://no.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qk.hahajie.cn

[U43] PHP：声明命名空间
来源：http://fo.lnxyls.cn

namespace App\Http;
来源：http://dl.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://zr.huanxung.cn

declare(strict_types=1);
来源：http://fe.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://sf.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vk.lnxyls.cn

[U46] PHP：可空类型
来源：http://yo.gzmigu.cn

?string $name = null
来源：http://bq.colortex.cn

[U47] PHP：联合类型
来源：http://cd.shxzskj.cn

int|string $id
来源：http://vv.bookmarksfly.cn

[U48] PHP：纯枚举
来源：http://ah.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://no.wgjwhj.cn

[U49] PHP：只读属性
来源：http://lh.521024.cn

public readonly string $name
来源：http://hs.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://oq.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://pv.panjiajie.cn

[U51] PHP：数组解构
来源：http://dm.shxzskj.cn

[$a, $b] = $arr;
来源：http://at.huanxung.cn

[U52] PHP：箭头函数
来源：http://ep.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://ug.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://pl.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://kr.colortex.cn

[U54] PHP：空安全调用
来源：http://kb.jianghongdianzi.cn

$obj?->method()
来源：http://xf.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://kk.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bq.huixiangedu.cn

[U56] PHP：命名参数
来源：http://ig.hahajie.cn

f(a: 1, b: 2)
来源：http://sa.szxytkj.cn

[U57] PHP：字符串插值
来源：http://lp.nicolike.cn

"值: {$a}"
来源：http://ja.gzmigu.cn

[U58] PHP：数组三件套
来源：http://gq.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tr.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://ft.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ze.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://jz.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://td.haigaiapp.cn

[U61] PHP：正则
来源：http://hs.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cs.yuexingan06.cn

[U62] PHP：日期对象
来源：http://iy.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fq.bookmarksfly.cn


<!-- 参考信息 -->