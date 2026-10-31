代发 wailian999

while (std::getline(in, line)) { }
来源：http://pt.yuexingan06.cn

[S49] C++：写文件
来源：http://zf.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ug.asd995.cn

[S50] C++：格式化数字
来源：http://cg.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kw.szxytkj.cn

[S51] C++：显式类型转换
来源：http://zi.chemitech.net.cn

static_cast<double>(a) / b
来源：http://iw.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://xb.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://ej.panjiajie.cn

[S53] C++：移动语义
来源：http://hu.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://pn.hnjuh.cn

[S54] C++：异常处理
来源：http://xk.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://av.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://tp.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cy.jctech888.com.cn

[S56] C++：optional
来源：http://up.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mm.haigaiapp.cn

[S57] C++：编译期常量
来源：http://fe.shxzskj.cn

constexpr int N = 10;
来源：http://kk.wgjwhj.cn

[S58] C++：命名空间
来源：http://bz.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://is.bjjhwx.cn

[S59] C++：静态断言
来源：http://yr.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gh.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://ih.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vl.bjjhwx.cn

================================================================================
来源：http://xn.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aw.yuexingan06.cn

================================================================================
来源：http://qb.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://ms.gzmigu.cn

println("Hello")
来源：http://lg.newstarts.cn

[T02] Kotlin：变量
来源：http://xz.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ni.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://bu.haigaiapp.cn

"值: $b"
来源：http://yk.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://kp.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://lp.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://em.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kf.newstarts.cn

[T06] Kotlin：集合映射
来源：http://da.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zp.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://ln.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://br.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://px.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://kl.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://zs.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://wh.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://nn.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lq.muxihuayi.cn

[T11] Kotlin：协程
来源：http://oo.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pb.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://pi.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://by.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://co.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://bh.muxihuayi.cn

[T14] Kotlin：循环
来源：http://nq.szsharing.cn

for (i in 1..10) println(i)
来源：http://hi.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://wh.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://ze.muxihuayi.cn

[T16] Swift：Hello World
来源：http://nx.nszjky.cn

print("Hello")
来源：http://mb.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://or.yuexingan06.cn

var a = 1;  let b = 2
来源：http://uf.nszjky.cn

[T18] Swift：字符串插值
来源：http://jn.shtwfgs.cn

"值: \(b)"
来源：http://ur.hnjuh.cn

[T19] Swift：可选绑定
来源：http://vl.lnxyls.cn

if let n = opt { print(n) }
来源：http://gj.muxihuayi.cn

[T20] Swift：数组操作
来源：http://ke.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ye.nszjky.cn

[T21] Swift：遍历
来源：http://cb.521024.cn

for x in a { print(x) }
来源：http://pp.gzmigu.cn

[T22] Swift：字典
来源：http://dj.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://up.bookmarksfly.cn

[T23] Swift：函数
来源：http://uv.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gf.shtwfgs.cn

[T24] Swift：闭包
来源：http://as.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nz.shtwfgs.cn

[T25] Swift：结构体
来源：http://qp.haigaiapp.cn

struct P { var x: Int }
来源：http://hi.521024.cn

[T26] Swift：类与重写
来源：http://zd.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://jz.nicolike.cn

[T27] Swift：错误处理
来源：http://om.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://lz.panjiajie.cn

[T28] Swift：枚举
来源：http://vp.jianghongdianzi.cn

enum Color { case red, green }
来源：http://wz.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://ac.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://ce.muxihuayi.cn

[T30] Swift：协议
来源：http://kz.asd995.cn

protocol Shape { func area() -> Double }
来源：http://hi.shtwfgs.cn

[T31] Lua：Hello World
来源：http://zs.yuntaijiaju.cn

print("Hello")
来源：http://dw.521024.cn

[T32] Lua：局部变量
来源：http://vs.bjjhwx.cn

local a = 1
来源：http://te.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://go.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xn.lnxyls.cn

[T34] Lua：遍历表
来源：http://dm.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ly.panjiajie.cn

[T35] Lua：字典表
来源：http://xn.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://hr.haigaiapp.cn

[T36] Lua：函数
来源：http://kh.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://kr.asd995.cn

[T37] Lua：字符串拼接
来源：http://wv.lnxyls.cn

"a" .. "b"
来源：http://zl.szxytkj.cn

