代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://bj.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vc.szxytkj.cn

[S48] C++：逐行读文件
来源：http://ao.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://os.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://hy.huixiangedu.cn

[S49] C++：写文件
来源：http://jp.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ae.szsharing.cn

[S50] C++：格式化数字
来源：http://wj.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aa.nicolike.cn

[S51] C++：显式类型转换
来源：http://hx.muxihuayi.cn

static_cast<double>(a) / b
来源：http://gv.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://ex.asd995.cn

int size() const noexcept { return n_; }
来源：http://mh.huixiangedu.cn

[S53] C++：移动语义
来源：http://nm.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://wk.hahajie.cn

[S54] C++：异常处理
来源：http://tc.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bf.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://me.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rf.asd995.cn

[S56] C++：optional
来源：http://fj.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ij.nszjky.cn

[S57] C++：编译期常量
来源：http://vq.nicolike.cn

constexpr int N = 10;
来源：http://ir.shtwfgs.cn

[S58] C++：命名空间
来源：http://tr.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://yk.yuntaijiaju.cn

[S59] C++：静态断言
来源：http://hc.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://im.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://ef.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tp.gzmigu.cn

================================================================================
来源：http://bw.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://la.szxytkj.cn

================================================================================
来源：http://fy.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://tc.jianghongdianzi.cn

println("Hello")
来源：http://gy.521024.cn

[T02] Kotlin：变量
来源：http://gc.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nu.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://bz.jianghongdianzi.cn

"值: $b"
来源：http://ec.521024.cn

[T04] Kotlin：空安全
来源：http://rz.nszjky.cn

val n: String? = null;  n?.length
来源：http://xc.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://ll.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jl.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://qy.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hm.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://hp.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://po.gzmigu.cn

[T08] Kotlin：数据类
来源：http://uc.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://yl.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://en.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://kc.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://ft.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://en.bjjhwx.cn

[T11] Kotlin：协程
来源：http://mt.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lt.huanxung.cn

[T12] Kotlin：解构声明
来源：http://yo.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://gr.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://yl.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://uc.hnjuh.cn

[T14] Kotlin：循环
来源：http://dk.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://qf.jctech888.com.cn

[T15] Kotlin：接口
来源：http://ob.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://yj.huixiangedu.cn

[T16] Swift：Hello World
来源：http://uv.haigaiapp.cn

print("Hello")
来源：http://rb.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://ey.asd995.cn

var a = 1;  let b = 2
来源：http://ix.nicolike.cn

[T18] Swift：字符串插值
来源：http://sg.panjiajie.cn

"值: \(b)"
来源：http://bz.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://ku.asd995.cn

if let n = opt { print(n) }
来源：http://et.newstarts.cn

[T20] Swift：数组操作
来源：http://jd.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uq.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://st.nszjky.cn

for x in a { print(x) }
来源：http://fv.gzmigu.cn

[T22] Swift：字典
来源：http://sw.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://et.shxzskj.cn

[T23] Swift：函数
来源：http://ko.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://is.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://ir.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yz.nszjky.cn

[T25] Swift：结构体
来源：http://yr.9csxet.cn

struct P { var x: Int }
来源：http://oz.muxihuayi.cn

[T26] Swift：类与重写
来源：http://ea.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://cw.chemitech.net.cn

[T27] Swift：错误处理
来源：http://bi.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://ct.huanxung.cn

[T28] Swift：枚举
来源：http://ek.nicolike.cn

enum Color { case red, green }
来源：http://ub.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://jb.asd995.cn

guard let x = opt else { return }
来源：http://ti.hahajie.cn

[T30] Swift：协议
来源：http://ty.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://br.hahajie.cn

[T31] Lua：Hello World
来源：http://xx.haigaiapp.cn

print("Hello")
来源：http://bf.gzmigu.cn

[T32] Lua：局部变量
来源：http://ww.wgjwhj.cn

local a = 1
来源：http://fi.lnxyls.cn

[T33] Lua：表（数组）
来源：http://zb.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jt.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://jq.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vn.haigaiapp.cn

[T35] Lua：字典表
来源：http://iy.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://kf.colortex.cn

