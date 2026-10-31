代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jv.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://ba.panjiajie.cn

static_cast<double>(a) / b
来源：http://wb.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://xw.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://ow.shxzukj.cn

[S53] C++：移动语义
来源：http://bp.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://fv.521024.cn

[S54] C++：异常处理
来源：http://hy.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://un.shxzukj.cn

[S55] C++：结构化绑定
来源：http://zr.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://za.chemitech.net.cn

[S56] C++：optional
来源：http://zv.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cn.521024.cn

[S57] C++：编译期常量
来源：http://fe.colortex.cn

constexpr int N = 10;
来源：http://id.9csxet.cn

[S58] C++：命名空间
来源：http://lq.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://ds.shxzskj.cn

[S59] C++：静态断言
来源：http://vy.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pk.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://hf.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oo.yuexingan06.cn

================================================================================
来源：http://qs.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dn.shtwfgs.cn

================================================================================
来源：http://pz.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://zf.shxzskj.cn

println("Hello")
来源：http://wz.gzmigu.cn

[T02] Kotlin：变量
来源：http://gw.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xs.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://iy.nicolike.cn

"值: $b"
来源：http://rq.9csxet.cn

[T04] Kotlin：空安全
来源：http://mr.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://sc.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://up.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ta.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://mb.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eo.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://kj.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gh.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://ce.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://vi.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://du.521024.cn

fun String.exclaim() = this + "!"
来源：http://mt.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://vx.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qs.shxzskj.cn

[T11] Kotlin：协程
来源：http://jl.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qj.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://hm.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://rq.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://se.nszjky.cn

val m = mapOf("a" to 1)
来源：http://st.asd995.cn

[T14] Kotlin：循环
来源：http://hy.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://oe.9csxet.cn

[T15] Kotlin：接口
来源：http://is.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://dz.haigaiapp.cn

[T16] Swift：Hello World
来源：http://rm.asd995.cn

print("Hello")
来源：http://rv.521024.cn

[T17] Swift：变量与常量
来源：http://hh.huixiangedu.cn

var a = 1;  let b = 2
来源：http://mo.colortex.cn

[T18] Swift：字符串插值
来源：http://ka.shxzukj.cn

"值: \(b)"
来源：http://hi.gzmigu.cn

[T19] Swift：可选绑定
来源：http://uy.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://vc.jctech888.com.cn

[T20] Swift：数组操作
来源：http://dd.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uu.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://za.haigaiapp.cn

for x in a { print(x) }
来源：http://da.jianghongdianzi.cn

[T22] Swift：字典
来源：http://mj.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ur.hnjuh.cn

[T23] Swift：函数
来源：http://lf.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aw.muxihuayi.cn

[T24] Swift：闭包
来源：http://bv.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xp.nszjky.cn

[T25] Swift：结构体
来源：http://jy.panjiajie.cn

struct P { var x: Int }
来源：http://vj.shtwfgs.cn

[T26] Swift：类与重写
来源：http://az.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://kw.szsharing.cn

[T27] Swift：错误处理
来源：http://jo.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://ba.shtwfgs.cn

[T28] Swift：枚举
来源：http://vo.bjjhwx.cn

enum Color { case red, green }
来源：http://xn.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://uh.haigaiapp.cn

guard let x = opt else { return }
来源：http://rr.haigaiapp.cn

[T30] Swift：协议
来源：http://ut.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://me.shxzukj.cn

[T31] Lua：Hello World
来源：http://ai.huanxung.cn

print("Hello")
来源：http://zs.wgjwhj.cn

[T32] Lua：局部变量
来源：http://lw.szsharing.cn

local a = 1
来源：http://zj.szsharing.cn

[T33] Lua：表（数组）
来源：http://yw.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lj.huanxung.cn

[T34] Lua：遍历表
来源：http://wv.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rv.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://zh.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://kt.yuexingan06.cn

[T36] Lua：函数
来源：http://gh.hahajie.cn

function add(a, b) return a + b end
来源：http://ud.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://rf.nicolike.cn

"a" .. "b"
来源：http://xh.jctech888.com.cn

[T38] Lua：条件
来源：http://sc.nszjky.cn

