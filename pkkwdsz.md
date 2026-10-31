代发 wailian999

[S33] C++：vector 增删
来源：http://xc.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uo.hahajie.cn

[S34] C++：遍历 vector
来源：http://om.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://jb.shxzskj.cn

[S35] C++：map
来源：http://ct.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fa.hnjuh.cn

[S36] C++：unordered_map
来源：http://vy.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ds.huixinmuqiang.cn

[S37] C++：set
来源：http://kg.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xg.colortex.cn

[S38] C++：排序
来源：http://iw.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://ij.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://za.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://db.yuexingan06.cn

[S40] C++：查找元素
来源：http://gj.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kk.colortex.cn

[S41] C++：类与构造函数
来源：http://jb.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bc.hahajie.cn

[S42] C++：继承与虚函数
来源：http://xd.521024.cn

class B : public Base { public: void f() override {} };
来源：http://zt.nicolike.cn

[S43] C++：智能指针
来源：http://na.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://bt.gzmigu.cn

[S44] C++：引用传参
来源：http://qz.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://yt.huixinmuqiang.cn

[S45] C++：lambda
来源：http://fl.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nl.9csxet.cn

[S46] C++：函数模板
来源：http://uo.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oz.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://hs.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aq.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://oa.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lp.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://rg.huixinmuqiang.cn

[S49] C++：写文件
来源：http://zc.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://us.newstarts.cn

[S50] C++：格式化数字
来源：http://wz.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ta.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://gm.gzmigu.cn

static_cast<double>(a) / b
来源：http://pd.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://nm.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://gt.asd995.cn

[S53] C++：移动语义
来源：http://mq.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://gh.yuexingan06.cn

[S54] C++：异常处理
来源：http://sk.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dz.panjiajie.cn

[S55] C++：结构化绑定
来源：http://uj.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zx.9csxet.cn

[S56] C++：optional
来源：http://jb.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eh.colortex.cn

[S57] C++：编译期常量
来源：http://rg.asd995.cn

constexpr int N = 10;
来源：http://vo.lnxyls.cn

[S58] C++：命名空间
来源：http://pb.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://ka.hnjuh.cn

[S59] C++：静态断言
来源：http://cz.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ap.asd995.cn

[S60] C++：遍历并删除元素
来源：http://uj.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xt.shxzskj.cn

================================================================================
来源：http://ch.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ju.muxihuayi.cn

================================================================================
来源：http://ye.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://lc.shxzukj.cn

println("Hello")
来源：http://hp.huixiangedu.cn

[T02] Kotlin：变量
来源：http://ev.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lj.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://zs.huixiangedu.cn

"值: $b"
来源：http://mu.nicolike.cn

[T04] Kotlin：空安全
来源：http://vm.hahajie.cn

val n: String? = null;  n?.length
来源：http://ph.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://wp.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lx.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://kk.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qa.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://ds.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://es.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://gc.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://fz.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://wv.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://vn.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://nr.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mg.huixiangedu.cn

[T11] Kotlin：协程
来源：http://od.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ip.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://lz.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://ei.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://ps.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://li.bjjhwx.cn

[T14] Kotlin：循环
来源：http://sl.9csxet.cn

for (i in 1..10) println(i)
来源：http://hi.nicolike.cn

[T15] Kotlin：接口
来源：http://rs.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://fv.shxzukj.cn

[T16] Swift：Hello World
来源：http://vv.bjjhwx.cn

print("Hello")
来源：http://rp.gzmigu.cn

[T17] Swift：变量与常量
来源：http://za.hahajie.cn

var a = 1;  let b = 2
来源：http://no.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://uy.huixinmuqiang.cn

"值: \(b)"
来源：http://jb.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://ql.shtwfgs.cn

if let n = opt { print(n) }
来源：http://wj.haigaiapp.cn

[T20] Swift：数组操作
来源：http://nn.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vb.asd995.cn

[T21] Swift：遍历
来源：http://xz.chemitech.net.cn

for x in a { print(x) }
来源：http://pc.hnjuh.cn

[T22] Swift：字典
来源：http://yr.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hq.521024.cn

[T23] Swift：函数
来源：http://uo.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rr.521024.cn

[T24] Swift：闭包
来源：http://cy.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gy.colortex.cn

