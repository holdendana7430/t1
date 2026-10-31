代发 wailian999

[S33] C++：vector 增删
来源：http://kf.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ed.szxytkj.cn

[S34] C++：遍历 vector
来源：http://kj.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://cs.nicolike.cn

[S35] C++：map
来源：http://oo.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pt.newstarts.cn

[S36] C++：unordered_map
来源：http://cd.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ho.bjjhwx.cn

[S37] C++：set
来源：http://bk.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nj.hnjuh.cn

[S38] C++：排序
来源：http://gn.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://ef.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://tg.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mc.hahajie.cn

[S40] C++：查找元素
来源：http://bk.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bj.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://wp.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aq.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://mp.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://zf.wgjwhj.cn

[S43] C++：智能指针
来源：http://nl.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://kl.haigaiapp.cn

[S44] C++：引用传参
来源：http://mh.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://nv.newstarts.cn

[S45] C++：lambda
来源：http://ha.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tl.nszjky.cn

[S46] C++：函数模板
来源：http://dm.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qd.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://vi.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bt.gzmigu.cn

[S48] C++：逐行读文件
来源：http://gv.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ht.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://sz.szsharing.cn

[S49] C++：写文件
来源：http://fi.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jx.lnxyls.cn

[S50] C++：格式化数字
来源：http://tw.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fa.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://ck.haigaiapp.cn

static_cast<double>(a) / b
来源：http://od.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://es.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://ry.muxihuayi.cn

[S53] C++：移动语义
来源：http://of.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://vn.asd995.cn

[S54] C++：异常处理
来源：http://yr.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sd.colortex.cn

[S55] C++：结构化绑定
来源：http://wf.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kg.asd995.cn

[S56] C++：optional
来源：http://rs.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ed.521024.cn

[S57] C++：编译期常量
来源：http://ul.yuntaijiaju.cn

constexpr int N = 10;
来源：http://nf.shtwfgs.cn

[S58] C++：命名空间
来源：http://og.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://cg.panjiajie.cn

[S59] C++：静态断言
来源：http://gn.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rc.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://zj.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zr.colortex.cn

================================================================================
来源：http://mv.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://to.shxzskj.cn

================================================================================
来源：http://qq.nszjky.cn

[T01] Kotlin：Hello World
来源：http://aw.colortex.cn

println("Hello")
来源：http://vz.huixiangedu.cn

[T02] Kotlin：变量
来源：http://la.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gn.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://rx.lnxyls.cn

"值: $b"
来源：http://gv.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://xg.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://nc.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://hm.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fe.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://vj.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dc.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://wo.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ve.newstarts.cn

[T08] Kotlin：数据类
来源：http://if.521024.cn

data class User(val name: String, val age: Int)
来源：http://vi.asd995.cn

[T09] Kotlin：扩展函数
来源：http://sd.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://cd.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://dh.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oy.wgjwhj.cn

[T11] Kotlin：协程
来源：http://gr.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ig.colortex.cn

[T12] Kotlin：解构声明
来源：http://fe.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://ll.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://nn.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://gd.shtwfgs.cn

[T14] Kotlin：循环
来源：http://pu.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://wv.yuexingan06.cn

[T15] Kotlin：接口
来源：http://eh.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://ed.muxihuayi.cn

[T16] Swift：Hello World
来源：http://xt.haigaiapp.cn

print("Hello")
来源：http://dl.521024.cn

[T17] Swift：变量与常量
来源：http://gb.nszjky.cn

var a = 1;  let b = 2
来源：http://ju.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://hz.shtwfgs.cn

"值: \(b)"
来源：http://ev.nicolike.cn

[T19] Swift：可选绑定
来源：http://ht.nicolike.cn

if let n = opt { print(n) }
来源：http://hd.hahajie.cn

[T20] Swift：数组操作
来源：http://lb.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ey.lnxyls.cn

[T21] Swift：遍历
来源：http://en.colortex.cn

for x in a { print(x) }
来源：http://pm.shxzskj.cn

[T22] Swift：字典
来源：http://zf.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ej.bookmarksfly.cn

[T23] Swift：函数
来源：http://ud.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ig.panjiajie.cn