if x > 0 then print("正") end
来源：http://bo.nicolike.cn

[T39] Lua：模式匹配
来源：http://jz.9csxet.cn

string.find(s, "%d+")
来源：http://pl.yuntaijiaju.cn

[T40] Lua：元表
来源：http://eb.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://rs.gzmigu.cn

[T41] Perl：Hello World
来源：http://wx.wgjwhj.cn

print "Hello\n";
来源：http://df.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://jj.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yy.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://rw.nicolike.cn

"值: $a"
来源：http://xi.muxihuayi.cn

[T44] Perl：条件
来源：http://av.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://bi.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://ge.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://et.shxzukj.cn

[T46] Perl：哈希操作
来源：http://im.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fs.shxzukj.cn

[T47] Perl：正则捕获
来源：http://sr.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cr.wgjwhj.cn

[T48] Perl：正则替换
来源：http://ev.newstarts.cn

$s =~ s/old/new/g;
来源：http://xj.huixinmuqiang.cn

[T49] Perl：函数
来源：http://yl.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mc.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://qb.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xe.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://fk.nszjky.cn

[T51] Scala：Hello World
来源：http://ox.jianghongdianzi.cn

println("Hello")
来源：http://lt.yuntaijiaju.cn

[T52] Scala：变量
来源：http://lp.hahajie.cn

val a = 1;  var b = 2
来源：http://qn.nszjky.cn

[T53] Scala：字符串插值
来源：http://cw.yuntaijiaju.cn

s"值: $b"
来源：http://aa.shtwfgs.cn

[T54] Scala：集合映射
来源：http://bz.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://mf.szxytkj.cn

[T55] Scala：集合过滤
来源：http://iy.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://st.lnxyls.cn

[T56] Scala：样例类
来源：http://ho.gzmigu.cn

case class User(name: String, age: Int)
来源：http://ql.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://md.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dd.shxzukj.cn

[T58] Scala：函数定义
来源：http://kj.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mp.haigaiapp.cn

[T59] Scala：循环
来源：http://jw.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://uq.shtwfgs.cn

[T60] Scala：折叠
来源：http://rl.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pa.521024.cn

================================================================================
来源：http://kr.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dx.shtwfgs.cn

================================================================================
来源：http://bu.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://yf.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pj.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://ml.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hw.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://ig.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yt.shxzukj.cn

[U04] Py：变量调试打印
来源：http://ha.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nt.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://rd.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://oy.colortex.cn

[U06] Py：合并两个字典
来源：http://zt.shtwfgs.cn

{**a, **b}
来源：http://rb.panjiajie.cn

[U07] Py：反转字典键值
来源：http://gi.9csxet.cn

{v: k for k, v in d.items()}
来源：http://ui.panjiajie.cn

[U08] Py：展平二维列表
来源：http://uq.huixiangedu.cn

[y for x in nested for y in x]
来源：http://ai.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://ow.szsharing.cn

max(d, key=d.get)
来源：http://ht.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://fp.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aw.asd995.cn

[U11] Py：生成器表达式
来源：http://ld.szxytkj.cn

(x * 2 for x in arr)
来源：http://rp.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pu.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://zt.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://bw.bjjhwx.cn

deque(maxlen=10)
来源：http://nh.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://bf.hahajie.cn

defaultdict(list)
来源：http://ex.gzmigu.cn

[U15] Py：高精度计时
来源：http://it.shxzskj.cn

t = time.perf_counter()
来源：http://gm.colortex.cn

[U16] Py：命令行参数解析
来源：http://gu.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pl.asd995.cn

[U17] Py：初始化日志
来源：http://lq.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://jb.chemitech.net.cn

[U18] Py：预编译正则
来源：http://zi.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://sw.asd995.cn

[U19] Py：正则替换带回调
来源：http://de.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kg.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://oy.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://bq.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://iu.asd995.cn

@contextlib.contextmanager
来源：http://xz.newstarts.cn

[U22] Py：矩阵转置
来源：http://ax.huanxung.cn

list(zip(*m))
来源：http://jh.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://hc.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ab.bjjhwx.cn

[U24] Py：路径操作
来源：http://ev.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zu.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://cb.huixiangedu.cn

