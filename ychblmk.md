代发 wailian999

[S33] C++：vector 增删
来源：http://dg.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ep.asd995.cn

[S34] C++：遍历 vector
来源：http://pn.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://op.jianghongdianzi.cn

[S35] C++：map
来源：http://nm.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tc.szxytkj.cn

[S36] C++：unordered_map
来源：http://iq.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ud.haigaiapp.cn

[S37] C++：set
来源：http://jh.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vk.9csxet.cn

[S38] C++：排序
来源：http://zq.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://mw.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://ef.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://st.bookmarksfly.cn

[S40] C++：查找元素
来源：http://vc.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ci.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://gp.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ql.nicolike.cn

[S42] C++：继承与虚函数
来源：http://bo.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://fw.chemitech.net.cn

[S43] C++：智能指针
来源：http://ro.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://fq.chemitech.net.cn

[S44] C++：引用传参
来源：http://pz.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://xh.jctech888.com.cn

[S45] C++：lambda
来源：http://rn.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gk.hnjuh.cn

[S46] C++：函数模板
来源：http://hz.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lb.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://mn.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uz.lnxyls.cn

[S48] C++：逐行读文件
来源：http://yc.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qk.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://ub.jctech888.com.cn

[S49] C++：写文件
来源：http://go.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qw.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://ed.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sa.szxytkj.cn

[S51] C++：显式类型转换
来源：http://px.yuexingan06.cn

static_cast<double>(a) / b
来源：http://aq.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://li.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://xw.hnjuh.cn

[S53] C++：移动语义
来源：http://lu.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://kq.jctech888.com.cn

[S54] C++：异常处理
来源：http://zm.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ak.gzmigu.cn

[S55] C++：结构化绑定
来源：http://dj.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zc.bookmarksfly.cn

[S56] C++：optional
来源：http://al.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ly.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://do.newstarts.cn

constexpr int N = 10;
来源：http://dm.szxytkj.cn

[S58] C++：命名空间
来源：http://ij.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://hw.hahajie.cn

[S59] C++：静态断言
来源：http://wj.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wb.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://jl.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tc.panjiajie.cn

================================================================================
来源：http://rf.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dh.shtwfgs.cn

================================================================================
来源：http://bm.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://ai.yuntaijiaju.cn

println("Hello")
来源：http://by.shxzskj.cn

[T02] Kotlin：变量
来源：http://ci.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rw.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://pc.panjiajie.cn

"值: $b"
来源：http://al.hnjuh.cn

[T04] Kotlin：空安全
来源：http://in.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://yy.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://hl.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://re.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://dr.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yy.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://kh.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qs.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://wu.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://jt.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://fw.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://so.9csxet.cn

[T10] Kotlin：默认参数
来源：http://ge.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uy.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://ip.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ks.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://bf.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://bt.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://oz.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://qt.szxytkj.cn

[T14] Kotlin：循环
来源：http://tq.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://yo.wgjwhj.cn

[T15] Kotlin：接口
来源：http://rh.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://hv.hnjuh.cn

[T16] Swift：Hello World
来源：http://kw.huixinmuqiang.cn

print("Hello")
来源：http://kw.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://oj.jctech888.com.cn

var a = 1;  let b = 2
来源：http://jz.shxzukj.cn

[T18] Swift：字符串插值
来源：http://yg.shxzukj.cn

"值: \(b)"
来源：http://rq.newstarts.cn

[T19] Swift：可选绑定
来源：http://va.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://dr.yuexingan06.cn

[T20] Swift：数组操作
来源：http://ma.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ne.newstarts.cn

[T21] Swift：遍历
来源：http://ov.muxihuayi.cn

for x in a { print(x) }
来源：http://ui.szxytkj.cn

[T22] Swift：字典
来源：http://gv.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bg.szxytkj.cn

[T23] Swift：函数
来源：http://ms.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://it.shxzskj.cn

[T24] Swift：闭包
来源：http://gz.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cw.yuexingan06.cn

[T25] Swift：结构体
来源：http://sf.lnxyls.cn