[T38] Lua：条件
来源：http://yw.shxzukj.cn

if x > 0 then print("正") end
来源：http://pk.szsharing.cn

[T39] Lua：模式匹配
来源：http://ts.jctech888.com.cn

string.find(s, "%d+")
来源：http://sb.huanxung.cn

[T40] Lua：元表
来源：http://tz.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://bq.haigaiapp.cn

[T41] Perl：Hello World
来源：http://bi.asd995.cn

print "Hello\n";
来源：http://so.haigaiapp.cn

[T42] Perl：变量类型
来源：http://vc.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cn.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://ge.521024.cn

"值: $a"
来源：http://tj.haigaiapp.cn

[T44] Perl：条件
来源：http://ql.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://rc.szsharing.cn

[T45] Perl：数组遍历
来源：http://xy.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://wr.nszjky.cn

[T46] Perl：哈希操作
来源：http://ey.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mb.521024.cn

[T47] Perl：正则捕获
来源：http://gb.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ni.shtwfgs.cn

[T48] Perl：正则替换
来源：http://ja.nicolike.cn

$s =~ s/old/new/g;
来源：http://ex.yuexingan06.cn

[T49] Perl：函数
来源：http://bx.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lc.szsharing.cn

[T50] Perl：逐行读文件
来源：http://qg.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cj.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://dr.huixiangedu.cn

[T51] Scala：Hello World
来源：http://ps.huanxung.cn

println("Hello")
来源：http://ul.shxzskj.cn

[T52] Scala：变量
来源：http://wk.shxzukj.cn

val a = 1;  var b = 2
来源：http://vv.nszjky.cn

[T53] Scala：字符串插值
来源：http://cz.hahajie.cn

s"值: $b"
来源：http://fe.shxzskj.cn

[T54] Scala：集合映射
来源：http://mi.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://tx.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://kj.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xs.haigaiapp.cn

[T56] Scala：样例类
来源：http://wx.lnxyls.cn

case class User(name: String, age: Int)
来源：http://te.hnjuh.cn

[T57] Scala：模式匹配
来源：http://io.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jl.shxzskj.cn

[T58] Scala：函数定义
来源：http://xn.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://em.newstarts.cn

[T59] Scala：循环
来源：http://lj.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://yo.bookmarksfly.cn

[T60] Scala：折叠
来源：http://cz.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wv.nicolike.cn

================================================================================
来源：http://rl.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rv.shxzukj.cn

================================================================================
来源：http://tq.asd995.cn

[U01] Py：创建虚拟环境
来源：http://tb.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rg.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://wo.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://le.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://xi.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rg.nicolike.cn

[U04] Py：变量调试打印
来源：http://oq.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tf.szsharing.cn

[U05] Py：列表去重且保序
来源：http://pc.newstarts.cn

list(dict.fromkeys(arr))
来源：http://ol.hahajie.cn

[U06] Py：合并两个字典
来源：http://kp.asd995.cn

{**a, **b}
来源：http://fx.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://mz.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://pm.szsharing.cn

[U08] Py：展平二维列表
来源：http://vr.bjjhwx.cn

[y for x in nested for y in x]
来源：http://en.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://kb.gzmigu.cn

max(d, key=d.get)
来源：http://jn.521024.cn

[U10] Py：按值排序字典
来源：http://ci.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ex.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://jd.yuexingan06.cn

(x * 2 for x in arr)
来源：http://yn.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xg.nszjky.cn

Counter(arr).most_common(3)
来源：http://wi.colortex.cn

[U13] Py：固定长度队列
来源：http://bq.huixiangedu.cn

deque(maxlen=10)
来源：http://cw.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://dm.shtwfgs.cn

defaultdict(list)
来源：http://vx.jctech888.com.cn

[U15] Py：高精度计时
来源：http://on.hahajie.cn

t = time.perf_counter()
来源：http://yl.asd995.cn

[U16] Py：命令行参数解析
来源：http://aw.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mb.nicolike.cn

[U17] Py：初始化日志
来源：http://js.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://to.jctech888.com.cn

[U18] Py：预编译正则
来源：http://wb.521024.cn

pat = re.compile(r"\d+")
来源：http://be.9csxet.cn

[U19] Py：正则替换带回调
来源：http://al.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pk.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://ky.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://zc.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://zf.bookmarksfly.cn

