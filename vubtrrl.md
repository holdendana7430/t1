代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://re.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vk.shxzskj.cn

[S48] C++：逐行读文件
来源：http://kv.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ad.asd995.cn

while (std::getline(in, line)) { }
来源：http://kh.yuntaijiaju.cn

[S49] C++：写文件
来源：http://lj.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ry.lnxyls.cn

[S50] C++：格式化数字
来源：http://bh.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wp.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://tm.colortex.cn

static_cast<double>(a) / b
来源：http://le.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://ic.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://ya.nszjky.cn

[S53] C++：移动语义
来源：http://ec.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://di.asd995.cn

[S54] C++：异常处理
来源：http://rf.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://it.szxytkj.cn

[S55] C++：结构化绑定
来源：http://rp.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gu.shxzskj.cn

[S56] C++：optional
来源：http://km.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dp.muxihuayi.cn

[S57] C++：编译期常量
来源：http://pw.yuntaijiaju.cn

constexpr int N = 10;
来源：http://as.wgjwhj.cn

[S58] C++：命名空间
来源：http://pp.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://cd.huanxung.cn

[S59] C++：静态断言
来源：http://rn.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bh.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://vz.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ki.lnxyls.cn

================================================================================
来源：http://pm.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zf.521024.cn

================================================================================
来源：http://kv.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://ar.jianghongdianzi.cn

println("Hello")
来源：http://oc.jctech888.com.cn

[T02] Kotlin：变量
来源：http://rq.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ar.colortex.cn

[T03] Kotlin：字符串模板
来源：http://pz.yuntaijiaju.cn

"值: $b"
来源：http://de.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://sw.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://wg.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://qe.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yj.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://lb.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ik.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://ir.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ny.shxzukj.cn

[T08] Kotlin：数据类
来源：http://gj.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://xi.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://wd.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://el.nszjky.cn

[T10] Kotlin：默认参数
来源：http://dj.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://as.yuexingan06.cn

[T11] Kotlin：协程
来源：http://hw.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kx.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://pp.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://qg.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://ts.9csxet.cn

val m = mapOf("a" to 1)
来源：http://zp.gzmigu.cn

[T14] Kotlin：循环
来源：http://lf.521024.cn

for (i in 1..10) println(i)
来源：http://kn.gzmigu.cn

[T15] Kotlin：接口
来源：http://xs.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://xl.shxzskj.cn

[T16] Swift：Hello World
来源：http://uj.shxzskj.cn

print("Hello")
来源：http://ge.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://bi.panjiajie.cn

var a = 1;  let b = 2
来源：http://mm.colortex.cn

[T18] Swift：字符串插值
来源：http://cp.huanxung.cn

"值: \(b)"
来源：http://ip.521024.cn

[T19] Swift：可选绑定
来源：http://sp.shxzukj.cn

if let n = opt { print(n) }
来源：http://gl.hahajie.cn

[T20] Swift：数组操作
来源：http://xo.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://li.szxytkj.cn

[T21] Swift：遍历
来源：http://jj.huixiangedu.cn

for x in a { print(x) }
来源：http://oe.szxytkj.cn

[T22] Swift：字典
来源：http://di.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://an.nicolike.cn

[T23] Swift：函数
来源：http://dh.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lq.haigaiapp.cn

[T24] Swift：闭包
来源：http://ft.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ov.bookmarksfly.cn

[T25] Swift：结构体
来源：http://tu.nicolike.cn

struct P { var x: Int }
来源：http://cj.hahajie.cn

[T26] Swift：类与重写
来源：http://mv.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://rb.hnjuh.cn

[T27] Swift：错误处理
来源：http://zi.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://wf.colortex.cn

[T28] Swift：枚举
来源：http://dq.huixinmuqiang.cn

enum Color { case red, green }
来源：http://jz.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://gx.shxzukj.cn

guard let x = opt else { return }
来源：http://is.jctech888.com.cn

[T30] Swift：协议
来源：http://du.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://sz.chemitech.net.cn

[T31] Lua：Hello World
来源：http://fb.nicolike.cn

print("Hello")
来源：http://ue.nszjky.cn

[T32] Lua：局部变量
来源：http://xf.huixiangedu.cn