struct P { var x: Int }
来源：http://hl.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://kh.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://cu.shtwfgs.cn

[T27] Swift：错误处理
来源：http://ww.huanxung.cn

do { try f() } catch { print(error) }
来源：http://uu.gzmigu.cn

[T28] Swift：枚举
来源：http://lc.newstarts.cn

enum Color { case red, green }
来源：http://jl.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://fa.chemitech.net.cn

guard let x = opt else { return }
来源：http://zp.wgjwhj.cn

[T30] Swift：协议
来源：http://wi.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://iy.yuexingan06.cn

[T31] Lua：Hello World
来源：http://pb.bjjhwx.cn

print("Hello")
来源：http://of.shxzukj.cn

[T32] Lua：局部变量
来源：http://rj.chemitech.net.cn

local a = 1
来源：http://le.asd995.cn

[T33] Lua：表（数组）
来源：http://rk.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tj.haigaiapp.cn

[T34] Lua：遍历表
来源：http://do.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ne.lnxyls.cn

[T35] Lua：字典表
来源：http://eu.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://zs.nicolike.cn

[T36] Lua：函数
来源：http://vc.9csxet.cn

function add(a, b) return a + b end
来源：http://om.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://fe.shtwfgs.cn

"a" .. "b"
来源：http://lz.newstarts.cn

[T38] Lua：条件
来源：http://ep.nicolike.cn

if x > 0 then print("正") end
来源：http://tw.panjiajie.cn

[T39] Lua：模式匹配
来源：http://vh.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://xu.newstarts.cn

[T40] Lua：元表
来源：http://iy.newstarts.cn

setmetatable({}, { __index = base })
来源：http://gu.bjjhwx.cn

[T41] Perl：Hello World
来源：http://sa.jianghongdianzi.cn

print "Hello\n";
来源：http://lc.gzmigu.cn

[T42] Perl：变量类型
来源：http://mp.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mo.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://ga.muxihuayi.cn

"值: $a"
来源：http://bg.shxzskj.cn

[T44] Perl：条件
来源：http://fn.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://at.szsharing.cn

[T45] Perl：数组遍历
来源：http://cm.colortex.cn

for my $x (@arr) { print $x; }
来源：http://qh.hahajie.cn

[T46] Perl：哈希操作
来源：http://yr.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lr.colortex.cn

[T47] Perl：正则捕获
来源：http://rj.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nq.jctech888.com.cn

[T48] Perl：正则替换
来源：http://ue.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://hz.newstarts.cn

[T49] Perl：函数
来源：http://vg.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yn.colortex.cn

[T50] Perl：逐行读文件
来源：http://ca.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oz.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://iv.huanxung.cn

[T51] Scala：Hello World
来源：http://ta.9csxet.cn

println("Hello")
来源：http://tq.panjiajie.cn

[T52] Scala：变量
来源：http://bk.chemitech.net.cn

val a = 1;  var b = 2
来源：http://bd.hnjuh.cn

[T53] Scala：字符串插值
来源：http://ys.szxytkj.cn

s"值: $b"
来源：http://tm.wgjwhj.cn

[T54] Scala：集合映射
来源：http://bo.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://zo.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://qt.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kp.jctech888.com.cn

[T56] Scala：样例类
来源：http://uc.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://mm.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://yz.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tp.colortex.cn

[T58] Scala：函数定义
来源：http://kv.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ur.colortex.cn

[T59] Scala：循环
来源：http://xl.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://py.yuexingan06.cn

[T60] Scala：折叠
来源：http://gu.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gm.bookmarksfly.cn

================================================================================
来源：http://ia.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fo.hnjuh.cn

================================================================================
来源：http://sl.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://ue.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://by.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://cm.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nx.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://sr.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tx.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://we.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uu.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://dd.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://oc.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://rz.bjjhwx.cn

{**a, **b}
来源：http://xn.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://jn.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://nw.hahajie.cn

[U08] Py：展平二维列表
来源：http://wb.chemitech.net.cn

[y for x in nested for y in x]
来源：http://ue.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://et.panjiajie.cn

