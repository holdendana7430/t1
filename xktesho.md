代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://nv.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://va.newstarts.cn

[S48] C++：逐行读文件
来源：http://ga.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iz.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://my.huixiangedu.cn

[S49] C++：写文件
来源：http://jl.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ss.shxzukj.cn

[S50] C++：格式化数字
来源：http://pb.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sz.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://gm.newstarts.cn

static_cast<double>(a) / b
来源：http://nj.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://fy.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://np.bookmarksfly.cn

[S53] C++：移动语义
来源：http://cb.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://jc.muxihuayi.cn

[S54] C++：异常处理
来源：http://gs.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kj.hnjuh.cn

[S55] C++：结构化绑定
来源：http://fi.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bx.bjjhwx.cn

[S56] C++：optional
来源：http://hf.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nq.muxihuayi.cn

[S57] C++：编译期常量
来源：http://zg.huixinmuqiang.cn

constexpr int N = 10;
来源：http://nv.521024.cn

[S58] C++：命名空间
来源：http://wm.521024.cn

namespace ns { int f() { return 1; } }
来源：http://bf.szsharing.cn

[S59] C++：静态断言
来源：http://ur.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://do.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://ac.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sy.bjjhwx.cn

================================================================================
来源：http://nj.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://he.colortex.cn

================================================================================
来源：http://pi.hahajie.cn

[T01] Kotlin：Hello World
来源：http://rs.lnxyls.cn

println("Hello")
来源：http://nw.521024.cn

[T02] Kotlin：变量
来源：http://id.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ca.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://sp.shxzskj.cn

"值: $b"
来源：http://qo.lnxyls.cn

[T04] Kotlin：空安全
来源：http://so.panjiajie.cn

val n: String? = null;  n?.length
来源：http://io.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://zm.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mw.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://nt.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kg.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://os.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yl.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://rc.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://xo.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://qh.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://es.szsharing.cn

[T10] Kotlin：默认参数
来源：http://ga.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bj.9csxet.cn

[T11] Kotlin：协程
来源：http://zg.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ue.newstarts.cn

[T12] Kotlin：解构声明
来源：http://ir.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://iv.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://cm.521024.cn

val m = mapOf("a" to 1)
来源：http://ds.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://mc.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://xc.nicolike.cn

[T15] Kotlin：接口
来源：http://gw.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://rp.jctech888.com.cn

[T16] Swift：Hello World
来源：http://zm.panjiajie.cn

print("Hello")
来源：http://to.asd995.cn

[T17] Swift：变量与常量
来源：http://gg.bjjhwx.cn

var a = 1;  let b = 2
来源：http://lu.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://xt.jianghongdianzi.cn

"值: \(b)"
来源：http://uh.nicolike.cn

[T19] Swift：可选绑定
来源：http://sp.huixiangedu.cn

if let n = opt { print(n) }
来源：http://ub.bjjhwx.cn

[T20] Swift：数组操作
来源：http://oa.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://za.szxytkj.cn

[T21] Swift：遍历
来源：http://ot.haigaiapp.cn

for x in a { print(x) }
来源：http://re.muxihuayi.cn

[T22] Swift：字典
来源：http://pw.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://py.lnxyls.cn

[T23] Swift：函数
来源：http://ph.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dj.gzmigu.cn

[T24] Swift：闭包
来源：http://yh.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ka.colortex.cn

[T25] Swift：结构体
来源：http://bs.hnjuh.cn

struct P { var x: Int }
来源：http://xt.haigaiapp.cn

[T26] Swift：类与重写
来源：http://zr.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://on.asd995.cn

[T27] Swift：错误处理
来源：http://tu.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://jy.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://cb.jctech888.com.cn

enum Color { case red, green }
来源：http://ae.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://uw.shxzukj.cn

guard let x = opt else { return }
来源：http://pu.panjiajie.cn

[T30] Swift：协议
来源：http://rf.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://qn.hnjuh.cn

[T31] Lua：Hello World
来源：http://cb.bookmarksfly.cn

print("Hello")
来源：http://mh.szsharing.cn

[T32] Lua：局部变量
来源：http://uc.jctech888.com.cn

local a = 1
来源：http://yd.panjiajie.cn

