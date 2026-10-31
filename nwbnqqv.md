代发 wailian999

[S43] C++：智能指针
来源：http://vx.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://pj.yuexingan06.cn

[S44] C++：引用传参
来源：http://wu.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://es.panjiajie.cn

[S45] C++：lambda
来源：http://iz.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sk.hnjuh.cn

[S46] C++：函数模板
来源：http://es.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jq.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://fq.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ze.colortex.cn

[S48] C++：逐行读文件
来源：http://kf.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zb.nicolike.cn

while (std::getline(in, line)) { }
来源：http://ab.bjjhwx.cn

[S49] C++：写文件
来源：http://cn.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dg.hnjuh.cn

[S50] C++：格式化数字
来源：http://tm.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gt.hnjuh.cn

[S51] C++：显式类型转换
来源：http://md.chemitech.net.cn

static_cast<double>(a) / b
来源：http://qy.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://zx.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://ml.huixiangedu.cn

[S53] C++：移动语义
来源：http://yx.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://ti.wgjwhj.cn

[S54] C++：异常处理
来源：http://ol.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yl.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://oi.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nf.nicolike.cn

[S56] C++：optional
来源：http://bj.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ey.hnjuh.cn

[S57] C++：编译期常量
来源：http://fy.gzmigu.cn

constexpr int N = 10;
来源：http://ab.lnxyls.cn

[S58] C++：命名空间
来源：http://kp.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://px.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://uh.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zn.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://ee.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://up.nszjky.cn

================================================================================
来源：http://gh.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bn.huixinmuqiang.cn

================================================================================
来源：http://us.szsharing.cn

[T01] Kotlin：Hello World
来源：http://md.bjjhwx.cn

println("Hello")
来源：http://hi.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://ms.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://md.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://qh.gzmigu.cn

"值: $b"
来源：http://ue.szsharing.cn

[T04] Kotlin：空安全
来源：http://ga.hahajie.cn

val n: String? = null;  n?.length
来源：http://fy.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://qs.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xw.521024.cn

[T06] Kotlin：集合映射
来源：http://fb.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fi.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://us.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gm.lnxyls.cn

[T08] Kotlin：数据类
来源：http://la.asd995.cn

data class User(val name: String, val age: Int)
来源：http://mh.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://kf.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://rq.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://bz.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ze.hnjuh.cn

[T11] Kotlin：协程
来源：http://jq.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://br.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://px.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://cx.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://tf.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://dg.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://hh.9csxet.cn

for (i in 1..10) println(i)
来源：http://jn.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://px.colortex.cn

interface Shape { fun area(): Double }
来源：http://en.shtwfgs.cn

[T16] Swift：Hello World
来源：http://zn.nicolike.cn

print("Hello")
来源：http://fj.newstarts.cn

[T17] Swift：变量与常量
来源：http://cy.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://cl.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://xx.huixiangedu.cn

"值: \(b)"
来源：http://ki.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://pe.jctech888.com.cn

if let n = opt { print(n) }
来源：http://po.521024.cn

[T20] Swift：数组操作
来源：http://lz.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jq.yuexingan06.cn

[T21] Swift：遍历
来源：http://qf.yuexingan06.cn

for x in a { print(x) }
来源：http://fe.huixinmuqiang.cn

[T22] Swift：字典
来源：http://oz.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yn.wgjwhj.cn

[T23] Swift：函数
来源：http://xd.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hs.yuexingan06.cn

[T24] Swift：闭包
来源：http://cj.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xl.asd995.cn

[T25] Swift：结构体
来源：http://sx.asd995.cn

struct P { var x: Int }
来源：http://eu.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://yl.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://zy.shxzukj.cn

[T27] Swift：错误处理
来源：http://gd.9csxet.cn

do { try f() } catch { print(error) }
来源：http://be.bookmarksfly.cn

[T28] Swift：枚举
来源：http://eq.yuexingan06.cn

enum Color { case red, green }
来源：http://nb.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://gq.hahajie.cn

guard let x = opt else { return }
来源：http://sl.9csxet.cn