csv.DictReader(f)
来源：http://uw.521024.cn

[U26] Py：并发下载
来源：http://zb.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ht.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://cc.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://zl.muxihuayi.cn

[U28] Py：类型别名
来源：http://gs.wgjwhj.cn

UserId = int
来源：http://xy.9csxet.cn

[U29] Py：属性校验
来源：http://ot.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://zb.521024.cn

[U30] Py：数据类
来源：http://fw.gzmigu.cn

@dataclass(slots=True)
来源：http://ki.szsharing.cn

[U31] Py：单测
来源：http://tw.huixinmuqiang.cn

python -m pytest -q
来源：http://lm.521024.cn

[U32] Py：代码格式化
来源：http://ra.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://ag.bjjhwx.cn

[U33] Py：打包发布
来源：http://zh.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://mn.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://ov.huixinmuqiang.cn

chardet.detect(raw)
来源：http://dc.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://pf.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://at.gzmigu.cn

[U36] Py：定时任务
来源：http://qa.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://dr.521024.cn

[U37] Py：读写 Excel
来源：http://kl.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uj.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://gh.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://er.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://uf.muxihuayi.cn

sys.stdout.isatty()
来源：http://cn.521024.cn

[U40] Py：打印到标准错误
来源：http://hq.nszjky.cn

print("err", file=sys.stderr)
来源：http://ea.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://gr.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ap.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://yb.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yq.hahajie.cn

[U43] PHP：声明命名空间
来源：http://dr.bjjhwx.cn

namespace App\Http;
来源：http://xb.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://ez.huanxung.cn

declare(strict_types=1);
来源：http://zn.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://xu.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vo.shxzskj.cn

[U46] PHP：可空类型
来源：http://ve.shxzukj.cn

?string $name = null
来源：http://wh.haigaiapp.cn

[U47] PHP：联合类型
来源：http://xn.jctech888.com.cn

int|string $id
来源：http://qx.nicolike.cn

[U48] PHP：纯枚举
来源：http://mq.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ye.newstarts.cn

[U49] PHP：只读属性
来源：http://eb.521024.cn

public readonly string $name
来源：http://ex.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://ti.lnxyls.cn

public function __construct(private int $id) {}
来源：http://mx.szxytkj.cn

[U51] PHP：数组解构
来源：http://ma.nszjky.cn

[$a, $b] = $arr;
来源：http://rx.shxzukj.cn

[U52] PHP：箭头函数
来源：http://uo.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://my.nicolike.cn

[U53] PHP：空合并运算符
来源：http://ug.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://jo.nszjky.cn

[U54] PHP：空安全调用
来源：http://oq.nszjky.cn

$obj?->method()
来源：http://uj.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://zk.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sg.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://hh.hahajie.cn

f(a: 1, b: 2)
来源：http://ny.nszjky.cn

[U57] PHP：字符串插值
来源：http://rn.bookmarksfly.cn

"值: {$a}"
来源：http://af.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://sy.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gt.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://sm.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bi.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://ab.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qc.colortex.cn

[U61] PHP：正则
来源：http://vw.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://md.chemitech.net.cn

[U62] PHP：日期对象
来源：http://fu.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hr.9csxet.cn

[U63] PHP：文件读写
来源：http://hy.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zz.hnjuh.cn

[U64] PHP：目录遍历
来源：http://vb.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://eb.lnxyls.cn

[U65] PHP：会话
来源：http://dj.gzmigu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kv.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://ew.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pf.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://pg.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://at.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://ic.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jm.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://sq.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eo.newstarts.cn

[U70] PHP：PDO 事务
来源：http://op.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nt.nicolike.cn

[U71] PHP：抛出异常
来源：http://av.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://uc.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://ix.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://dt.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://gz.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://ss.szsharing.cn

[U74] PHP：读取环境变量
来源：http://qc.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://lk.shxzukj.cn

[U75] PHP：依赖注入
来源：http://fq.jianghongdianzi.cn

composer require psr/container
来源：http://jc.szxytkj.cn

[U76] PHP：简单路由
来源：http://hg.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kt.jianghongdianzi.cn


<!-- 参考信息 -->