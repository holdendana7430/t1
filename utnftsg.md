代发 wailian999

[S35] C++：map
来源：http://nl.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dz.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://kz.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ud.huanxung.cn

[S37] C++：set
来源：http://fw.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gl.nszjky.cn

[S38] C++：排序
来源：http://un.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://uj.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://fk.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://na.szxytkj.cn

[S40] C++：查找元素
来源：http://kq.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jp.colortex.cn

[S41] C++：类与构造函数
来源：http://io.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://le.9csxet.cn

[S42] C++：继承与虚函数
来源：http://ry.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://da.szsharing.cn

[S43] C++：智能指针
来源：http://sw.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://zc.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://md.asd995.cn

void inc(int &x) { ++x; }
来源：http://kz.9csxet.cn

[S45] C++：lambda
来源：http://mu.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fd.huixiangedu.cn

[S46] C++：函数模板
来源：http://ox.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ti.521024.cn

[S47] C++：结构化绑定遍历
来源：http://hi.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kc.shxzukj.cn

[S48] C++：逐行读文件
来源：http://yi.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hn.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://uk.bjjhwx.cn

[S49] C++：写文件
来源：http://ra.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qb.9csxet.cn

[S50] C++：格式化数字
来源：http://lc.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lb.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://wg.chemitech.net.cn

static_cast<double>(a) / b
来源：http://kk.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://xd.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://nw.muxihuayi.cn

[S53] C++：移动语义
来源：http://oq.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://gy.521024.cn

[S54] C++：异常处理
来源：http://wm.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ez.nicolike.cn

[S55] C++：结构化绑定
来源：http://ei.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://in.lnxyls.cn

[S56] C++：optional
来源：http://on.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yq.hnjuh.cn

[S57] C++：编译期常量
来源：http://yq.haigaiapp.cn

constexpr int N = 10;
来源：http://fo.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://wy.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://tf.nicolike.cn

[S59] C++：静态断言
来源：http://gk.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ft.colortex.cn

[S60] C++：遍历并删除元素
来源：http://el.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dz.wgjwhj.cn

================================================================================
来源：http://hk.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ud.jctech888.com.cn

================================================================================
来源：http://pn.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://ah.shxzukj.cn

println("Hello")
来源：http://na.newstarts.cn

[T02] Kotlin：变量
来源：http://xp.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oz.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://wd.shxzskj.cn

"值: $b"
来源：http://pd.newstarts.cn

[T04] Kotlin：空安全
来源：http://qi.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://se.asd995.cn

[T05] Kotlin：when 表达式
来源：http://zp.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gx.szsharing.cn

[T06] Kotlin：集合映射
来源：http://vn.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://by.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://jk.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tv.szxytkj.cn

[T08] Kotlin：数据类
来源：http://bl.asd995.cn

data class User(val name: String, val age: Int)
来源：http://bp.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://iw.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://ae.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://jc.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vo.haigaiapp.cn

[T11] Kotlin：协程
来源：http://qj.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lb.szsharing.cn

[T12] Kotlin：解构声明
来源：http://fn.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://kx.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://vl.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://eq.haigaiapp.cn

[T14] Kotlin：循环
来源：http://lr.szxytkj.cn

for (i in 1..10) println(i)
来源：http://uy.asd995.cn

[T15] Kotlin：接口
来源：http://yo.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://ey.nszjky.cn

[T16] Swift：Hello World
来源：http://sl.hahajie.cn

print("Hello")
来源：http://ng.gzmigu.cn

[T17] Swift：变量与常量
来源：http://jo.9csxet.cn

var a = 1;  let b = 2
来源：http://nb.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://zd.bookmarksfly.cn

"值: \(b)"
来源：http://hk.9csxet.cn

[T19] Swift：可选绑定
来源：http://fr.huixiangedu.cn

if let n = opt { print(n) }
来源：http://px.huanxung.cn

[T20] Swift：数组操作
来源：http://em.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ax.nicolike.cn

[T21] Swift：遍历
来源：http://no.521024.cn

for x in a { print(x) }
来源：http://av.szxytkj.cn

[T22] Swift：字典
来源：http://gs.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qe.huixinmuqiang.cn

[T23] Swift：函数
来源：http://xl.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gy.chemitech.net.cn

[T24] Swift：闭包
来源：http://ke.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://od.hnjuh.cn

