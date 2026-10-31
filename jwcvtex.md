代发 wailian999

int size() const noexcept { return n_; }
来源：http://ru.jctech888.com.cn

[S53] C++：移动语义
来源：http://jl.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://sg.521024.cn

[S54] C++：异常处理
来源：http://fx.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ua.newstarts.cn

[S55] C++：结构化绑定
来源：http://fs.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ck.szxytkj.cn

[S56] C++：optional
来源：http://cv.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xk.huixiangedu.cn

[S57] C++：编译期常量
来源：http://zk.hnjuh.cn

constexpr int N = 10;
来源：http://ey.bookmarksfly.cn

[S58] C++：命名空间
来源：http://vn.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://pc.muxihuayi.cn

[S59] C++：静态断言
来源：http://db.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ft.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://hh.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uf.shtwfgs.cn

================================================================================
来源：http://yw.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ls.jctech888.com.cn

================================================================================
来源：http://bj.asd995.cn

[T01] Kotlin：Hello World
来源：http://eo.jianghongdianzi.cn

println("Hello")
来源：http://it.newstarts.cn

[T02] Kotlin：变量
来源：http://as.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ws.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://yj.jctech888.com.cn

"值: $b"
来源：http://fi.szsharing.cn

[T04] Kotlin：空安全
来源：http://fx.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://sn.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://sb.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cn.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://ag.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://od.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://kx.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yi.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://id.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://le.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://va.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://yx.szsharing.cn

[T10] Kotlin：默认参数
来源：http://jp.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uv.hahajie.cn

[T11] Kotlin：协程
来源：http://gt.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mx.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://fz.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://ij.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://kz.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://pl.yuexingan06.cn

[T14] Kotlin：循环
来源：http://vg.521024.cn

for (i in 1..10) println(i)
来源：http://hd.szxytkj.cn

[T15] Kotlin：接口
来源：http://vn.asd995.cn

interface Shape { fun area(): Double }
来源：http://bo.hahajie.cn

[T16] Swift：Hello World
来源：http://kw.szsharing.cn

print("Hello")
来源：http://vv.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://ad.huanxung.cn

var a = 1;  let b = 2
来源：http://zo.huanxung.cn

[T18] Swift：字符串插值
来源：http://gf.shxzukj.cn

"值: \(b)"
来源：http://if.panjiajie.cn

[T19] Swift：可选绑定
来源：http://wn.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://hi.shxzskj.cn

[T20] Swift：数组操作
来源：http://yv.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dk.asd995.cn

[T21] Swift：遍历
来源：http://ut.shtwfgs.cn

for x in a { print(x) }
来源：http://yl.wgjwhj.cn

[T22] Swift：字典
来源：http://zd.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qc.szxytkj.cn

[T23] Swift：函数
来源：http://eg.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cv.shxzskj.cn

[T24] Swift：闭包
来源：http://fj.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iq.gzmigu.cn

[T25] Swift：结构体
来源：http://qt.lnxyls.cn

struct P { var x: Int }
来源：http://rs.wgjwhj.cn

[T26] Swift：类与重写
来源：http://dy.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://sk.muxihuayi.cn

[T27] Swift：错误处理
来源：http://wo.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://mz.szxytkj.cn

[T28] Swift：枚举
来源：http://pk.asd995.cn

enum Color { case red, green }
来源：http://xc.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://qv.9csxet.cn

guard let x = opt else { return }
来源：http://zy.lnxyls.cn

[T30] Swift：协议
来源：http://la.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://vc.521024.cn

[T31] Lua：Hello World
来源：http://gk.newstarts.cn

print("Hello")
来源：http://sv.521024.cn

[T32] Lua：局部变量
来源：http://mu.huanxung.cn

local a = 1
来源：http://mm.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://tl.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ay.hnjuh.cn

[T34] Lua：遍历表
来源：http://cd.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bn.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://hl.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://qf.colortex.cn

[T36] Lua：函数
来源：http://pn.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://cg.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://zw.yuntaijiaju.cn

