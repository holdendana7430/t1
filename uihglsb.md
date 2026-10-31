代发 wailian999

int size() const noexcept { return n_; }
来源：http://ag.gzmigu.cn

[S53] C++：移动语义
来源：http://zz.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://ry.szsharing.cn

[S54] C++：异常处理
来源：http://eh.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zy.hahajie.cn

[S55] C++：结构化绑定
来源：http://pr.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fy.huixiangedu.cn

[S56] C++：optional
来源：http://xj.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://he.haigaiapp.cn

[S57] C++：编译期常量
来源：http://fq.asd995.cn

constexpr int N = 10;
来源：http://xg.szxytkj.cn

[S58] C++：命名空间
来源：http://qv.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://io.newstarts.cn

[S59] C++：静态断言
来源：http://ge.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wm.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://co.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qf.lnxyls.cn

================================================================================
来源：http://nr.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://li.hahajie.cn

================================================================================
来源：http://zp.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://et.colortex.cn

println("Hello")
来源：http://av.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://wl.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vi.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://mt.wgjwhj.cn

"值: $b"
来源：http://ga.lnxyls.cn

[T04] Kotlin：空安全
来源：http://gz.panjiajie.cn

val n: String? = null;  n?.length
来源：http://zy.521024.cn

[T05] Kotlin：when 表达式
来源：http://yk.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vk.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://ng.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yh.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://iu.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bo.huanxung.cn

[T08] Kotlin：数据类
来源：http://za.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://yo.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://pa.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://zs.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://nr.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://je.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://wh.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sd.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://eh.521024.cn

val (a, b) = Pair(1, 2)
来源：http://nt.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://rc.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://bi.colortex.cn

[T14] Kotlin：循环
来源：http://qn.shxzskj.cn

for (i in 1..10) println(i)
来源：http://mi.yuexingan06.cn

[T15] Kotlin：接口
来源：http://xs.521024.cn

interface Shape { fun area(): Double }
来源：http://to.nicolike.cn

[T16] Swift：Hello World
来源：http://eo.nicolike.cn

print("Hello")
来源：http://yx.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://px.9csxet.cn

var a = 1;  let b = 2
来源：http://wl.hahajie.cn

[T18] Swift：字符串插值
来源：http://xb.hnjuh.cn

"值: \(b)"
来源：http://lh.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://oj.shxzukj.cn

if let n = opt { print(n) }
来源：http://uu.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://ff.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://df.gzmigu.cn

[T21] Swift：遍历
来源：http://bq.jianghongdianzi.cn

for x in a { print(x) }
来源：http://fo.hnjuh.cn

[T22] Swift：字典
来源：http://rz.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ly.muxihuayi.cn

[T23] Swift：函数
来源：http://yx.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xz.muxihuayi.cn

[T24] Swift：闭包
来源：http://jv.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ox.521024.cn

[T25] Swift：结构体
来源：http://ux.panjiajie.cn

struct P { var x: Int }
来源：http://yo.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://iw.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://pq.jctech888.com.cn

[T27] Swift：错误处理
来源：http://bf.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://kc.chemitech.net.cn

[T28] Swift：枚举
来源：http://dz.newstarts.cn

enum Color { case red, green }
来源：http://jb.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://fd.szsharing.cn

guard let x = opt else { return }
来源：http://sb.szxytkj.cn

[T30] Swift：协议
来源：http://hf.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://ji.jctech888.com.cn

[T31] Lua：Hello World
来源：http://du.haigaiapp.cn

print("Hello")
来源：http://ed.haigaiapp.cn

[T32] Lua：局部变量
来源：http://ck.yuntaijiaju.cn

local a = 1
来源：http://ra.9csxet.cn

[T33] Lua：表（数组）
来源：http://gf.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://eb.muxihuayi.cn

[T34] Lua：遍历表
来源：http://nw.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mi.haigaiapp.cn

[T35] Lua：字典表
来源：http://sa.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://zz.nszjky.cn

[T36] Lua：函数
来源：http://fo.huixiangedu.cn

function add(a, b) return a + b end
来源：http://hc.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://sj.huixinmuqiang.cn

