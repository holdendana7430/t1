代发 wailian999

int size() const noexcept { return n_; }
来源：http://qi.gzmigu.cn

[S53] C++：移动语义
来源：http://nb.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://lb.hahajie.cn

[S54] C++：异常处理
来源：http://cc.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jc.lnxyls.cn

[S55] C++：结构化绑定
来源：http://ro.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ey.shxzskj.cn

[S56] C++：optional
来源：http://bq.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fq.yuexingan06.cn

[S57] C++：编译期常量
来源：http://fd.hahajie.cn

constexpr int N = 10;
来源：http://sl.haigaiapp.cn

[S58] C++：命名空间
来源：http://mg.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://bb.521024.cn

[S59] C++：静态断言
来源：http://cj.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sj.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://fu.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://td.szxytkj.cn

================================================================================
来源：http://px.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ve.chemitech.net.cn

================================================================================
来源：http://oy.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://ea.hnjuh.cn

println("Hello")
来源：http://wf.bjjhwx.cn

[T02] Kotlin：变量
来源：http://jy.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ju.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://xb.huanxung.cn

"值: $b"
来源：http://cs.szsharing.cn

[T04] Kotlin：空安全
来源：http://no.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://bb.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://lw.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pe.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://cb.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hy.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://bl.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bs.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://ee.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://bz.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://zr.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://ch.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://ih.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://km.jctech888.com.cn

[T11] Kotlin：协程
来源：http://zs.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pe.hahajie.cn

[T12] Kotlin：解构声明
来源：http://ox.521024.cn

val (a, b) = Pair(1, 2)
来源：http://ck.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://yt.nicolike.cn

val m = mapOf("a" to 1)
来源：http://au.gzmigu.cn

[T14] Kotlin：循环
来源：http://zz.nszjky.cn

for (i in 1..10) println(i)
来源：http://to.hnjuh.cn

[T15] Kotlin：接口
来源：http://gi.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://rx.huanxung.cn

[T16] Swift：Hello World
来源：http://km.shxzukj.cn

print("Hello")
来源：http://kf.newstarts.cn

[T17] Swift：变量与常量
来源：http://ze.jctech888.com.cn

var a = 1;  let b = 2
来源：http://aa.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://hx.hahajie.cn

"值: \(b)"
来源：http://ux.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://jp.521024.cn

if let n = opt { print(n) }
来源：http://pw.muxihuayi.cn

[T20] Swift：数组操作
来源：http://py.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gn.shxzukj.cn

[T21] Swift：遍历
来源：http://dw.szsharing.cn

for x in a { print(x) }
来源：http://mi.lnxyls.cn

[T22] Swift：字典
来源：http://yd.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pe.shxzskj.cn

[T23] Swift：函数
来源：http://yc.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vz.gzmigu.cn

[T24] Swift：闭包
来源：http://go.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hl.panjiajie.cn

[T25] Swift：结构体
来源：http://oc.yuntaijiaju.cn

struct P { var x: Int }
来源：http://jp.wgjwhj.cn

[T26] Swift：类与重写
来源：http://hd.521024.cn

class A: Base { override func f() {} }
来源：http://il.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://gu.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://pw.hahajie.cn

[T28] Swift：枚举
来源：http://uo.shtwfgs.cn

enum Color { case red, green }
来源：http://wb.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://zm.shxzukj.cn

guard let x = opt else { return }
来源：http://xx.chemitech.net.cn

[T30] Swift：协议
来源：http://ix.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://bg.shtwfgs.cn

[T31] Lua：Hello World
来源：http://ih.bjjhwx.cn

print("Hello")
来源：http://jd.yuexingan06.cn

[T32] Lua：局部变量
来源：http://lx.szxytkj.cn

local a = 1
来源：http://ho.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://fg.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ft.shxzukj.cn

[T34] Lua：遍历表
来源：http://sh.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dk.szxytkj.cn

[T35] Lua：字典表
来源：http://ts.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://uz.shxzskj.cn

[T36] Lua：函数
来源：http://pw.huanxung.cn

function add(a, b) return a + b end
来源：http://ld.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://xk.yuntaijiaju.cn