local a = 1
来源：http://ao.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://uo.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sf.szxytkj.cn

[T34] Lua：遍历表
来源：http://ow.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ww.muxihuayi.cn

[T35] Lua：字典表
来源：http://uz.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://sc.jianghongdianzi.cn

[T36] Lua：函数
来源：http://qc.newstarts.cn

function add(a, b) return a + b end
来源：http://be.colortex.cn

[T37] Lua：字符串拼接
来源：http://rx.huanxung.cn

"a" .. "b"
来源：http://kh.muxihuayi.cn

[T38] Lua：条件
来源：http://bv.jctech888.com.cn

if x > 0 then print("正") end
来源：http://eb.nszjky.cn

[T39] Lua：模式匹配
来源：http://bz.newstarts.cn

string.find(s, "%d+")
来源：http://pm.nszjky.cn

[T40] Lua：元表
来源：http://mo.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://xs.chemitech.net.cn

[T41] Perl：Hello World
来源：http://sb.asd995.cn

print "Hello\n";
来源：http://bd.521024.cn

[T42] Perl：变量类型
来源：http://bj.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yt.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://rc.haigaiapp.cn

"值: $a"
来源：http://jo.bookmarksfly.cn

[T44] Perl：条件
来源：http://dt.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://ku.nszjky.cn

[T45] Perl：数组遍历
来源：http://wd.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://vo.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://sr.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fq.521024.cn

[T47] Perl：正则捕获
来源：http://xl.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ki.huanxung.cn

[T48] Perl：正则替换
来源：http://je.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://ui.wgjwhj.cn

[T49] Perl：函数
来源：http://or.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nr.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://oa.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://by.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://lw.hnjuh.cn

[T51] Scala：Hello World
来源：http://xg.bjjhwx.cn

println("Hello")
来源：http://zi.lnxyls.cn

[T52] Scala：变量
来源：http://kp.muxihuayi.cn

val a = 1;  var b = 2
来源：http://cy.hahajie.cn

[T53] Scala：字符串插值
来源：http://br.chemitech.net.cn

s"值: $b"
来源：http://te.szxytkj.cn

[T54] Scala：集合映射
来源：http://tl.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://vf.newstarts.cn

[T55] Scala：集合过滤
来源：http://jg.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fd.nicolike.cn

[T56] Scala：样例类
来源：http://fk.nszjky.cn

case class User(name: String, age: Int)
来源：http://wj.hahajie.cn

[T57] Scala：模式匹配
来源：http://uz.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dy.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://qa.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oj.huanxung.cn

[T59] Scala：循环
来源：http://yj.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://ue.szsharing.cn

[T60] Scala：折叠
来源：http://qz.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ze.bjjhwx.cn

================================================================================
来源：http://ag.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nv.jianghongdianzi.cn

================================================================================
来源：http://wr.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://kb.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jl.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://ug.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oo.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://hy.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sd.panjiajie.cn

[U04] Py：变量调试打印
来源：http://ar.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jz.9csxet.cn

[U05] Py：列表去重且保序
来源：http://bd.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://hr.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://lo.huixinmuqiang.cn

{**a, **b}
来源：http://nb.asd995.cn

[U07] Py：反转字典键值
来源：http://vj.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://er.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://me.bjjhwx.cn

[y for x in nested for y in x]
来源：http://uc.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://ny.shxzskj.cn

max(d, key=d.get)
来源：http://nl.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://jq.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gg.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://un.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://ux.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ai.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://ov.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://pz.bjjhwx.cn

deque(maxlen=10)
来源：http://pr.asd995.cn

[U14] Py：分组收集到列表
来源：http://qo.szsharing.cn

defaultdict(list)
来源：http://fs.asd995.cn

[U15] Py：高精度计时
来源：http://sp.yuntaijiaju.cn

t = time.perf_counter()
来源：http://vr.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://oq.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tn.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://np.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://jd.shxzskj.cn

[U18] Py：预编译正则
来源：http://ji.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://hw.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://wm.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qm.hahajie.cn

[U20] Py：缓存函数结果
来源：http://eb.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://qk.521024.cn

[U21] Py：自定义上下文管理器
来源：http://ty.huanxung.cn

@contextlib.contextmanager
来源：http://tr.shxzskj.cn

