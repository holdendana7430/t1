代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://se.521024.cn

[S51] C++：显式类型转换
来源：http://op.chemitech.net.cn

static_cast<double>(a) / b
来源：http://mx.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://jt.521024.cn

int size() const noexcept { return n_; }
来源：http://vt.bookmarksfly.cn

[S53] C++：移动语义
来源：http://el.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://fb.huanxung.cn

[S54] C++：异常处理
来源：http://lv.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bk.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://nr.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bj.haigaiapp.cn

[S56] C++：optional
来源：http://cy.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://na.haigaiapp.cn

[S57] C++：编译期常量
来源：http://zm.asd995.cn

constexpr int N = 10;
来源：http://gn.bjjhwx.cn

[S58] C++：命名空间
来源：http://bt.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://rq.521024.cn

[S59] C++：静态断言
来源：http://rr.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qv.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://ho.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://km.jctech888.com.cn

================================================================================
来源：http://yc.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sq.bjjhwx.cn

================================================================================
来源：http://xb.hahajie.cn

[T01] Kotlin：Hello World
来源：http://if.muxihuayi.cn

println("Hello")
来源：http://gb.shxzukj.cn

[T02] Kotlin：变量
来源：http://tl.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ya.colortex.cn

[T03] Kotlin：字符串模板
来源：http://qn.asd995.cn

"值: $b"
来源：http://wk.asd995.cn

[T04] Kotlin：空安全
来源：http://he.521024.cn

val n: String? = null;  n?.length
来源：http://pb.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://tg.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jx.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://dk.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eg.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://gh.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qg.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://xv.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://ej.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://jv.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://et.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://bi.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tu.colortex.cn

[T11] Kotlin：协程
来源：http://dz.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://su.asd995.cn

[T12] Kotlin：解构声明
来源：http://ix.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://ux.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://om.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://pj.jctech888.com.cn

[T14] Kotlin：循环
来源：http://wy.gzmigu.cn

for (i in 1..10) println(i)
来源：http://av.hahajie.cn

[T15] Kotlin：接口
来源：http://me.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://wy.521024.cn

[T16] Swift：Hello World
来源：http://gh.nszjky.cn

print("Hello")
来源：http://el.lnxyls.cn

[T17] Swift：变量与常量
来源：http://pp.chemitech.net.cn

var a = 1;  let b = 2
来源：http://gp.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://ca.hnjuh.cn

"值: \(b)"
来源：http://ai.shxzskj.cn

[T19] Swift：可选绑定
来源：http://as.521024.cn

if let n = opt { print(n) }
来源：http://gm.nszjky.cn

[T20] Swift：数组操作
来源：http://iu.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wq.nszjky.cn

[T21] Swift：遍历
来源：http://fi.gzmigu.cn

for x in a { print(x) }
来源：http://ow.nszjky.cn

[T22] Swift：字典
来源：http://iw.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tp.shxzskj.cn

[T23] Swift：函数
来源：http://zn.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sk.huixiangedu.cn

[T24] Swift：闭包
来源：http://ew.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sg.newstarts.cn

[T25] Swift：结构体
来源：http://xy.shtwfgs.cn

struct P { var x: Int }
来源：http://dq.muxihuayi.cn

[T26] Swift：类与重写
来源：http://hs.9csxet.cn

class A: Base { override func f() {} }
来源：http://pj.huanxung.cn

[T27] Swift：错误处理
来源：http://vn.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://vp.panjiajie.cn

[T28] Swift：枚举
来源：http://jx.yuntaijiaju.cn

enum Color { case red, green }
来源：http://ct.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://qh.wgjwhj.cn

guard let x = opt else { return }
来源：http://at.szsharing.cn

[T30] Swift：协议
来源：http://jp.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://uw.colortex.cn

[T31] Lua：Hello World
来源：http://ck.lnxyls.cn

print("Hello")
来源：http://bk.szsharing.cn

[T32] Lua：局部变量
来源：http://ei.shxzskj.cn

local a = 1
来源：http://zb.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://zw.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zu.jctech888.com.cn

[T34] Lua：遍历表
来源：http://uh.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ry.muxihuayi.cn

[T35] Lua：字典表
来源：http://zq.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://by.shxzukj.cn