max(d, key=d.get)
来源：http://gu.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://ek.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ju.lnxyls.cn

[U11] Py：生成器表达式
来源：http://fq.9csxet.cn

(x * 2 for x in arr)
来源：http://zu.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://me.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://rc.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://eu.lnxyls.cn

deque(maxlen=10)
来源：http://ht.nszjky.cn

[U14] Py：分组收集到列表
来源：http://dx.521024.cn

defaultdict(list)
来源：http://bp.lnxyls.cn

[U15] Py：高精度计时
来源：http://nf.newstarts.cn

t = time.perf_counter()
来源：http://zj.hahajie.cn

[U16] Py：命令行参数解析
来源：http://ag.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fw.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://lm.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://wh.nszjky.cn

[U18] Py：预编译正则
来源：http://yw.asd995.cn

pat = re.compile(r"\d+")
来源：http://ex.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://vi.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rz.nszjky.cn

[U20] Py：缓存函数结果
来源：http://cc.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://fc.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://yu.szsharing.cn

@contextlib.contextmanager
来源：http://wh.asd995.cn

[U22] Py：矩阵转置
来源：http://dv.nicolike.cn

list(zip(*m))
来源：http://dk.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://fr.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ea.bjjhwx.cn

[U24] Py：路径操作
来源：http://vj.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fs.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://zk.nicolike.cn

csv.DictReader(f)
来源：http://tm.bjjhwx.cn

[U26] Py：并发下载
来源：http://tx.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qr.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://pt.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://wt.szxytkj.cn

[U28] Py：类型别名
来源：http://ig.shtwfgs.cn

UserId = int
来源：http://he.huanxung.cn

[U29] Py：属性校验
来源：http://yc.asd995.cn

@property 与 @x.setter 配合
来源：http://ry.yuexingan06.cn

[U30] Py：数据类
来源：http://ue.shtwfgs.cn

@dataclass(slots=True)
来源：http://ue.haigaiapp.cn

[U31] Py：单测
来源：http://jn.521024.cn

python -m pytest -q
来源：http://lo.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://en.colortex.cn

ruff format . && ruff check --fix .
来源：http://pd.hahajie.cn

[U33] Py：打包发布
来源：http://cl.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://kg.shxzskj.cn

[U34] Py：判断编码
来源：http://oq.shxzukj.cn

chardet.detect(raw)
来源：http://rd.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://wv.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nd.shtwfgs.cn

[U36] Py：定时任务
来源：http://rv.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://mf.nszjky.cn

[U37] Py：读写 Excel
来源：http://ft.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zq.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://pa.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://xf.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://ys.521024.cn

sys.stdout.isatty()
来源：http://mn.huanxung.cn

[U40] Py：打印到标准错误
来源：http://to.nicolike.cn

print("err", file=sys.stderr)
来源：http://dh.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://nu.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mh.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://xk.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://do.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://gx.yuexingan06.cn

namespace App\Http;
来源：http://qr.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://sp.shxzukj.cn

declare(strict_types=1);
来源：http://xo.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://nh.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cs.colortex.cn

[U46] PHP：可空类型
来源：http://qh.asd995.cn

?string $name = null
来源：http://qz.521024.cn

[U47] PHP：联合类型
来源：http://fy.nszjky.cn

int|string $id
来源：http://gs.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://ot.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ns.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://mv.szxytkj.cn

public readonly string $name
来源：http://na.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://wm.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://fs.panjiajie.cn

[U51] PHP：数组解构
来源：http://kl.shxzskj.cn

[$a, $b] = $arr;
来源：http://dp.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://kj.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://fs.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://bf.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://nu.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://fm.bookmarksfly.cn

$obj?->method()
来源：http://vs.nszjky.cn

[U55] PHP：match 表达式
来源：http://kw.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qn.panjiajie.cn

[U56] PHP：命名参数
来源：http://yk.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://tm.hnjuh.cn

[U57] PHP：字符串插值
来源：http://hr.asd995.cn

"值: {$a}"
来源：http://kf.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://yw.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vi.bookmarksfly.cn


<!-- 参考信息 -->