[T24] Swift：闭包
来源：http://pd.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kp.gzmigu.cn

[T25] Swift：结构体
来源：http://nj.hnjuh.cn

struct P { var x: Int }
来源：http://dh.bjjhwx.cn

[T26] Swift：类与重写
来源：http://vx.nszjky.cn

class A: Base { override func f() {} }
来源：http://ir.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://rv.newstarts.cn

do { try f() } catch { print(error) }
来源：http://fo.nicolike.cn

[T28] Swift：枚举
来源：http://my.asd995.cn

enum Color { case red, green }
来源：http://qy.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://ds.huanxung.cn

guard let x = opt else { return }
来源：http://zi.szxytkj.cn

[T30] Swift：协议
来源：http://br.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://nv.9csxet.cn

[T31] Lua：Hello World
来源：http://fi.9csxet.cn

print("Hello")
来源：http://kj.asd995.cn

[T32] Lua：局部变量
来源：http://zg.yuexingan06.cn

local a = 1
来源：http://op.asd995.cn

[T33] Lua：表（数组）
来源：http://yr.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zz.asd995.cn

[T34] Lua：遍历表
来源：http://wr.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://by.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://fr.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://ul.huanxung.cn

[T36] Lua：函数
来源：http://vk.shxzskj.cn

function add(a, b) return a + b end
来源：http://pt.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://sg.muxihuayi.cn

"a" .. "b"
来源：http://me.panjiajie.cn

[T38] Lua：条件
来源：http://pw.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://zr.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://ck.asd995.cn

string.find(s, "%d+")
来源：http://vv.hahajie.cn

[T40] Lua：元表
来源：http://lg.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://dy.panjiajie.cn

[T41] Perl：Hello World
来源：http://tm.9csxet.cn

print "Hello\n";
来源：http://pw.szsharing.cn

[T42] Perl：变量类型
来源：http://if.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nn.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://kg.newstarts.cn

"值: $a"
来源：http://vl.bookmarksfly.cn

[T44] Perl：条件
来源：http://qk.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://yf.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://fg.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://dm.nicolike.cn

[T46] Perl：哈希操作
来源：http://ob.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sm.shxzskj.cn

[T47] Perl：正则捕获
来源：http://wy.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gh.szsharing.cn

[T48] Perl：正则替换
来源：http://vt.huanxung.cn

$s =~ s/old/new/g;
来源：http://xu.nicolike.cn

[T49] Perl：函数
来源：http://fe.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oj.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://hp.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vr.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://sx.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://mj.shxzskj.cn

println("Hello")
来源：http://xv.szsharing.cn

[T52] Scala：变量
来源：http://cx.9csxet.cn

val a = 1;  var b = 2
来源：http://mp.hahajie.cn

[T53] Scala：字符串插值
来源：http://uc.gzmigu.cn

s"值: $b"
来源：http://sa.szxytkj.cn

[T54] Scala：集合映射
来源：http://ns.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://gx.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://gj.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sa.chemitech.net.cn

[T56] Scala：样例类
来源：http://ow.huanxung.cn

case class User(name: String, age: Int)
来源：http://jr.nicolike.cn

[T57] Scala：模式匹配
来源：http://yp.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ga.bjjhwx.cn

[T58] Scala：函数定义
来源：http://jr.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://by.shtwfgs.cn

[T59] Scala：循环
来源：http://go.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://uw.wgjwhj.cn

[T60] Scala：折叠
来源：http://be.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mv.haigaiapp.cn

================================================================================
来源：http://gb.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ka.hnjuh.cn

================================================================================
来源：http://lv.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://ki.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ml.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://sm.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://me.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://qg.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gt.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://rf.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jc.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://fy.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://us.colortex.cn

[U06] Py：合并两个字典
来源：http://ry.wgjwhj.cn

{**a, **b}
来源：http://cn.panjiajie.cn

[U07] Py：反转字典键值
来源：http://ao.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://nn.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://go.muxihuayi.cn

[y for x in nested for y in x]
来源：http://or.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://pr.huixiangedu.cn

max(d, key=d.get)
来源：http://jz.colortex.cn