[T36] Lua：函数
来源：http://gu.wgjwhj.cn

function add(a, b) return a + b end
来源：http://uy.nicolike.cn

[T37] Lua：字符串拼接
来源：http://cw.9csxet.cn

"a" .. "b"
来源：http://oz.chemitech.net.cn

[T38] Lua：条件
来源：http://ki.szxytkj.cn

if x > 0 then print("正") end
来源：http://fi.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://dz.szsharing.cn

string.find(s, "%d+")
来源：http://zc.jctech888.com.cn

[T40] Lua：元表
来源：http://jd.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://ez.colortex.cn

[T41] Perl：Hello World
来源：http://pn.asd995.cn

print "Hello\n";
来源：http://zz.nszjky.cn

[T42] Perl：变量类型
来源：http://xd.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ha.shxzukj.cn

[T43] Perl：字符串插值
来源：http://yn.colortex.cn

"值: $a"
来源：http://px.nicolike.cn

[T44] Perl：条件
来源：http://sy.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://hr.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://pz.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://us.szsharing.cn

[T46] Perl：哈希操作
来源：http://yp.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oz.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://lv.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://di.hnjuh.cn

[T48] Perl：正则替换
来源：http://le.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://aw.asd995.cn

[T49] Perl：函数
来源：http://ht.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ya.521024.cn

[T50] Perl：逐行读文件
来源：http://ri.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hw.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://id.wgjwhj.cn

[T51] Scala：Hello World
来源：http://li.jianghongdianzi.cn

println("Hello")
来源：http://cu.bookmarksfly.cn

[T52] Scala：变量
来源：http://jp.colortex.cn

val a = 1;  var b = 2
来源：http://fb.hnjuh.cn

[T53] Scala：字符串插值
来源：http://gs.521024.cn

s"值: $b"
来源：http://ao.lnxyls.cn

[T54] Scala：集合映射
来源：http://rr.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://sp.panjiajie.cn

[T55] Scala：集合过滤
来源：http://yb.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iz.shtwfgs.cn

[T56] Scala：样例类
来源：http://ms.hahajie.cn

case class User(name: String, age: Int)
来源：http://aa.huanxung.cn

[T57] Scala：模式匹配
来源：http://eb.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rp.jctech888.com.cn

[T58] Scala：函数定义
来源：http://bf.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wc.muxihuayi.cn

[T59] Scala：循环
来源：http://qk.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://xk.9csxet.cn

[T60] Scala：折叠
来源：http://jo.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mi.jctech888.com.cn

================================================================================
来源：http://xy.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://la.hahajie.cn

================================================================================
来源：http://fz.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://yx.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yv.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://oz.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sn.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://zf.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wc.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://wn.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vd.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://jy.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://un.521024.cn

[U06] Py：合并两个字典
来源：http://zw.bookmarksfly.cn

{**a, **b}
来源：http://xr.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://yn.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://xe.szxytkj.cn

[U08] Py：展平二维列表
来源：http://me.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://aw.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://wo.shxzukj.cn

max(d, key=d.get)
来源：http://yu.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://dz.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ft.hahajie.cn

[U11] Py：生成器表达式
来源：http://cz.wgjwhj.cn

(x * 2 for x in arr)
来源：http://dp.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hp.hahajie.cn

Counter(arr).most_common(3)
来源：http://sa.shxzskj.cn

[U13] Py：固定长度队列
来源：http://rc.huanxung.cn

deque(maxlen=10)
来源：http://mc.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://sf.jctech888.com.cn

defaultdict(list)
来源：http://tr.colortex.cn

[U15] Py：高精度计时
来源：http://lw.hnjuh.cn

t = time.perf_counter()
来源：http://xt.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://zb.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vm.wgjwhj.cn

[U17] Py：初始化日志
来源：http://lk.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://ns.wgjwhj.cn

[U18] Py：预编译正则
来源：http://mk.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://de.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://xh.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fp.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://ik.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://at.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://rz.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://gu.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://po.newstarts.cn

list(zip(*m))
来源：http://aa.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://oy.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gc.newstarts.cn

[U24] Py：路径操作
来源：http://we.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lf.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://aa.huixiangedu.cn