"a" .. "b"
来源：http://po.521024.cn

[T38] Lua：条件
来源：http://le.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://mc.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://lv.nicolike.cn

string.find(s, "%d+")
来源：http://mh.nicolike.cn

[T40] Lua：元表
来源：http://ug.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://mb.gzmigu.cn

[T41] Perl：Hello World
来源：http://mu.shxzukj.cn

print "Hello\n";
来源：http://px.panjiajie.cn

[T42] Perl：变量类型
来源：http://kh.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cv.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://oo.asd995.cn

"值: $a"
来源：http://aj.lnxyls.cn

[T44] Perl：条件
来源：http://na.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://wa.hahajie.cn

[T45] Perl：数组遍历
来源：http://je.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://ju.nszjky.cn

[T46] Perl：哈希操作
来源：http://hj.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lk.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://iu.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pf.szxytkj.cn

[T48] Perl：正则替换
来源：http://ay.newstarts.cn

$s =~ s/old/new/g;
来源：http://ww.shxzskj.cn

[T49] Perl：函数
来源：http://mu.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ov.huanxung.cn

[T50] Perl：逐行读文件
来源：http://of.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xt.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://pg.hahajie.cn

[T51] Scala：Hello World
来源：http://kz.yuntaijiaju.cn

println("Hello")
来源：http://av.bookmarksfly.cn

[T52] Scala：变量
来源：http://ov.hahajie.cn

val a = 1;  var b = 2
来源：http://dx.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://tw.9csxet.cn

s"值: $b"
来源：http://cp.shxzukj.cn

[T54] Scala：集合映射
来源：http://uw.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://mp.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://sz.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ha.szsharing.cn

[T56] Scala：样例类
来源：http://vr.hnjuh.cn

case class User(name: String, age: Int)
来源：http://eh.colortex.cn

[T57] Scala：模式匹配
来源：http://rj.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uj.nszjky.cn

[T58] Scala：函数定义
来源：http://dh.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://aw.panjiajie.cn

[T59] Scala：循环
来源：http://gw.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://dk.nszjky.cn

[T60] Scala：折叠
来源：http://tb.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eb.hahajie.cn

================================================================================
来源：http://bz.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://un.nszjky.cn

================================================================================
来源：http://gd.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://yh.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nb.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://vz.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wq.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://dh.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jm.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://qu.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ak.newstarts.cn

[U05] Py：列表去重且保序
来源：http://jq.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://bu.nszjky.cn

[U06] Py：合并两个字典
来源：http://hs.bookmarksfly.cn

{**a, **b}
来源：http://vg.gzmigu.cn

[U07] Py：反转字典键值
来源：http://ce.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://pm.asd995.cn

[U08] Py：展平二维列表
来源：http://yr.huixiangedu.cn

[y for x in nested for y in x]
来源：http://hy.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://td.huixinmuqiang.cn

max(d, key=d.get)
来源：http://la.newstarts.cn

[U10] Py：按值排序字典
来源：http://gw.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://li.huanxung.cn

[U11] Py：生成器表达式
来源：http://rh.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://ai.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://su.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://ky.521024.cn

[U13] Py：固定长度队列
来源：http://vg.huixiangedu.cn

deque(maxlen=10)
来源：http://ik.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://mu.shtwfgs.cn

defaultdict(list)
来源：http://zl.panjiajie.cn

[U15] Py：高精度计时
来源：http://yv.lnxyls.cn

t = time.perf_counter()
来源：http://ad.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://xq.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uc.hnjuh.cn

[U17] Py：初始化日志
来源：http://ai.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://nl.yuexingan06.cn

[U18] Py：预编译正则
来源：http://ep.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://os.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://ae.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uw.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://kk.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://jc.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://oy.muxihuayi.cn

@contextlib.contextmanager
来源：http://ti.shxzskj.cn

[U22] Py：矩阵转置
来源：http://pz.szxytkj.cn

list(zip(*m))
来源：http://bd.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://rs.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ld.yuexingan06.cn