[T33] Lua：表（数组）
来源：http://wi.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mq.shxzukj.cn

[T34] Lua：遍历表
来源：http://bn.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ug.nicolike.cn

[T35] Lua：字典表
来源：http://rl.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://qw.bookmarksfly.cn

[T36] Lua：函数
来源：http://zp.yuexingan06.cn

function add(a, b) return a + b end
来源：http://kq.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://dk.nicolike.cn

"a" .. "b"
来源：http://jk.jctech888.com.cn

[T38] Lua：条件
来源：http://qt.huanxung.cn

if x > 0 then print("正") end
来源：http://uu.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://fy.newstarts.cn

string.find(s, "%d+")
来源：http://oh.hahajie.cn

[T40] Lua：元表
来源：http://fq.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://uu.yuexingan06.cn

[T41] Perl：Hello World
来源：http://we.bookmarksfly.cn

print "Hello\n";
来源：http://hv.shxzskj.cn

[T42] Perl：变量类型
来源：http://iv.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ob.newstarts.cn

[T43] Perl：字符串插值
来源：http://hd.huixiangedu.cn

"值: $a"
来源：http://ex.muxihuayi.cn

[T44] Perl：条件
来源：http://ub.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://nf.newstarts.cn

[T45] Perl：数组遍历
来源：http://xk.521024.cn

for my $x (@arr) { print $x; }
来源：http://vf.lnxyls.cn

[T46] Perl：哈希操作
来源：http://bw.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jv.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://pd.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ta.newstarts.cn

[T48] Perl：正则替换
来源：http://dp.lnxyls.cn

$s =~ s/old/new/g;
来源：http://uf.newstarts.cn

[T49] Perl：函数
来源：http://pf.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cu.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://dj.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qe.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://kf.huixiangedu.cn

[T51] Scala：Hello World
来源：http://od.muxihuayi.cn

println("Hello")
来源：http://dq.yuexingan06.cn

[T52] Scala：变量
来源：http://qo.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://yo.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://hf.nicolike.cn

s"值: $b"
来源：http://dd.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://nu.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://wj.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://qw.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dm.yuexingan06.cn

[T56] Scala：样例类
来源：http://kn.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://lw.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://ya.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jl.gzmigu.cn

[T58] Scala：函数定义
来源：http://za.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ss.shxzskj.cn

[T59] Scala：循环
来源：http://ko.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://ni.shtwfgs.cn

[T60] Scala：折叠
来源：http://tf.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vn.panjiajie.cn

================================================================================
来源：http://in.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bb.newstarts.cn

================================================================================
来源：http://tt.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://oh.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://si.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://wo.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uf.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://bj.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hj.nicolike.cn

[U04] Py：变量调试打印
来源：http://ct.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ts.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://fw.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://sq.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://sv.muxihuayi.cn

{**a, **b}
来源：http://bi.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://xv.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://nv.asd995.cn

[U08] Py：展平二维列表
来源：http://ke.szxytkj.cn

[y for x in nested for y in x]
来源：http://dx.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://mj.nszjky.cn

max(d, key=d.get)
来源：http://oq.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://sw.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ma.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://er.yuexingan06.cn

(x * 2 for x in arr)
来源：http://cl.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qm.hahajie.cn

Counter(arr).most_common(3)
来源：http://if.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://dp.bookmarksfly.cn

deque(maxlen=10)
来源：http://wd.asd995.cn

[U14] Py：分组收集到列表
来源：http://lr.bjjhwx.cn

defaultdict(list)
来源：http://js.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://pa.hahajie.cn

t = time.perf_counter()
来源：http://ln.szsharing.cn

[U16] Py：命令行参数解析
来源：http://vt.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xp.newstarts.cn

[U17] Py：初始化日志
来源：http://it.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://dq.huanxung.cn

[U18] Py：预编译正则
来源：http://xq.nicolike.cn

pat = re.compile(r"\d+")
来源：http://oy.huanxung.cn

[U19] Py：正则替换带回调
来源：http://rf.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ma.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://pr.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://kx.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://tj.szxytkj.cn

@contextlib.contextmanager
来源：http://ce.nszjky.cn

[U22] Py：矩阵转置
来源：http://kt.newstarts.cn

list(zip(*m))
来源：http://py.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://ev.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sf.wgjwhj.cn