@contextlib.contextmanager
来源：http://nr.szsharing.cn

[U22] Py：矩阵转置
来源：http://qv.shxzukj.cn

list(zip(*m))
来源：http://qp.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://lm.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wj.521024.cn

[U24] Py：路径操作
来源：http://tc.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://il.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://jt.haigaiapp.cn

csv.DictReader(f)
来源：http://rn.haigaiapp.cn

[U26] Py：并发下载
来源：http://ab.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yy.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://fz.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://bj.bookmarksfly.cn

[U28] Py：类型别名
来源：http://vz.nicolike.cn

UserId = int
来源：http://kv.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://dz.shxzukj.cn

@property 与 @x.setter 配合
来源：http://mw.szxytkj.cn

[U30] Py：数据类
来源：http://dk.huanxung.cn

@dataclass(slots=True)
来源：http://we.huixiangedu.cn

[U31] Py：单测
来源：http://zh.jianghongdianzi.cn

python -m pytest -q
来源：http://sm.szsharing.cn

[U32] Py：代码格式化
来源：http://oy.asd995.cn

ruff format . && ruff check --fix .
来源：http://fl.shxzukj.cn

[U33] Py：打包发布
来源：http://js.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://aq.panjiajie.cn

[U34] Py：判断编码
来源：http://za.huixiangedu.cn

chardet.detect(raw)
来源：http://sd.haigaiapp.cn

[U35] Py：发送邮件
来源：http://hn.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cn.nszjky.cn

[U36] Py：定时任务
来源：http://fs.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://fj.hahajie.cn

[U37] Py：读写 Excel
来源：http://zf.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gq.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://ym.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://pd.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://sv.shxzskj.cn

sys.stdout.isatty()
来源：http://uy.asd995.cn

[U40] Py：打印到标准错误
来源：http://fr.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://ty.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://ud.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vw.chemitech.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://kc.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ik.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://qi.yuexingan06.cn

namespace App\Http;
来源：http://wy.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://py.bookmarksfly.cn

declare(strict_types=1);
来源：http://dd.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://qj.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fu.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://ym.huixiangedu.cn

?string $name = null
来源：http://rd.shtwfgs.cn

[U47] PHP：联合类型
来源：http://di.szxytkj.cn

int|string $id
来源：http://wt.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://ad.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://st.nicolike.cn

[U49] PHP：只读属性
来源：http://tk.9csxet.cn

public readonly string $name
来源：http://ec.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://mj.asd995.cn

public function __construct(private int $id) {}
来源：http://jz.huixiangedu.cn

[U51] PHP：数组解构
来源：http://wq.nszjky.cn

[$a, $b] = $arr;
来源：http://xd.521024.cn

[U52] PHP：箭头函数
来源：http://rx.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://im.nicolike.cn

[U53] PHP：空合并运算符
来源：http://bm.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://sa.asd995.cn

[U54] PHP：空安全调用
来源：http://yy.nicolike.cn

$obj?->method()
来源：http://tg.colortex.cn

[U55] PHP：match 表达式
来源：http://mg.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iv.hnjuh.cn

[U56] PHP：命名参数
来源：http://qu.lnxyls.cn

f(a: 1, b: 2)
来源：http://ux.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://mh.newstarts.cn

"值: {$a}"
来源：http://ev.newstarts.cn

[U58] PHP：数组三件套
来源：http://om.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mr.szsharing.cn

[U59] PHP：自定义排序
来源：http://bw.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vj.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://ax.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yy.9csxet.cn

[U61] PHP：正则
来源：http://pv.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vc.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://jt.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jx.haigaiapp.cn

[U63] PHP：文件读写
来源：http://hy.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qp.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://oi.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://xy.huanxung.cn

[U65] PHP：会话
来源：http://ww.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vp.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://wq.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nh.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://qz.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fo.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://lx.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rz.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://zf.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rr.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://sj.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cf.521024.cn

[U71] PHP：抛出异常
来源：http://zo.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://vv.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://kg.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://vq.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://lr.521024.cn

parse_ini_file("config.ini", true)
来源：http://ys.huanxung.cn

[U74] PHP：读取环境变量
来源：http://sv.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://jh.colortex.cn


<!-- 参考信息 -->