代发 wailian999

int size() const noexcept { return n_; }
来源：http://ex.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://ft.asd995.cn

std::vector<int> w = std::move(v);
来源：http://qv.haigaiapp.cn

[S54] C++：异常处理
来源：http://lf.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gx.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://vh.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ks.nicolike.cn

[S56] C++：optional
来源：http://os.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://be.szxytkj.cn

[S57] C++：编译期常量
来源：http://ir.huixinmuqiang.cn

constexpr int N = 10;
来源：http://ro.521024.cn

[S58] C++：命名空间
来源：http://tu.521024.cn

namespace ns { int f() { return 1; } }
来源：http://pt.wgjwhj.cn

[S59] C++：静态断言
来源：http://ea.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tl.colortex.cn

[S60] C++：遍历并删除元素
来源：http://rx.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fr.szsharing.cn

================================================================================
来源：http://hr.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tv.colortex.cn

================================================================================
来源：http://ox.hahajie.cn

[T01] Kotlin：Hello World
来源：http://mh.shxzskj.cn

println("Hello")
来源：http://it.shxzskj.cn

[T02] Kotlin：变量
来源：http://as.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qh.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://yc.chemitech.net.cn

"值: $b"
来源：http://fp.nszjky.cn

[T04] Kotlin：空安全
来源：http://ql.nicolike.cn

val n: String? = null;  n?.length
来源：http://mk.521024.cn

[T05] Kotlin：when 表达式
来源：http://tq.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tp.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://oq.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fg.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://oh.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ud.521024.cn

[T08] Kotlin：数据类
来源：http://fn.asd995.cn

data class User(val name: String, val age: Int)
来源：http://do.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://qh.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://ah.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://ah.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gj.jctech888.com.cn

[T11] Kotlin：协程
来源：http://wo.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yl.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://ry.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://qz.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://te.521024.cn

val m = mapOf("a" to 1)
来源：http://el.newstarts.cn

[T14] Kotlin：循环
来源：http://zb.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://us.muxihuayi.cn

[T15] Kotlin：接口
来源：http://eh.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://ej.nicolike.cn

[T16] Swift：Hello World
来源：http://oy.nszjky.cn

print("Hello")
来源：http://yg.szxytkj.cn

[T17] Swift：变量与常量
来源：http://rz.asd995.cn

var a = 1;  let b = 2
来源：http://tf.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://bp.hnjuh.cn

"值: \(b)"
来源：http://mg.szsharing.cn

[T19] Swift：可选绑定
来源：http://vf.lnxyls.cn

if let n = opt { print(n) }
来源：http://aq.521024.cn

[T20] Swift：数组操作
来源：http://fg.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wd.yuexingan06.cn

[T21] Swift：遍历
来源：http://bu.szsharing.cn

for x in a { print(x) }
来源：http://af.huanxung.cn

[T22] Swift：字典
来源：http://xw.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fd.huanxung.cn

[T23] Swift：函数
来源：http://vz.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://th.muxihuayi.cn

[T24] Swift：闭包
来源：http://kt.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xr.shxzukj.cn

[T25] Swift：结构体
来源：http://zj.521024.cn

struct P { var x: Int }
来源：http://vm.jctech888.com.cn

[T26] Swift：类与重写
来源：http://kk.521024.cn

class A: Base { override func f() {} }
来源：http://oj.newstarts.cn

[T27] Swift：错误处理
来源：http://og.szsharing.cn

do { try f() } catch { print(error) }
来源：http://sa.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://vq.hnjuh.cn

enum Color { case red, green }
来源：http://wc.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://sw.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://qt.colortex.cn

[T30] Swift：协议
来源：http://gh.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://bh.colortex.cn

[T31] Lua：Hello World
来源：http://ng.huixinmuqiang.cn

print("Hello")
来源：http://yw.szxytkj.cn

[T32] Lua：局部变量
来源：http://rv.colortex.cn

local a = 1
来源：http://so.asd995.cn

[T33] Lua：表（数组）
来源：http://bz.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zt.haigaiapp.cn

[T34] Lua：遍历表
来源：http://ww.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tv.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://ja.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://zq.gzmigu.cn