[T25] Swift：结构体
来源：http://ra.muxihuayi.cn

struct P { var x: Int }
来源：http://hg.lnxyls.cn

[T26] Swift：类与重写
来源：http://rx.shxzskj.cn

class A: Base { override func f() {} }
来源：http://yi.szxytkj.cn

[T27] Swift：错误处理
来源：http://bo.521024.cn

do { try f() } catch { print(error) }
来源：http://wl.bjjhwx.cn

[T28] Swift：枚举
来源：http://bs.nicolike.cn

enum Color { case red, green }
来源：http://la.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://bj.muxihuayi.cn

guard let x = opt else { return }
来源：http://he.haigaiapp.cn

[T30] Swift：协议
来源：http://rz.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://ma.jctech888.com.cn

[T31] Lua：Hello World
来源：http://gs.jctech888.com.cn

print("Hello")
来源：http://ve.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://zc.huixinmuqiang.cn

local a = 1
来源：http://bx.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://ya.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jt.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://uo.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kj.9csxet.cn

[T35] Lua：字典表
来源：http://fb.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://rp.jctech888.com.cn

[T36] Lua：函数
来源：http://mr.jctech888.com.cn

function add(a, b) return a + b end
来源：http://je.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://lt.huanxung.cn

"a" .. "b"
来源：http://vp.huixinmuqiang.cn

[T38] Lua：条件
来源：http://ru.521024.cn

if x > 0 then print("正") end
来源：http://ha.asd995.cn

[T39] Lua：模式匹配
来源：http://yo.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://dl.newstarts.cn

[T40] Lua：元表
来源：http://wu.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://fr.chemitech.net.cn

[T41] Perl：Hello World
来源：http://im.szxytkj.cn

print "Hello\n";
来源：http://mu.nszjky.cn

[T42] Perl：变量类型
来源：http://xq.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qy.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://xr.jianghongdianzi.cn

"值: $a"
来源：http://ay.shxzskj.cn

[T44] Perl：条件
来源：http://uz.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://di.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://iw.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://vz.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://xo.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ys.shxzukj.cn

[T47] Perl：正则捕获
来源：http://zr.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fg.shxzukj.cn

[T48] Perl：正则替换
来源：http://pp.lnxyls.cn

$s =~ s/old/new/g;
来源：http://se.wgjwhj.cn

[T49] Perl：函数
来源：http://ao.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cv.newstarts.cn

[T50] Perl：逐行读文件
来源：http://bn.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://px.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://vf.gzmigu.cn

[T51] Scala：Hello World
来源：http://tg.gzmigu.cn

println("Hello")
来源：http://pb.jctech888.com.cn

[T52] Scala：变量
来源：http://ij.asd995.cn

val a = 1;  var b = 2
来源：http://va.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://et.huanxung.cn

s"值: $b"
来源：http://ak.gzmigu.cn

[T54] Scala：集合映射
来源：http://aq.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://hk.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://km.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ca.shtwfgs.cn

[T56] Scala：样例类
来源：http://yy.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://tk.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://cm.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mc.nszjky.cn

[T58] Scala：函数定义
来源：http://ra.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://je.yuexingan06.cn

[T59] Scala：循环
来源：http://pw.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://jr.colortex.cn

[T60] Scala：折叠
来源：http://ui.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jz.nszjky.cn

================================================================================
来源：http://bf.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://or.hahajie.cn

================================================================================
来源：http://ad.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://rt.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://en.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://nx.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dd.colortex.cn

[U03] Py：加载 .env 配置
来源：http://gp.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vv.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://mv.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sp.colortex.cn

[U05] Py：列表去重且保序
来源：http://bd.nicolike.cn

list(dict.fromkeys(arr))
来源：http://ww.shxzukj.cn

[U06] Py：合并两个字典
来源：http://if.newstarts.cn

{**a, **b}
来源：http://oh.colortex.cn

[U07] Py：反转字典键值
来源：http://zy.nicolike.cn

{v: k for k, v in d.items()}
来源：http://oa.hnjuh.cn

[U08] Py：展平二维列表
来源：http://fa.bjjhwx.cn

[y for x in nested for y in x]
来源：http://lz.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://vo.jianghongdianzi.cn

max(d, key=d.get)
来源：http://it.9csxet.cn