[T25] Swift：结构体
来源：http://zi.yuexingan06.cn

struct P { var x: Int }
来源：http://rx.bjjhwx.cn

[T26] Swift：类与重写
来源：http://tr.hnjuh.cn

class A: Base { override func f() {} }
来源：http://ii.szxytkj.cn

[T27] Swift：错误处理
来源：http://ia.nicolike.cn

do { try f() } catch { print(error) }
来源：http://qe.huixiangedu.cn

[T28] Swift：枚举
来源：http://wn.chemitech.net.cn

enum Color { case red, green }
来源：http://id.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://bt.szxytkj.cn

guard let x = opt else { return }
来源：http://cj.yuntaijiaju.cn

[T30] Swift：协议
来源：http://yi.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://ic.nszjky.cn

[T31] Lua：Hello World
来源：http://uf.wgjwhj.cn

print("Hello")
来源：http://ke.szxytkj.cn

[T32] Lua：局部变量
来源：http://lt.huixiangedu.cn

local a = 1
来源：http://xf.9csxet.cn

[T33] Lua：表（数组）
来源：http://af.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ki.nszjky.cn

[T34] Lua：遍历表
来源：http://ly.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ba.newstarts.cn

[T35] Lua：字典表
来源：http://pn.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://nn.jctech888.com.cn

[T36] Lua：函数
来源：http://jj.panjiajie.cn

function add(a, b) return a + b end
来源：http://fa.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://lm.panjiajie.cn

"a" .. "b"
来源：http://nz.szsharing.cn

[T38] Lua：条件
来源：http://qt.chemitech.net.cn

if x > 0 then print("正") end
来源：http://rf.hnjuh.cn

[T39] Lua：模式匹配
来源：http://uk.bookmarksfly.cn

string.find(s, "%d+")
来源：http://xe.shtwfgs.cn

[T40] Lua：元表
来源：http://fr.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://gj.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://no.hnjuh.cn

print "Hello\n";
来源：http://wp.521024.cn

[T42] Perl：变量类型
来源：http://cz.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bt.newstarts.cn

[T43] Perl：字符串插值
来源：http://bh.9csxet.cn

"值: $a"
来源：http://jm.shtwfgs.cn

[T44] Perl：条件
来源：http://kk.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://an.hnjuh.cn

[T45] Perl：数组遍历
来源：http://vo.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://ks.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://wy.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://un.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://fq.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nf.haigaiapp.cn

[T48] Perl：正则替换
来源：http://wc.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://bp.9csxet.cn

[T49] Perl：函数
来源：http://pe.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bc.huixiangedu.cn

[T50] Perl：逐行读文件
来源：http://sn.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cy.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://gb.huanxung.cn

[T51] Scala：Hello World
来源：http://ik.9csxet.cn

println("Hello")
来源：http://up.szxytkj.cn

[T52] Scala：变量
来源：http://bg.gzmigu.cn

val a = 1;  var b = 2
来源：http://cd.gzmigu.cn

[T53] Scala：字符串插值
来源：http://ic.jianghongdianzi.cn

s"值: $b"
来源：http://dn.panjiajie.cn

[T54] Scala：集合映射
来源：http://tf.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://jd.gzmigu.cn

[T55] Scala：集合过滤
来源：http://fi.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ga.hnjuh.cn

[T56] Scala：样例类
来源：http://cd.9csxet.cn

case class User(name: String, age: Int)
来源：http://sa.shxzukj.cn

[T57] Scala：模式匹配
来源：http://ak.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vx.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://hh.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wc.muxihuayi.cn

[T59] Scala：循环
来源：http://dl.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://hi.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://ms.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ds.shxzskj.cn

================================================================================
来源：http://wo.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hf.huixiangedu.cn

================================================================================
来源：http://jp.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://vv.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vj.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://tj.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://up.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://uu.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pj.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://vp.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mr.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://io.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://yn.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://oy.szxytkj.cn

{**a, **b}
来源：http://yx.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://yr.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://vp.huanxung.cn

[U08] Py：展平二维列表
来源：http://fl.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://hb.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://cn.shxzskj.cn

max(d, key=d.get)
来源：http://sr.nszjky.cn

[U10] Py：按值排序字典
来源：http://iw.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ie.gzmigu.cn

[U11] Py：生成器表达式
来源：http://yy.shtwfgs.cn