[T30] Swift：协议
来源：http://ds.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://ah.bjjhwx.cn

[T31] Lua：Hello World
来源：http://ee.bookmarksfly.cn

print("Hello")
来源：http://bt.panjiajie.cn

[T32] Lua：局部变量
来源：http://eg.hnjuh.cn

local a = 1
来源：http://lg.huanxung.cn

[T33] Lua：表（数组）
来源：http://zz.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bh.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://yg.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://aj.szxytkj.cn

[T35] Lua：字典表
来源：http://us.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://xv.huanxung.cn

[T36] Lua：函数
来源：http://ra.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://dz.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://kg.yuntaijiaju.cn

"a" .. "b"
来源：http://ul.asd995.cn

[T38] Lua：条件
来源：http://lm.wgjwhj.cn

if x > 0 then print("正") end
来源：http://po.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://bh.panjiajie.cn

string.find(s, "%d+")
来源：http://wj.9csxet.cn

[T40] Lua：元表
来源：http://lb.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://rv.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://at.shxzskj.cn

print "Hello\n";
来源：http://lk.gzmigu.cn

[T42] Perl：变量类型
来源：http://tp.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qt.521024.cn

[T43] Perl：字符串插值
来源：http://lr.9csxet.cn

"值: $a"
来源：http://ti.gzmigu.cn

[T44] Perl：条件
来源：http://ry.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://vf.9csxet.cn

[T45] Perl：数组遍历
来源：http://of.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://ab.shxzukj.cn

[T46] Perl：哈希操作
来源：http://lx.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://md.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://lo.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sj.nicolike.cn

[T48] Perl：正则替换
来源：http://vw.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://cq.wgjwhj.cn

[T49] Perl：函数
来源：http://za.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vs.newstarts.cn

[T50] Perl：逐行读文件
来源：http://tn.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rr.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://od.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://gr.nszjky.cn

println("Hello")
来源：http://pg.newstarts.cn

[T52] Scala：变量
来源：http://wc.chemitech.net.cn

val a = 1;  var b = 2
来源：http://pb.hnjuh.cn

[T53] Scala：字符串插值
来源：http://oq.521024.cn

s"值: $b"
来源：http://ez.huanxung.cn

[T54] Scala：集合映射
来源：http://bh.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://zk.colortex.cn

[T55] Scala：集合过滤
来源：http://ih.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fz.szsharing.cn

[T56] Scala：样例类
来源：http://br.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://pi.hnjuh.cn

[T57] Scala：模式匹配
来源：http://yy.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wm.lnxyls.cn

[T58] Scala：函数定义
来源：http://qg.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rw.gzmigu.cn

[T59] Scala：循环
来源：http://yy.521024.cn

for (i <- 1 to 10) println(i)
来源：http://qo.hahajie.cn

[T60] Scala：折叠
来源：http://ff.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nh.huanxung.cn

================================================================================
来源：http://wu.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fy.hahajie.cn

================================================================================
来源：http://ln.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://xs.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sh.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://sx.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dv.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://xg.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qz.szsharing.cn

[U04] Py：变量调试打印
来源：http://as.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ed.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://sg.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://qm.gzmigu.cn

[U06] Py：合并两个字典
来源：http://xj.lnxyls.cn

{**a, **b}
来源：http://gk.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://nq.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://bs.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://xx.newstarts.cn

[y for x in nested for y in x]
来源：http://sf.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://pb.9csxet.cn

max(d, key=d.get)
来源：http://qz.shxzukj.cn

[U10] Py：按值排序字典
来源：http://pq.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ex.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://so.haigaiapp.cn

(x * 2 for x in arr)
来源：http://pk.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lo.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://wg.newstarts.cn

[U13] Py：固定长度队列
来源：http://kx.lnxyls.cn

deque(maxlen=10)
来源：http://ke.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://fd.colortex.cn

defaultdict(list)
来源：http://pr.nicolike.cn

[U15] Py：高精度计时
来源：http://cg.shtwfgs.cn

t = time.perf_counter()
来源：http://jp.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://gy.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cc.newstarts.cn

[U17] Py：初始化日志
来源：http://rc.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://ms.szxytkj.cn