[T36] Lua：函数
来源：http://ow.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://au.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://cd.shtwfgs.cn

"a" .. "b"
来源：http://hp.muxihuayi.cn

[T38] Lua：条件
来源：http://re.9csxet.cn

if x > 0 then print("正") end
来源：http://ya.asd995.cn

[T39] Lua：模式匹配
来源：http://kj.hnjuh.cn

string.find(s, "%d+")
来源：http://mp.yuexingan06.cn

[T40] Lua：元表
来源：http://tu.nicolike.cn

setmetatable({}, { __index = base })
来源：http://gz.newstarts.cn

[T41] Perl：Hello World
来源：http://ze.szsharing.cn

print "Hello\n";
来源：http://bq.chemitech.net.cn

[T42] Perl：变量类型
来源：http://xk.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ta.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://ds.nicolike.cn

"值: $a"
来源：http://uw.haigaiapp.cn

[T44] Perl：条件
来源：http://oy.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://ax.newstarts.cn

[T45] Perl：数组遍历
来源：http://mw.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://wk.521024.cn

[T46] Perl：哈希操作
来源：http://ih.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qz.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://hs.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zq.shxzukj.cn

[T48] Perl：正则替换
来源：http://zk.huanxung.cn

$s =~ s/old/new/g;
来源：http://jg.wgjwhj.cn

[T49] Perl：函数
来源：http://dq.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dy.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://ul.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vh.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://zs.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://nb.shxzskj.cn

println("Hello")
来源：http://zi.haigaiapp.cn

[T52] Scala：变量
来源：http://ie.bjjhwx.cn

val a = 1;  var b = 2
来源：http://ff.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://jm.lnxyls.cn

s"值: $b"
来源：http://kf.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://fd.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://fn.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://aq.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uf.nszjky.cn

[T56] Scala：样例类
来源：http://qp.asd995.cn

case class User(name: String, age: Int)
来源：http://wx.nszjky.cn

[T57] Scala：模式匹配
来源：http://ty.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ue.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://zk.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iu.panjiajie.cn

[T59] Scala：循环
来源：http://wq.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://cy.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://tp.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jy.nicolike.cn

================================================================================
来源：http://uv.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ax.huixiangedu.cn

================================================================================
来源：http://os.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://fu.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://az.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://pj.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lu.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://pw.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dc.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://vq.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cf.9csxet.cn

[U05] Py：列表去重且保序
来源：http://sm.nszjky.cn

list(dict.fromkeys(arr))
来源：http://hr.colortex.cn

[U06] Py：合并两个字典
来源：http://co.yuntaijiaju.cn

{**a, **b}
来源：http://va.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://fo.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://xe.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://bl.szsharing.cn

[y for x in nested for y in x]
来源：http://wc.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://mt.hahajie.cn

max(d, key=d.get)
来源：http://cn.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://cf.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zi.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://va.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://lj.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qu.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://ga.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://ff.huixiangedu.cn

deque(maxlen=10)
来源：http://hp.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://ff.hnjuh.cn

defaultdict(list)
来源：http://fn.bjjhwx.cn

[U15] Py：高精度计时
来源：http://mc.asd995.cn

t = time.perf_counter()
来源：http://zo.newstarts.cn

[U16] Py：命令行参数解析
来源：http://vf.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bp.nszjky.cn

[U17] Py：初始化日志
来源：http://gq.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://cq.asd995.cn

[U18] Py：预编译正则
来源：http://kd.nszjky.cn

pat = re.compile(r"\d+")
来源：http://xe.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://lt.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lg.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://xo.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://td.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://oz.shxzukj.cn

@contextlib.contextmanager
来源：http://jc.nszjky.cn

[U22] Py：矩阵转置
来源：http://vm.shxzukj.cn

list(zip(*m))
来源：http://tl.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://fl.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tp.asd995.cn

[U24] Py：路径操作
来源：http://gm.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ih.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://rc.yuntaijiaju.cn

csv.DictReader(f)
来源：http://od.wgjwhj.cn

[U26] Py：并发下载
来源：http://ku.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hd.521024.cn

[U27] Py：异步 HTTP
来源：http://xg.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://rv.nszjky.cn