[T36] Lua：函数
来源：http://mm.jctech888.com.cn

function add(a, b) return a + b end
来源：http://xa.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://tf.shxzskj.cn

"a" .. "b"
来源：http://jy.bjjhwx.cn

[T38] Lua：条件
来源：http://su.szxytkj.cn

if x > 0 then print("正") end
来源：http://bc.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://va.521024.cn

string.find(s, "%d+")
来源：http://cz.colortex.cn

[T40] Lua：元表
来源：http://of.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://aw.nszjky.cn

[T41] Perl：Hello World
来源：http://le.muxihuayi.cn

print "Hello\n";
来源：http://mh.szsharing.cn

[T42] Perl：变量类型
来源：http://bx.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yc.nicolike.cn

[T43] Perl：字符串插值
来源：http://ua.haigaiapp.cn

"值: $a"
来源：http://jq.chemitech.net.cn

[T44] Perl：条件
来源：http://st.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://mt.colortex.cn

[T45] Perl：数组遍历
来源：http://ms.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://xl.nszjky.cn

[T46] Perl：哈希操作
来源：http://iy.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jv.huanxung.cn

[T47] Perl：正则捕获
来源：http://st.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://df.9csxet.cn

[T48] Perl：正则替换
来源：http://iv.9csxet.cn

$s =~ s/old/new/g;
来源：http://sg.szsharing.cn

[T49] Perl：函数
来源：http://xk.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zn.521024.cn

[T50] Perl：逐行读文件
来源：http://fq.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://np.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://kw.muxihuayi.cn

[T51] Scala：Hello World
来源：http://xw.colortex.cn

println("Hello")
来源：http://xo.jianghongdianzi.cn

[T52] Scala：变量
来源：http://dl.bjjhwx.cn

val a = 1;  var b = 2
来源：http://nw.shxzskj.cn

[T53] Scala：字符串插值
来源：http://xb.gzmigu.cn

s"值: $b"
来源：http://wi.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://zr.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://mg.lnxyls.cn

[T55] Scala：集合过滤
来源：http://zq.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xr.gzmigu.cn

[T56] Scala：样例类
来源：http://aj.huanxung.cn

case class User(name: String, age: Int)
来源：http://wx.hahajie.cn

[T57] Scala：模式匹配
来源：http://fr.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lf.chemitech.net.cn

[T58] Scala：函数定义
来源：http://un.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sg.chemitech.net.cn

[T59] Scala：循环
来源：http://rn.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://jj.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://ta.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uf.shtwfgs.cn

================================================================================
来源：http://qk.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iz.lnxyls.cn

================================================================================
来源：http://xx.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://hp.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hk.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://py.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bl.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://re.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ck.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://wq.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vu.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://og.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://pl.szsharing.cn

[U06] Py：合并两个字典
来源：http://dk.lnxyls.cn

{**a, **b}
来源：http://li.huanxung.cn

[U07] Py：反转字典键值
来源：http://hn.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://pe.hnjuh.cn

[U08] Py：展平二维列表
来源：http://zt.shtwfgs.cn

[y for x in nested for y in x]
来源：http://im.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://tr.panjiajie.cn

max(d, key=d.get)
来源：http://or.shxzskj.cn

[U10] Py：按值排序字典
来源：http://xu.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jb.gzmigu.cn

[U11] Py：生成器表达式
来源：http://pp.gzmigu.cn

(x * 2 for x in arr)
来源：http://mx.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cy.panjiajie.cn

Counter(arr).most_common(3)
来源：http://hb.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://bo.yuntaijiaju.cn

deque(maxlen=10)
来源：http://ue.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://cs.huanxung.cn

defaultdict(list)
来源：http://hp.szsharing.cn

[U15] Py：高精度计时
来源：http://we.lnxyls.cn

t = time.perf_counter()
来源：http://kn.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://pc.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ws.nicolike.cn

[U17] Py：初始化日志
来源：http://bg.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://af.shtwfgs.cn

[U18] Py：预编译正则
来源：http://lw.newstarts.cn

pat = re.compile(r"\d+")
来源：http://yj.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://ze.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ry.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://ye.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://lw.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://gm.huixiangedu.cn