[U22] Py：矩阵转置
来源：http://in.asd995.cn

list(zip(*m))
来源：http://pg.nszjky.cn

[U23] Py：分块读取大文件
来源：http://cd.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ub.nicolike.cn

[U24] Py：路径操作
来源：http://ch.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rr.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://mj.asd995.cn

csv.DictReader(f)
来源：http://kz.hnjuh.cn

[U26] Py：并发下载
来源：http://co.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cs.nicolike.cn

[U27] Py：异步 HTTP
来源：http://rn.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://yb.asd995.cn

[U28] Py：类型别名
来源：http://bc.9csxet.cn

UserId = int
来源：http://ki.muxihuayi.cn

[U29] Py：属性校验
来源：http://rk.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://am.chemitech.net.cn

[U30] Py：数据类
来源：http://no.shxzskj.cn

@dataclass(slots=True)
来源：http://qc.huixiangedu.cn

[U31] Py：单测
来源：http://iv.yuexingan06.cn

python -m pytest -q
来源：http://rk.huanxung.cn

[U32] Py：代码格式化
来源：http://vk.szsharing.cn

ruff format . && ruff check --fix .
来源：http://jn.hahajie.cn

[U33] Py：打包发布
来源：http://op.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://eo.jctech888.com.cn

[U34] Py：判断编码
来源：http://xu.gzmigu.cn

chardet.detect(raw)
来源：http://rr.521024.cn

[U35] Py：发送邮件
来源：http://yo.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://or.haigaiapp.cn

[U36] Py：定时任务
来源：http://qv.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://go.szsharing.cn

[U37] Py：读写 Excel
来源：http://tt.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ea.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://nm.shxzukj.cn

Path(__file__).resolve().parent
来源：http://pm.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://sn.huixiangedu.cn

sys.stdout.isatty()
来源：http://nu.szsharing.cn

[U40] Py：打印到标准错误
来源：http://yk.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://rn.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://vz.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ha.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://gw.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jv.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://av.521024.cn

namespace App\Http;
来源：http://zm.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://mk.lnxyls.cn

declare(strict_types=1);
来源：http://qq.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://ga.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rr.colortex.cn

[U46] PHP：可空类型
来源：http://wg.huanxung.cn

?string $name = null
来源：http://qr.521024.cn

[U47] PHP：联合类型
来源：http://ks.9csxet.cn

int|string $id
来源：http://uq.newstarts.cn

[U48] PHP：纯枚举
来源：http://bd.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://in.yuexingan06.cn

[U49] PHP：只读属性
来源：http://zf.shxzskj.cn

public readonly string $name
来源：http://ym.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://tt.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://qi.shxzskj.cn

[U51] PHP：数组解构
来源：http://cc.lnxyls.cn

[$a, $b] = $arr;
来源：http://cw.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://uk.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://se.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://tg.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://oa.9csxet.cn

[U54] PHP：空安全调用
来源：http://vc.huanxung.cn

$obj?->method()
来源：http://mu.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://eu.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yh.huixiangedu.cn

[U56] PHP：命名参数
来源：http://wk.panjiajie.cn

f(a: 1, b: 2)
来源：http://ox.asd995.cn

[U57] PHP：字符串插值
来源：http://cu.shtwfgs.cn

"值: {$a}"
来源：http://op.521024.cn

[U58] PHP：数组三件套
来源：http://yi.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ne.nszjky.cn

[U59] PHP：自定义排序
来源：http://aj.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vr.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://ph.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wf.nicolike.cn

[U61] PHP：正则
来源：http://kl.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bt.shxzskj.cn

[U62] PHP：日期对象
来源：http://df.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vf.bjjhwx.cn

[U63] PHP：文件读写
来源：http://um.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bc.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://sy.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://eb.shxzukj.cn

[U65] PHP：会话
来源：http://mw.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nn.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://ec.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://or.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://fl.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ie.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://mq.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qb.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://bq.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uy.huanxung.cn

[U70] PHP：PDO 事务
来源：http://lm.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bc.hahajie.cn

[U71] PHP：抛出异常
来源：http://wi.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://df.lnxyls.cn

[U72] PHP：写错误日志
来源：http://nk.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://nq.asd995.cn


<!-- 参考信息 -->