"a" .. "b"
来源：http://nn.bookmarksfly.cn

[T38] Lua：条件
来源：http://wa.nicolike.cn

if x > 0 then print("正") end
来源：http://hy.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://uu.szsharing.cn

string.find(s, "%d+")
来源：http://kb.nicolike.cn

[T40] Lua：元表
来源：http://kx.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://ei.huanxung.cn

[T41] Perl：Hello World
来源：http://xr.9csxet.cn

print "Hello\n";
来源：http://im.colortex.cn

[T42] Perl：变量类型
来源：http://ej.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xi.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://mr.colortex.cn

"值: $a"
来源：http://kg.szsharing.cn

[T44] Perl：条件
来源：http://ie.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://yl.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://hw.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://ho.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://ov.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fp.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://xw.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mb.huixiangedu.cn

[T48] Perl：正则替换
来源：http://am.hnjuh.cn

$s =~ s/old/new/g;
来源：http://rh.szxytkj.cn

[T49] Perl：函数
来源：http://at.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mm.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://hq.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://am.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://zp.szxytkj.cn

[T51] Scala：Hello World
来源：http://cr.jctech888.com.cn

println("Hello")
来源：http://vo.huixinmuqiang.cn

[T52] Scala：变量
来源：http://wz.gzmigu.cn

val a = 1;  var b = 2
来源：http://fo.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://yq.haigaiapp.cn

s"值: $b"
来源：http://dm.szxytkj.cn

[T54] Scala：集合映射
来源：http://qm.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://xx.shxzskj.cn

[T55] Scala：集合过滤
来源：http://et.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sy.huanxung.cn

[T56] Scala：样例类
来源：http://hh.szxytkj.cn

case class User(name: String, age: Int)
来源：http://wo.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://am.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qu.muxihuayi.cn

[T58] Scala：函数定义
来源：http://at.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xy.chemitech.net.cn

[T59] Scala：循环
来源：http://pc.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://wq.bjjhwx.cn

[T60] Scala：折叠
来源：http://dm.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tr.nszjky.cn

================================================================================
来源：http://rc.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vt.huanxung.cn

================================================================================
来源：http://ml.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://ps.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://od.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://wl.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ga.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://cq.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fg.9csxet.cn

[U04] Py：变量调试打印
来源：http://bw.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zm.szsharing.cn

[U05] Py：列表去重且保序
来源：http://ui.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://hr.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://nd.jctech888.com.cn

{**a, **b}
来源：http://jf.szsharing.cn

[U07] Py：反转字典键值
来源：http://fg.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://ut.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://ql.haigaiapp.cn

[y for x in nested for y in x]
来源：http://nw.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://xk.asd995.cn

max(d, key=d.get)
来源：http://en.huanxung.cn

[U10] Py：按值排序字典
来源：http://sp.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fg.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://du.panjiajie.cn

(x * 2 for x in arr)
来源：http://tq.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ur.hahajie.cn

Counter(arr).most_common(3)
来源：http://dk.colortex.cn

[U13] Py：固定长度队列
来源：http://ph.lnxyls.cn

deque(maxlen=10)
来源：http://jo.nicolike.cn

[U14] Py：分组收集到列表
来源：http://na.jianghongdianzi.cn

defaultdict(list)
来源：http://ht.huanxung.cn

[U15] Py：高精度计时
来源：http://om.bookmarksfly.cn

t = time.perf_counter()
来源：http://kb.521024.cn

[U16] Py：命令行参数解析
来源：http://zw.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://io.hnjuh.cn

[U17] Py：初始化日志
来源：http://nm.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://xo.szxytkj.cn

[U18] Py：预编译正则
来源：http://lh.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://go.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://jw.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pg.521024.cn

[U20] Py：缓存函数结果
来源：http://hf.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://gc.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://lc.hahajie.cn

@contextlib.contextmanager
来源：http://ti.gzmigu.cn

[U22] Py：矩阵转置
来源：http://sr.bookmarksfly.cn

list(zip(*m))
来源：http://wt.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://qf.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wj.wgjwhj.cn

[U24] Py：路径操作
来源：http://ym.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dc.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://am.521024.cn

csv.DictReader(f)
来源：http://xi.szxytkj.cn