@contextlib.contextmanager
来源：http://fb.nicolike.cn

[U22] Py：矩阵转置
来源：http://ku.huixinmuqiang.cn

list(zip(*m))
来源：http://od.nszjky.cn

[U23] Py：分块读取大文件
来源：http://wc.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ql.nszjky.cn

[U24] Py：路径操作
来源：http://im.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://an.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://vy.wgjwhj.cn

csv.DictReader(f)
来源：http://co.hnjuh.cn

[U26] Py：并发下载
来源：http://rx.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tn.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://hu.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://xl.szsharing.cn

[U28] Py：类型别名
来源：http://lk.muxihuayi.cn

UserId = int
来源：http://xe.asd995.cn

[U29] Py：属性校验
来源：http://ls.shxzskj.cn

@property 与 @x.setter 配合
来源：http://pl.hahajie.cn

[U30] Py：数据类
来源：http://nf.hnjuh.cn

@dataclass(slots=True)
来源：http://ec.hnjuh.cn

[U31] Py：单测
来源：http://ww.gzmigu.cn

python -m pytest -q
来源：http://mi.newstarts.cn

[U32] Py：代码格式化
来源：http://ma.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://mg.hnjuh.cn

[U33] Py：打包发布
来源：http://cu.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://ma.hnjuh.cn

[U34] Py：判断编码
来源：http://nn.nicolike.cn

chardet.detect(raw)
来源：http://ht.colortex.cn

[U35] Py：发送邮件
来源：http://nk.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gc.shxzskj.cn

[U36] Py：定时任务
来源：http://dm.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://ck.nszjky.cn

[U37] Py：读写 Excel
来源：http://zh.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dg.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://sd.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://dp.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://xp.shxzukj.cn

sys.stdout.isatty()
来源：http://ny.colortex.cn

[U40] Py：打印到标准错误
来源：http://ch.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://mm.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://at.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jz.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://za.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://df.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://or.szsharing.cn

namespace App\Http;
来源：http://hz.colortex.cn

[U44] PHP：开启严格类型
来源：http://ko.muxihuayi.cn

declare(strict_types=1);
来源：http://pn.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://qd.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wo.shtwfgs.cn

[U46] PHP：可空类型
来源：http://ka.haigaiapp.cn

?string $name = null
来源：http://sx.9csxet.cn

[U47] PHP：联合类型
来源：http://an.nszjky.cn

int|string $id
来源：http://cq.gzmigu.cn

[U48] PHP：纯枚举
来源：http://zf.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cb.asd995.cn

[U49] PHP：只读属性
来源：http://ia.521024.cn

public readonly string $name
来源：http://lu.colortex.cn

[U50] PHP：构造器属性提升
来源：http://jm.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://nh.hnjuh.cn

[U51] PHP：数组解构
来源：http://xr.wgjwhj.cn

[$a, $b] = $arr;
来源：http://mb.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://tu.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://bx.asd995.cn

[U53] PHP：空合并运算符
来源：http://ec.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://ku.gzmigu.cn

[U54] PHP：空安全调用
来源：http://md.521024.cn

$obj?->method()
来源：http://wy.lnxyls.cn

[U55] PHP：match 表达式
来源：http://ar.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jk.yuexingan06.cn

[U56] PHP：命名参数
来源：http://lq.chemitech.net.cn

f(a: 1, b: 2)
来源：http://wa.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://ek.huanxung.cn

"值: {$a}"
来源：http://tc.nszjky.cn

[U58] PHP：数组三件套
来源：http://rf.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zf.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://tb.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://br.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://mr.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://je.muxihuayi.cn

[U61] PHP：正则
来源：http://da.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://df.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://lp.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qd.521024.cn

[U63] PHP：文件读写
来源：http://ew.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zl.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://nf.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://uk.huixiangedu.cn

[U65] PHP：会话
来源：http://bb.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kk.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://zz.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qe.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://zd.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wu.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://tm.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://os.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://oo.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xz.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://eo.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eu.hnjuh.cn

[U71] PHP：抛出异常
来源：http://eu.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://lf.521024.cn

[U72] PHP：写错误日志
来源：http://vo.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://ec.newstarts.cn


<!-- 参考信息 -->