csv.DictReader(f)
来源：http://lp.nszjky.cn

[U26] Py：并发下载
来源：http://pz.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xr.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://hz.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://uh.9csxet.cn

[U28] Py：类型别名
来源：http://rk.hahajie.cn

UserId = int
来源：http://cm.chemitech.net.cn

[U29] Py：属性校验
来源：http://fq.panjiajie.cn

@property 与 @x.setter 配合
来源：http://mn.haigaiapp.cn

[U30] Py：数据类
来源：http://ij.jctech888.com.cn

@dataclass(slots=True)
来源：http://kg.9csxet.cn

[U31] Py：单测
来源：http://gx.9csxet.cn

python -m pytest -q
来源：http://fs.shxzukj.cn

[U32] Py：代码格式化
来源：http://nk.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://cv.gzmigu.cn

[U33] Py：打包发布
来源：http://bg.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://qf.lnxyls.cn

[U34] Py：判断编码
来源：http://en.huanxung.cn

chardet.detect(raw)
来源：http://we.szsharing.cn

[U35] Py：发送邮件
来源：http://fn.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yg.panjiajie.cn

[U36] Py：定时任务
来源：http://xz.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://lk.newstarts.cn

[U37] Py：读写 Excel
来源：http://gj.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fv.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://xd.huanxung.cn

Path(__file__).resolve().parent
来源：http://fq.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://pw.bjjhwx.cn

sys.stdout.isatty()
来源：http://cb.9csxet.cn

[U40] Py：打印到标准错误
来源：http://ic.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://nf.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://wr.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yz.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://sd.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zc.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://el.shxzskj.cn

namespace App\Http;
来源：http://dx.nicolike.cn

[U44] PHP：开启严格类型
来源：http://ng.jianghongdianzi.cn

declare(strict_types=1);
来源：http://sz.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://ax.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mu.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://vm.asd995.cn

?string $name = null
来源：http://sh.yuexingan06.cn

[U47] PHP：联合类型
来源：http://tb.asd995.cn

int|string $id
来源：http://vr.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://zk.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://id.9csxet.cn

[U49] PHP：只读属性
来源：http://cl.nicolike.cn

public readonly string $name
来源：http://zu.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://qq.hnjuh.cn

public function __construct(private int $id) {}
来源：http://ho.lnxyls.cn

[U51] PHP：数组解构
来源：http://pq.huixiangedu.cn

[$a, $b] = $arr;
来源：http://ro.newstarts.cn

[U52] PHP：箭头函数
来源：http://hd.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://ih.9csxet.cn

[U53] PHP：空合并运算符
来源：http://nf.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://op.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://im.szxytkj.cn

$obj?->method()
来源：http://mq.521024.cn

[U55] PHP：match 表达式
来源：http://an.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://br.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://ne.wgjwhj.cn

f(a: 1, b: 2)
来源：http://pz.hnjuh.cn

[U57] PHP：字符串插值
来源：http://ib.yuntaijiaju.cn

"值: {$a}"
来源：http://ni.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://qh.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://re.panjiajie.cn

[U59] PHP：自定义排序
来源：http://pi.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://we.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://ch.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yy.gzmigu.cn

[U61] PHP：正则
来源：http://jp.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ry.huixiangedu.cn

[U62] PHP：日期对象
来源：http://uj.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dc.9csxet.cn

[U63] PHP：文件读写
来源：http://hn.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uw.hahajie.cn

[U64] PHP：目录遍历
来源：http://az.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://gl.hahajie.cn

[U65] PHP：会话
来源：http://hv.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ex.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://pi.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://il.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://tt.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lj.9csxet.cn

[U68] PHP：PDO 连接
来源：http://rp.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hn.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://tv.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ug.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://so.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://er.9csxet.cn

[U71] PHP：抛出异常
来源：http://gh.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://vh.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://wy.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://am.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://ad.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://mt.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://ws.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://xg.shxzukj.cn

[U75] PHP：依赖注入
来源：http://fk.haigaiapp.cn

composer require psr/container
来源：http://hy.szsharing.cn

[U76] PHP：简单路由
来源：http://mp.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zh.szxytkj.cn


<!-- 参考信息 -->