[U10] Py：按值排序字典
来源：http://gn.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ca.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://sk.colortex.cn

(x * 2 for x in arr)
来源：http://in.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yf.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://bu.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://js.lnxyls.cn

deque(maxlen=10)
来源：http://ji.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://an.panjiajie.cn

defaultdict(list)
来源：http://hd.lnxyls.cn

[U15] Py：高精度计时
来源：http://qh.muxihuayi.cn

t = time.perf_counter()
来源：http://cz.hahajie.cn

[U16] Py：命令行参数解析
来源：http://ub.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ak.lnxyls.cn

[U17] Py：初始化日志
来源：http://ts.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://rd.521024.cn

[U18] Py：预编译正则
来源：http://up.newstarts.cn

pat = re.compile(r"\d+")
来源：http://fy.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://wn.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zx.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://ls.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://rb.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://bn.9csxet.cn

@contextlib.contextmanager
来源：http://rj.9csxet.cn

[U22] Py：矩阵转置
来源：http://se.asd995.cn

list(zip(*m))
来源：http://nx.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://ug.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fk.yuexingan06.cn

[U24] Py：路径操作
来源：http://cz.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cs.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://ev.nicolike.cn

csv.DictReader(f)
来源：http://vc.muxihuayi.cn

[U26] Py：并发下载
来源：http://do.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ft.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://mc.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://jh.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://jr.newstarts.cn

UserId = int
来源：http://ra.szsharing.cn

[U29] Py：属性校验
来源：http://ia.9csxet.cn

@property 与 @x.setter 配合
来源：http://ay.huanxung.cn

[U30] Py：数据类
来源：http://nj.521024.cn

@dataclass(slots=True)
来源：http://yj.haigaiapp.cn

[U31] Py：单测
来源：http://ux.szsharing.cn

python -m pytest -q
来源：http://xs.lnxyls.cn

[U32] Py：代码格式化
来源：http://fm.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://pq.huanxung.cn

[U33] Py：打包发布
来源：http://ix.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://oy.bookmarksfly.cn

[U34] Py：判断编码
来源：http://zq.lnxyls.cn

chardet.detect(raw)
来源：http://jr.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://kf.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hj.bjjhwx.cn

[U36] Py：定时任务
来源：http://qe.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://es.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://xl.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jd.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://xe.colortex.cn

Path(__file__).resolve().parent
来源：http://ey.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://hk.yuexingan06.cn

sys.stdout.isatty()
来源：http://av.nszjky.cn

[U40] Py：打印到标准错误
来源：http://tv.nicolike.cn

print("err", file=sys.stderr)
来源：http://mm.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://uz.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hy.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://mv.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dt.newstarts.cn

[U43] PHP：声明命名空间
来源：http://px.colortex.cn

namespace App\Http;
来源：http://gg.hahajie.cn

[U44] PHP：开启严格类型
来源：http://se.nicolike.cn

declare(strict_types=1);
来源：http://ya.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://nn.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bh.bjjhwx.cn

[U46] PHP：可空类型
来源：http://tq.shxzskj.cn

?string $name = null
来源：http://zo.szsharing.cn

[U47] PHP：联合类型
来源：http://sc.gzmigu.cn

int|string $id
来源：http://ay.huanxung.cn

[U48] PHP：纯枚举
来源：http://sv.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jb.wgjwhj.cn

[U49] PHP：只读属性
来源：http://kk.shxzskj.cn

public readonly string $name
来源：http://pm.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://cb.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://ih.huanxung.cn

[U51] PHP：数组解构
来源：http://cv.hnjuh.cn

[$a, $b] = $arr;
来源：http://ob.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://yf.521024.cn

$double = fn($x) => $x * 2;
来源：http://mu.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://qd.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://vf.szsharing.cn

[U54] PHP：空安全调用
来源：http://hs.yuexingan06.cn

$obj?->method()
来源：http://qt.521024.cn

[U55] PHP：match 表达式
来源：http://dy.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kb.panjiajie.cn

[U56] PHP：命名参数
来源：http://ai.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://sf.chemitech.net.cn

[U57] PHP：字符串插值
来源：http://kq.yuntaijiaju.cn

"值: {$a}"
来源：http://we.colortex.cn

[U58] PHP：数组三件套
来源：http://ap.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pl.521024.cn


<!-- 参考信息 -->