[U18] Py：预编译正则
来源：http://gm.newstarts.cn

pat = re.compile(r"\d+")
来源：http://jz.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://ft.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dc.9csxet.cn

[U20] Py：缓存函数结果
来源：http://cb.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://ct.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://go.huanxung.cn

@contextlib.contextmanager
来源：http://ga.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://ts.yuexingan06.cn

list(zip(*m))
来源：http://vo.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://ha.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ww.jctech888.com.cn

[U24] Py：路径操作
来源：http://zu.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vy.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://po.jctech888.com.cn

csv.DictReader(f)
来源：http://wr.yuexingan06.cn

[U26] Py：并发下载
来源：http://bw.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bj.hahajie.cn

[U27] Py：异步 HTTP
来源：http://pm.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://wx.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://aw.huixiangedu.cn

UserId = int
来源：http://aj.hnjuh.cn

[U29] Py：属性校验
来源：http://kl.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://ov.bookmarksfly.cn

[U30] Py：数据类
来源：http://cs.colortex.cn

@dataclass(slots=True)
来源：http://od.huixinmuqiang.cn

[U31] Py：单测
来源：http://ge.hnjuh.cn

python -m pytest -q
来源：http://oz.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://jj.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://dp.wgjwhj.cn

[U33] Py：打包发布
来源：http://fk.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://fa.huixiangedu.cn

[U34] Py：判断编码
来源：http://zx.wgjwhj.cn

chardet.detect(raw)
来源：http://hr.nszjky.cn

[U35] Py：发送邮件
来源：http://xp.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rd.shxzukj.cn

[U36] Py：定时任务
来源：http://jb.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://zy.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://iz.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tq.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://pt.9csxet.cn

Path(__file__).resolve().parent
来源：http://vg.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://bq.colortex.cn

sys.stdout.isatty()
来源：http://rt.hahajie.cn

[U40] Py：打印到标准错误
来源：http://kg.shxzukj.cn

print("err", file=sys.stderr)
来源：http://bk.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://wx.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gv.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://dw.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sl.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://md.colortex.cn

namespace App\Http;
来源：http://sn.521024.cn

[U44] PHP：开启严格类型
来源：http://ix.shxzukj.cn

declare(strict_types=1);
来源：http://ua.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://yc.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bm.newstarts.cn

[U46] PHP：可空类型
来源：http://gt.shxzukj.cn

?string $name = null
来源：http://ke.hnjuh.cn

[U47] PHP：联合类型
来源：http://pm.yuntaijiaju.cn

int|string $id
来源：http://br.shxzskj.cn

[U48] PHP：纯枚举
来源：http://wn.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zp.521024.cn

[U49] PHP：只读属性
来源：http://no.yuntaijiaju.cn

public readonly string $name
来源：http://kp.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://mo.gzmigu.cn

public function __construct(private int $id) {}
来源：http://re.hnjuh.cn

[U51] PHP：数组解构
来源：http://lb.shxzskj.cn

[$a, $b] = $arr;
来源：http://zs.panjiajie.cn

[U52] PHP：箭头函数
来源：http://vu.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://gn.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://fl.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://ny.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://lq.huixinmuqiang.cn

$obj?->method()
来源：http://fs.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://sb.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fz.hahajie.cn

[U56] PHP：命名参数
来源：http://ts.szxytkj.cn

f(a: 1, b: 2)
来源：http://jq.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://su.lnxyls.cn

"值: {$a}"
来源：http://ec.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://ef.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pm.hnjuh.cn

[U59] PHP：自定义排序
来源：http://im.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sf.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://jb.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hc.newstarts.cn

[U61] PHP：正则
来源：http://po.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mu.panjiajie.cn

[U62] PHP：日期对象
来源：http://nv.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ov.szxytkj.cn

[U63] PHP：文件读写
来源：http://xr.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uw.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://mn.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://fg.gzmigu.cn

[U65] PHP：会话
来源：http://ul.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pv.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://iv.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iu.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://gv.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://og.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://mi.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aa.yuexingan06.cn


<!-- 参考信息 -->