[U26] Py：并发下载
来源：http://yv.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vc.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://mj.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://zz.wgjwhj.cn

[U28] Py：类型别名
来源：http://zu.panjiajie.cn

UserId = int
来源：http://sc.lnxyls.cn

[U29] Py：属性校验
来源：http://hg.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://xe.yuexingan06.cn

[U30] Py：数据类
来源：http://gk.huixiangedu.cn

@dataclass(slots=True)
来源：http://lf.huixinmuqiang.cn

[U31] Py：单测
来源：http://ar.hnjuh.cn

python -m pytest -q
来源：http://ut.muxihuayi.cn

[U32] Py：代码格式化
来源：http://yu.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://ge.lnxyls.cn

[U33] Py：打包发布
来源：http://xf.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://vo.shtwfgs.cn

[U34] Py：判断编码
来源：http://ca.jctech888.com.cn

chardet.detect(raw)
来源：http://cq.szxytkj.cn

[U35] Py：发送邮件
来源：http://mi.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cn.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://zx.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://cd.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://aw.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cq.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://dt.panjiajie.cn

Path(__file__).resolve().parent
来源：http://dc.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://xq.521024.cn

sys.stdout.isatty()
来源：http://qb.521024.cn

[U40] Py：打印到标准错误
来源：http://hb.shxzskj.cn

print("err", file=sys.stderr)
来源：http://tw.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://rr.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mo.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://mc.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cp.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://fm.nicolike.cn

namespace App\Http;
来源：http://ty.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://yi.jctech888.com.cn

declare(strict_types=1);
来源：http://th.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://ya.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qm.szxytkj.cn

[U46] PHP：可空类型
来源：http://kl.colortex.cn

?string $name = null
来源：http://ls.bjjhwx.cn

[U47] PHP：联合类型
来源：http://gn.nszjky.cn

int|string $id
来源：http://co.9csxet.cn

[U48] PHP：纯枚举
来源：http://yy.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rv.wgjwhj.cn

[U49] PHP：只读属性
来源：http://ks.hnjuh.cn

public readonly string $name
来源：http://ir.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://yk.hahajie.cn

public function __construct(private int $id) {}
来源：http://he.huixiangedu.cn

[U51] PHP：数组解构
来源：http://lp.huanxung.cn

[$a, $b] = $arr;
来源：http://rx.hnjuh.cn

[U52] PHP：箭头函数
来源：http://wk.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://le.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://vu.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://dw.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://op.panjiajie.cn

$obj?->method()
来源：http://rt.huanxung.cn

[U55] PHP：match 表达式
来源：http://ku.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zl.newstarts.cn

[U56] PHP：命名参数
来源：http://je.newstarts.cn

f(a: 1, b: 2)
来源：http://wb.panjiajie.cn

[U57] PHP：字符串插值
来源：http://ck.yuexingan06.cn

"值: {$a}"
来源：http://lr.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://hf.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sv.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://bk.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ht.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://st.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eh.hnjuh.cn

[U61] PHP：正则
来源：http://wt.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yd.chemitech.net.cn

[U62] PHP：日期对象
来源：http://qk.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gw.panjiajie.cn

[U63] PHP：文件读写
来源：http://wf.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bo.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://od.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://gs.asd995.cn

[U65] PHP：会话
来源：http://pj.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vm.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://di.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tp.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://cm.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lm.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://jh.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dz.521024.cn

[U69] PHP：PDO 预处理
来源：http://ur.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://th.nszjky.cn

[U70] PHP：PDO 事务
来源：http://pb.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nn.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://ly.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://qn.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://ra.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://ka.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://an.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://dp.newstarts.cn

[U74] PHP：读取环境变量
来源：http://zp.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://kn.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://sa.newstarts.cn

composer require psr/container
来源：http://jj.panjiajie.cn

[U76] PHP：简单路由
来源：http://qu.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hl.521024.cn

[U77] PHP：模板渲染
来源：http://bf.nszjky.cn

composer require twig/twig
来源：http://lm.9csxet.cn

[U78] PHP：单元测试
来源：http://de.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://jj.wgjwhj.cn


<!-- 参考信息 -->