[U28] Py：类型别名
来源：http://dc.nszjky.cn

UserId = int
来源：http://ez.bjjhwx.cn

[U29] Py：属性校验
来源：http://yz.asd995.cn

@property 与 @x.setter 配合
来源：http://ga.huanxung.cn

[U30] Py：数据类
来源：http://ko.521024.cn

@dataclass(slots=True)
来源：http://fz.521024.cn

[U31] Py：单测
来源：http://pt.shxzskj.cn

python -m pytest -q
来源：http://gq.shxzukj.cn

[U32] Py：代码格式化
来源：http://uv.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://kz.szsharing.cn

[U33] Py：打包发布
来源：http://ga.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://le.huanxung.cn

[U34] Py：判断编码
来源：http://yi.newstarts.cn

chardet.detect(raw)
来源：http://ij.wgjwhj.cn

[U35] Py：发送邮件
来源：http://lg.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yz.hahajie.cn

[U36] Py：定时任务
来源：http://re.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://cp.hnjuh.cn

[U37] Py：读写 Excel
来源：http://sd.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://el.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://wf.newstarts.cn

Path(__file__).resolve().parent
来源：http://bk.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://qv.hnjuh.cn

sys.stdout.isatty()
来源：http://gb.huanxung.cn

[U40] Py：打印到标准错误
来源：http://gu.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://ny.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://gv.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jl.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://it.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pl.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://zf.yuexingan06.cn

namespace App\Http;
来源：http://mj.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://wg.yuexingan06.cn

declare(strict_types=1);
来源：http://pj.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://hu.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://si.haigaiapp.cn

[U46] PHP：可空类型
来源：http://ej.521024.cn

?string $name = null
来源：http://do.521024.cn

[U47] PHP：联合类型
来源：http://ph.lnxyls.cn

int|string $id
来源：http://oa.gzmigu.cn

[U48] PHP：纯枚举
来源：http://wb.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xj.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://yd.nszjky.cn

public readonly string $name
来源：http://ue.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://vr.colortex.cn

public function __construct(private int $id) {}
来源：http://un.hahajie.cn

[U51] PHP：数组解构
来源：http://lw.nicolike.cn

[$a, $b] = $arr;
来源：http://gb.asd995.cn

[U52] PHP：箭头函数
来源：http://ut.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://gz.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://he.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://py.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://oe.szsharing.cn

$obj?->method()
来源：http://ka.shxzukj.cn

[U55] PHP：match 表达式
来源：http://am.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ga.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://rp.huixiangedu.cn

f(a: 1, b: 2)
来源：http://ki.shxzskj.cn

[U57] PHP：字符串插值
来源：http://gc.yuexingan06.cn

"值: {$a}"
来源：http://lr.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://gn.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xn.nicolike.cn

[U59] PHP：自定义排序
来源：http://rf.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qp.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://rc.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uk.panjiajie.cn

[U61] PHP：正则
来源：http://ac.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://am.colortex.cn

[U62] PHP：日期对象
来源：http://vk.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wg.asd995.cn

[U63] PHP：文件读写
来源：http://yu.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sa.szxytkj.cn

[U64] PHP：目录遍历
来源：http://sh.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://sg.colortex.cn

[U65] PHP：会话
来源：http://xr.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jy.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://hl.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yj.colortex.cn

[U67] PHP：处理文件上传
来源：http://br.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ig.hahajie.cn

[U68] PHP：PDO 连接
来源：http://ro.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tp.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://rr.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ca.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://dt.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bj.hahajie.cn

[U71] PHP：抛出异常
来源：http://je.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://on.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://wh.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://km.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://cq.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://fq.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://bq.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://oj.newstarts.cn

[U75] PHP：依赖注入
来源：http://ku.muxihuayi.cn

composer require psr/container
来源：http://te.gzmigu.cn

[U76] PHP：简单路由
来源：http://we.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ej.asd995.cn

[U77] PHP：模板渲染
来源：http://wl.yuntaijiaju.cn

composer require twig/twig
来源：http://db.huanxung.cn

[U78] PHP：单元测试
来源：http://pz.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://pv.nszjky.cn


<!-- 参考信息 -->