[U24] Py：路径操作
来源：http://gb.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zc.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://ht.chemitech.net.cn

csv.DictReader(f)
来源：http://si.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://ae.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xb.nicolike.cn

[U27] Py：异步 HTTP
来源：http://fd.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://va.9csxet.cn

[U28] Py：类型别名
来源：http://il.huixinmuqiang.cn

UserId = int
来源：http://vp.nicolike.cn

[U29] Py：属性校验
来源：http://cq.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://ir.shtwfgs.cn

[U30] Py：数据类
来源：http://an.szxytkj.cn

@dataclass(slots=True)
来源：http://lz.nicolike.cn

[U31] Py：单测
来源：http://db.huixinmuqiang.cn

python -m pytest -q
来源：http://mj.nszjky.cn

[U32] Py：代码格式化
来源：http://uk.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://xu.lnxyls.cn

[U33] Py：打包发布
来源：http://sf.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://cz.colortex.cn

[U34] Py：判断编码
来源：http://mr.huixiangedu.cn

chardet.detect(raw)
来源：http://ea.nicolike.cn

[U35] Py：发送邮件
来源：http://rj.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yn.521024.cn

[U36] Py：定时任务
来源：http://vr.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://yh.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://qr.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ra.521024.cn

[U38] Py：获取脚本所在目录
来源：http://em.hahajie.cn

Path(__file__).resolve().parent
来源：http://xz.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://mv.hahajie.cn

sys.stdout.isatty()
来源：http://ku.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://ag.gzmigu.cn

print("err", file=sys.stderr)
来源：http://gv.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://la.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://iu.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://he.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fi.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://mn.yuntaijiaju.cn

namespace App\Http;
来源：http://et.521024.cn

[U44] PHP：开启严格类型
来源：http://gl.huanxung.cn

declare(strict_types=1);
来源：http://kz.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://md.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tl.newstarts.cn

[U46] PHP：可空类型
来源：http://ll.yuexingan06.cn

?string $name = null
来源：http://uu.hahajie.cn

[U47] PHP：联合类型
来源：http://mo.newstarts.cn

int|string $id
来源：http://ax.shxzukj.cn

[U48] PHP：纯枚举
来源：http://uy.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nh.yuexingan06.cn

[U49] PHP：只读属性
来源：http://qh.szxytkj.cn

public readonly string $name
来源：http://am.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://ic.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://li.szsharing.cn

[U51] PHP：数组解构
来源：http://pm.lnxyls.cn

[$a, $b] = $arr;
来源：http://qv.colortex.cn

[U52] PHP：箭头函数
来源：http://nf.asd995.cn

$double = fn($x) => $x * 2;
来源：http://gb.huanxung.cn

[U53] PHP：空合并运算符
来源：http://uc.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://kc.lnxyls.cn

[U54] PHP：空安全调用
来源：http://zs.hnjuh.cn

$obj?->method()
来源：http://px.9csxet.cn

[U55] PHP：match 表达式
来源：http://di.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://le.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://id.asd995.cn

f(a: 1, b: 2)
来源：http://nr.chemitech.net.cn

[U57] PHP：字符串插值
来源：http://uj.huanxung.cn

"值: {$a}"
来源：http://lm.nszjky.cn

[U58] PHP：数组三件套
来源：http://mh.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sp.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://hy.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tn.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://vg.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hv.panjiajie.cn

[U61] PHP：正则
来源：http://bx.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rc.chemitech.net.cn

[U62] PHP：日期对象
来源：http://zh.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://em.huanxung.cn

[U63] PHP：文件读写
来源：http://he.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ut.shxzukj.cn

[U64] PHP：目录遍历
来源：http://mr.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://ih.asd995.cn

[U65] PHP：会话
来源：http://gl.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ry.521024.cn

[U66] PHP：设置 Cookie
来源：http://np.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vt.9csxet.cn

[U67] PHP：处理文件上传
来源：http://gx.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fb.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://ge.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://il.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://fc.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fy.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://tk.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eg.shxzskj.cn

[U71] PHP：抛出异常
来源：http://cn.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://oc.9csxet.cn

[U72] PHP：写错误日志
来源：http://pw.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://nd.jctech888.com.cn


<!-- 参考信息 -->