"a" .. "b"
来源：http://xp.shxzskj.cn

[T38] Lua：条件
来源：http://xv.hahajie.cn

if x > 0 then print("正") end
来源：http://lz.szxytkj.cn

[T39] Lua：模式匹配
来源：http://ib.newstarts.cn

string.find(s, "%d+")
来源：http://qi.jctech888.com.cn

[T40] Lua：元表
来源：http://ta.9csxet.cn

setmetatable({}, { __index = base })
来源：http://ir.huixiangedu.cn

[T41] Perl：Hello World
来源：http://tb.nszjky.cn

print "Hello\n";
来源：http://tm.huanxung.cn

[T42] Perl：变量类型
来源：http://sb.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hf.shxzskj.cn

[T43] Perl：字符串插值
来源：http://yp.shtwfgs.cn

"值: $a"
来源：http://cm.szxytkj.cn

[T44] Perl：条件
来源：http://bz.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://ep.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://nv.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://hr.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://wn.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tf.hahajie.cn

[T47] Perl：正则捕获
来源：http://ek.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vc.jctech888.com.cn

[T48] Perl：正则替换
来源：http://rb.gzmigu.cn

$s =~ s/old/new/g;
来源：http://il.szxytkj.cn

[T49] Perl：函数
来源：http://zp.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://do.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://hy.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wi.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://wt.nicolike.cn

[T51] Scala：Hello World
来源：http://fd.shtwfgs.cn

println("Hello")
来源：http://wh.jctech888.com.cn

[T52] Scala：变量
来源：http://wk.panjiajie.cn

val a = 1;  var b = 2
来源：http://iv.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://ph.wgjwhj.cn

s"值: $b"
来源：http://wr.lnxyls.cn

[T54] Scala：集合映射
来源：http://zz.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://bm.nszjky.cn

[T55] Scala：集合过滤
来源：http://yc.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rp.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://zi.shxzskj.cn

case class User(name: String, age: Int)
来源：http://pp.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://dx.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jb.gzmigu.cn

[T58] Scala：函数定义
来源：http://hs.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wg.nszjky.cn

[T59] Scala：循环
来源：http://kg.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://nf.huixiangedu.cn

[T60] Scala：折叠
来源：http://rl.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ux.colortex.cn

================================================================================
来源：http://jk.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fd.haigaiapp.cn

================================================================================
来源：http://zp.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://hb.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ij.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://vy.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cs.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://hs.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sx.nicolike.cn

[U04] Py：变量调试打印
来源：http://du.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bf.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://tk.huanxung.cn

list(dict.fromkeys(arr))
来源：http://iu.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://dg.hnjuh.cn

{**a, **b}
来源：http://hu.gzmigu.cn

[U07] Py：反转字典键值
来源：http://bn.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://fb.nszjky.cn

[U08] Py：展平二维列表
来源：http://sh.shtwfgs.cn

[y for x in nested for y in x]
来源：http://pm.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://op.szxytkj.cn

max(d, key=d.get)
来源：http://al.hnjuh.cn

[U10] Py：按值排序字典
来源：http://if.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lg.9csxet.cn

[U11] Py：生成器表达式
来源：http://ip.colortex.cn

(x * 2 for x in arr)
来源：http://px.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vo.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://zs.hnjuh.cn

[U13] Py：固定长度队列
来源：http://pi.huixinmuqiang.cn

deque(maxlen=10)
来源：http://qp.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://lr.gzmigu.cn

defaultdict(list)
来源：http://ki.521024.cn

[U15] Py：高精度计时
来源：http://eh.yuntaijiaju.cn

t = time.perf_counter()
来源：http://np.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://ur.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oj.newstarts.cn

[U17] Py：初始化日志
来源：http://sd.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://iq.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://hm.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://io.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://du.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yz.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://ef.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://ka.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://wd.bjjhwx.cn

@contextlib.contextmanager
来源：http://in.lnxyls.cn

[U22] Py：矩阵转置
来源：http://hj.asd995.cn

list(zip(*m))
来源：http://sv.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://fl.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kx.hnjuh.cn