[U10] Py：按值排序字典
来源：http://mt.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jo.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://hb.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://at.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ql.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://wv.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://ws.newstarts.cn

deque(maxlen=10)
来源：http://we.szsharing.cn

[U14] Py：分组收集到列表
来源：http://vk.yuexingan06.cn

defaultdict(list)
来源：http://gx.newstarts.cn

[U15] Py：高精度计时
来源：http://rd.jctech888.com.cn

t = time.perf_counter()
来源：http://qo.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://jm.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://my.chemitech.net.cn

[U17] Py：初始化日志
来源：http://lz.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://el.521024.cn

[U18] Py：预编译正则
来源：http://eh.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://ol.hahajie.cn

[U19] Py：正则替换带回调
来源：http://ei.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eh.hahajie.cn

[U20] Py：缓存函数结果
来源：http://va.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://qk.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://bx.bjjhwx.cn

@contextlib.contextmanager
来源：http://js.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://ua.shtwfgs.cn

list(zip(*m))
来源：http://cz.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://qe.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vy.nszjky.cn

[U24] Py：路径操作
来源：http://hq.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://za.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://pw.bjjhwx.cn

csv.DictReader(f)
来源：http://dv.gzmigu.cn

[U26] Py：并发下载
来源：http://xh.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fb.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://tf.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://af.muxihuayi.cn

[U28] Py：类型别名
来源：http://ej.lnxyls.cn

UserId = int
来源：http://oo.hnjuh.cn

[U29] Py：属性校验
来源：http://wh.521024.cn

@property 与 @x.setter 配合
来源：http://py.521024.cn

[U30] Py：数据类
来源：http://me.colortex.cn

@dataclass(slots=True)
来源：http://rc.nicolike.cn

[U31] Py：单测
来源：http://bn.bookmarksfly.cn

python -m pytest -q
来源：http://zo.shtwfgs.cn

[U32] Py：代码格式化
来源：http://us.521024.cn

ruff format . && ruff check --fix .
来源：http://gd.shxzskj.cn

[U33] Py：打包发布
来源：http://vz.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://mb.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://kg.haigaiapp.cn

chardet.detect(raw)
来源：http://ms.hahajie.cn

[U35] Py：发送邮件
来源：http://tg.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ow.haigaiapp.cn

[U36] Py：定时任务
来源：http://il.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://sh.szxytkj.cn

[U37] Py：读写 Excel
来源：http://hw.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ae.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://ew.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://vx.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://nf.nszjky.cn

sys.stdout.isatty()
来源：http://cg.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://fl.szsharing.cn

print("err", file=sys.stderr)
来源：http://qo.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://rp.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gr.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://xx.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xa.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://aa.huanxung.cn

namespace App\Http;
来源：http://hb.hahajie.cn

[U44] PHP：开启严格类型
来源：http://ot.wgjwhj.cn

declare(strict_types=1);
来源：http://st.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://gr.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://op.szsharing.cn

[U46] PHP：可空类型
来源：http://hp.jianghongdianzi.cn

?string $name = null
来源：http://wr.panjiajie.cn

[U47] PHP：联合类型
来源：http://kr.lnxyls.cn

int|string $id
来源：http://nk.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://es.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qj.lnxyls.cn

[U49] PHP：只读属性
来源：http://uy.shxzskj.cn

public readonly string $name
来源：http://ki.colortex.cn

[U50] PHP：构造器属性提升
来源：http://uy.nszjky.cn

public function __construct(private int $id) {}
来源：http://pd.yuexingan06.cn

[U51] PHP：数组解构
来源：http://go.wgjwhj.cn

[$a, $b] = $arr;
来源：http://tl.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://as.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://ig.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://uc.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://jx.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://mv.szsharing.cn

$obj?->method()
来源：http://id.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://wa.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sb.shxzskj.cn

[U56] PHP：命名参数
来源：http://ll.yuexingan06.cn

f(a: 1, b: 2)
来源：http://vz.szxytkj.cn

[U57] PHP：字符串插值
来源：http://ju.newstarts.cn

"值: {$a}"
来源：http://oh.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://pt.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ir.panjiajie.cn


<!-- 参考信息 -->