(x * 2 for x in arr)
来源：http://cs.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lu.shxzskj.cn

Counter(arr).most_common(3)
来源：http://uq.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://vf.colortex.cn

deque(maxlen=10)
来源：http://sc.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://pd.panjiajie.cn

defaultdict(list)
来源：http://vm.colortex.cn

[U15] Py：高精度计时
来源：http://ln.huixiangedu.cn

t = time.perf_counter()
来源：http://ro.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://cb.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yb.yuexingan06.cn

[U17] Py：初始化日志
来源：http://vm.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://ib.hnjuh.cn

[U18] Py：预编译正则
来源：http://fi.huanxung.cn

pat = re.compile(r"\d+")
来源：http://kr.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://wb.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ni.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://zr.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://cg.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://gy.9csxet.cn

@contextlib.contextmanager
来源：http://et.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://ai.wgjwhj.cn

list(zip(*m))
来源：http://lo.shxzskj.cn

[U23] Py：分块读取大文件
来源：http://cx.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nq.colortex.cn

[U24] Py：路径操作
来源：http://kw.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kz.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://ty.yuntaijiaju.cn

csv.DictReader(f)
来源：http://hl.newstarts.cn

[U26] Py：并发下载
来源：http://fr.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bm.asd995.cn

[U27] Py：异步 HTTP
来源：http://vq.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://qh.hahajie.cn

[U28] Py：类型别名
来源：http://gr.colortex.cn

UserId = int
来源：http://um.bjjhwx.cn

[U29] Py：属性校验
来源：http://ym.szsharing.cn

@property 与 @x.setter 配合
来源：http://vl.jianghongdianzi.cn

[U30] Py：数据类
来源：http://bh.lnxyls.cn

@dataclass(slots=True)
来源：http://sb.jianghongdianzi.cn

[U31] Py：单测
来源：http://sm.jianghongdianzi.cn

python -m pytest -q
来源：http://rr.huixiangedu.cn

[U32] Py：代码格式化
来源：http://bc.szsharing.cn

ruff format . && ruff check --fix .
来源：http://jz.haigaiapp.cn

[U33] Py：打包发布
来源：http://vz.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://jc.jctech888.com.cn

[U34] Py：判断编码
来源：http://pv.hahajie.cn

chardet.detect(raw)
来源：http://if.haigaiapp.cn

[U35] Py：发送邮件
来源：http://kx.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://na.muxihuayi.cn

[U36] Py：定时任务
来源：http://ww.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://ch.hnjuh.cn

[U37] Py：读写 Excel
来源：http://ix.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fe.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://gm.lnxyls.cn

Path(__file__).resolve().parent
来源：http://rd.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://bu.shxzskj.cn

sys.stdout.isatty()
来源：http://rh.nszjky.cn

[U40] Py：打印到标准错误
来源：http://ht.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://ix.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://qr.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bu.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://pt.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bf.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://bh.colortex.cn

namespace App\Http;
来源：http://ga.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://mf.gzmigu.cn

declare(strict_types=1);
来源：http://oj.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://px.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ab.9csxet.cn

[U46] PHP：可空类型
来源：http://ik.haigaiapp.cn

?string $name = null
来源：http://yf.shxzukj.cn

[U47] PHP：联合类型
来源：http://ac.panjiajie.cn

int|string $id
来源：http://yj.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://lv.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nj.muxihuayi.cn

[U49] PHP：只读属性
来源：http://xl.asd995.cn

public readonly string $name
来源：http://xt.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://yy.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://fe.yuexingan06.cn

[U51] PHP：数组解构
来源：http://tg.9csxet.cn

[$a, $b] = $arr;
来源：http://kv.9csxet.cn

[U52] PHP：箭头函数
来源：http://rz.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://ig.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://ty.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://zq.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://nw.asd995.cn

$obj?->method()
来源：http://sk.nicolike.cn

[U55] PHP：match 表达式
来源：http://ql.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cy.chemitech.net.cn

[U56] PHP：命名参数
来源：http://rb.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://ud.asd995.cn

[U57] PHP：字符串插值
来源：http://pz.9csxet.cn

"值: {$a}"
来源：http://da.szsharing.cn

[U58] PHP：数组三件套
来源：http://yk.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xt.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://ax.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ao.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://gv.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://di.gzmigu.cn


<!-- 参考信息 -->