[U24] Py：路径操作
来源：http://hp.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://im.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://nk.muxihuayi.cn

csv.DictReader(f)
来源：http://gd.521024.cn

[U26] Py：并发下载
来源：http://uk.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oq.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://sz.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://nf.asd995.cn

[U28] Py：类型别名
来源：http://yb.wgjwhj.cn

UserId = int
来源：http://us.521024.cn

[U29] Py：属性校验
来源：http://km.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://hv.yuntaijiaju.cn

[U30] Py：数据类
来源：http://gw.newstarts.cn

@dataclass(slots=True)
来源：http://pp.chemitech.net.cn

[U31] Py：单测
来源：http://by.huanxung.cn

python -m pytest -q
来源：http://qj.chemitech.net.cn

[U32] Py：代码格式化
来源：http://tt.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://ur.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://ns.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://de.shtwfgs.cn

[U34] Py：判断编码
来源：http://hl.hahajie.cn

chardet.detect(raw)
来源：http://bh.lnxyls.cn

[U35] Py：发送邮件
来源：http://kr.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cn.haigaiapp.cn

[U36] Py：定时任务
来源：http://zg.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://db.hahajie.cn

[U37] Py：读写 Excel
来源：http://rc.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zs.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://kb.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://gg.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://al.panjiajie.cn

sys.stdout.isatty()
来源：http://fl.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://ey.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://yx.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://tf.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bg.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://ng.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sf.9csxet.cn

[U43] PHP：声明命名空间
来源：http://wi.521024.cn

namespace App\Http;
来源：http://ub.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://ml.9csxet.cn

declare(strict_types=1);
来源：http://uk.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://ie.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xb.yuexingan06.cn

[U46] PHP：可空类型
来源：http://zp.shxzskj.cn

?string $name = null
来源：http://ee.wgjwhj.cn

[U47] PHP：联合类型
来源：http://wb.shtwfgs.cn

int|string $id
来源：http://pt.huanxung.cn

[U48] PHP：纯枚举
来源：http://vm.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ql.521024.cn

[U49] PHP：只读属性
来源：http://oq.asd995.cn

public readonly string $name
来源：http://jk.521024.cn

[U50] PHP：构造器属性提升
来源：http://he.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://ls.haigaiapp.cn

[U51] PHP：数组解构
来源：http://lr.hnjuh.cn

[$a, $b] = $arr;
来源：http://dt.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://hq.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://qx.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://vw.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://ai.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://fe.nicolike.cn

$obj?->method()
来源：http://qa.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://zn.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yb.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://fb.muxihuayi.cn

f(a: 1, b: 2)
来源：http://df.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://nt.yuexingan06.cn

"值: {$a}"
来源：http://bx.nszjky.cn

[U58] PHP：数组三件套
来源：http://mb.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ag.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://wa.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gp.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://yr.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uy.gzmigu.cn

[U61] PHP：正则
来源：http://fg.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sz.asd995.cn

[U62] PHP：日期对象
来源：http://kw.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yq.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://vf.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dw.nszjky.cn

[U64] PHP：目录遍历
来源：http://sn.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://ss.yuntaijiaju.cn

[U65] PHP：会话
来源：http://hw.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ru.asd995.cn

[U66] PHP：设置 Cookie
来源：http://lr.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bh.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://aa.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gs.colortex.cn

[U68] PHP：PDO 连接
来源：http://lg.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://og.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://fn.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qn.huanxung.cn

[U70] PHP：PDO 事务
来源：http://pk.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ff.shxzukj.cn

[U71] PHP：抛出异常
来源：http://wi.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://mq.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://bd.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://tz.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://lt.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://yd.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://kc.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://pr.szxytkj.cn

[U75] PHP：依赖注入
来源：http://km.shxzukj.cn

composer require psr/container
来源：http://ix.bjjhwx.cn

[U76] PHP：简单路由
来源：http://rw.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ew.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://gb.gzmigu.cn

composer require twig/twig
来源：http://lr.shtwfgs.cn

[U78] PHP：单元测试
来源：http://sj.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://eg.9csxet.cn


<!-- 参考信息 -->