[U24] Py：路径操作
来源：http://ed.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aj.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://jk.bookmarksfly.cn

csv.DictReader(f)
来源：http://hn.shtwfgs.cn

[U26] Py：并发下载
来源：http://oq.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qe.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://df.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://ou.haigaiapp.cn

[U28] Py：类型别名
来源：http://ti.wgjwhj.cn

UserId = int
来源：http://zn.hnjuh.cn

[U29] Py：属性校验
来源：http://ml.hnjuh.cn

@property 与 @x.setter 配合
来源：http://oi.hnjuh.cn

[U30] Py：数据类
来源：http://fo.jctech888.com.cn

@dataclass(slots=True)
来源：http://dn.panjiajie.cn

[U31] Py：单测
来源：http://pr.hahajie.cn

python -m pytest -q
来源：http://ww.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://xp.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://al.gzmigu.cn

[U33] Py：打包发布
来源：http://uc.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://kh.lnxyls.cn

[U34] Py：判断编码
来源：http://lg.jianghongdianzi.cn

chardet.detect(raw)
来源：http://kd.shxzskj.cn

[U35] Py：发送邮件
来源：http://mk.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ir.colortex.cn

[U36] Py：定时任务
来源：http://on.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://lo.9csxet.cn

[U37] Py：读写 Excel
来源：http://gs.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://em.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://td.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://dm.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://ny.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://hz.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://wd.szxytkj.cn

print("err", file=sys.stderr)
来源：http://bx.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ui.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wv.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://sb.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oy.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://aw.nszjky.cn

namespace App\Http;
来源：http://vm.nszjky.cn

[U44] PHP：开启严格类型
来源：http://or.shtwfgs.cn

declare(strict_types=1);
来源：http://my.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://vu.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://or.jctech888.com.cn

[U46] PHP：可空类型
来源：http://wo.hnjuh.cn

?string $name = null
来源：http://pt.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://gq.asd995.cn

int|string $id
来源：http://og.gzmigu.cn

[U48] PHP：纯枚举
来源：http://gk.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bt.panjiajie.cn

[U49] PHP：只读属性
来源：http://yd.colortex.cn

public readonly string $name
来源：http://vj.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://eo.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://vd.asd995.cn

[U51] PHP：数组解构
来源：http://oq.newstarts.cn

[$a, $b] = $arr;
来源：http://ba.szsharing.cn

[U52] PHP：箭头函数
来源：http://td.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://qy.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://wj.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://lf.szsharing.cn

[U54] PHP：空安全调用
来源：http://tk.9csxet.cn

$obj?->method()
来源：http://pz.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://ti.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hb.huixiangedu.cn

[U56] PHP：命名参数
来源：http://po.yuexingan06.cn

f(a: 1, b: 2)
来源：http://qd.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://ug.jianghongdianzi.cn

"值: {$a}"
来源：http://jv.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://oj.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kz.huanxung.cn

[U59] PHP：自定义排序
来源：http://le.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zu.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://mp.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lo.panjiajie.cn

[U61] PHP：正则
来源：http://fd.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bb.muxihuayi.cn

[U62] PHP：日期对象
来源：http://sc.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zs.shtwfgs.cn

[U63] PHP：文件读写
来源：http://kg.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://an.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://by.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://hg.nszjky.cn

[U65] PHP：会话
来源：http://ar.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gf.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://vl.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lo.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://kg.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fe.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://cx.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wa.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://bk.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://if.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://oo.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lm.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://ib.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://gj.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://bg.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://qp.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://lb.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://mx.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://gu.yuexingan06.cn

getenv("APP_ENV") ?: "production"
来源：http://sn.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://ti.jctech888.com.cn

composer require psr/container
来源：http://pl.shxzukj.cn

[U76] PHP：简单路由
来源：http://rd.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gv.nszjky.cn

[U77] PHP：模板渲染
来源：http://qd.huixiangedu.cn

composer require twig/twig
来源：http://ox.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://uw.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://hy.lnxyls.cn


<!-- 参考信息 -->