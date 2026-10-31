代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://iv.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dd.hnjuh.cn

[S48] C++：逐行读文件
来源：http://rg.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wz.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://ao.shxzskj.cn

[S49] C++：写文件
来源：http://je.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wz.newstarts.cn

[S50] C++：格式化数字
来源：http://tp.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ez.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://xe.chemitech.net.cn

static_cast<double>(a) / b
来源：http://zy.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://gh.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://gm.shtwfgs.cn

[S53] C++：移动语义
来源：http://ci.colortex.cn

std::vector<int> w = std::move(v);
来源：http://mo.bjjhwx.cn

[S54] C++：异常处理
来源：http://xi.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pk.shxzskj.cn

[S55] C++：结构化绑定
来源：http://ke.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dj.muxihuayi.cn

[S56] C++：optional
来源：http://jq.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bt.huanxung.cn

[S57] C++：编译期常量
来源：http://uw.panjiajie.cn

constexpr int N = 10;
来源：http://ti.huixiangedu.cn

[S58] C++：命名空间
来源：http://jn.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://rl.shtwfgs.cn

[S59] C++：静态断言
来源：http://zs.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kk.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://qv.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://az.huanxung.cn

================================================================================
来源：http://vh.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hp.huixinmuqiang.cn

================================================================================
来源：http://iv.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://xc.szsharing.cn

println("Hello")
来源：http://jt.hahajie.cn

[T02] Kotlin：变量
来源：http://ub.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mj.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://zv.szxytkj.cn

"值: $b"
来源：http://wm.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://zw.newstarts.cn

val n: String? = null;  n?.length
来源：http://yb.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://lv.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://or.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://rf.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sj.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://hs.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yr.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://ko.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://bo.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://kd.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://lv.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://fk.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ap.nicolike.cn

[T11] Kotlin：协程
来源：http://qn.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cb.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://vm.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://wc.asd995.cn

[T13] Kotlin：只读 Map
来源：http://mg.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://iv.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://yy.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://cu.bjjhwx.cn

[T15] Kotlin：接口
来源：http://nk.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://kx.wgjwhj.cn

[T16] Swift：Hello World
来源：http://pq.nicolike.cn

print("Hello")
来源：http://lw.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://th.asd995.cn

var a = 1;  let b = 2
来源：http://jw.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://dm.szsharing.cn

"值: \(b)"
来源：http://ed.nicolike.cn

[T19] Swift：可选绑定
来源：http://fy.colortex.cn

if let n = opt { print(n) }
来源：http://id.chemitech.net.cn

[T20] Swift：数组操作
来源：http://fq.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oq.wgjwhj.cn

[T21] Swift：遍历
来源：http://vr.yuexingan06.cn

for x in a { print(x) }
来源：http://eq.hnjuh.cn

[T22] Swift：字典
来源：http://mq.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xl.chemitech.net.cn

[T23] Swift：函数
来源：http://uu.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zx.521024.cn

[T24] Swift：闭包
来源：http://ch.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ly.panjiajie.cn

[T25] Swift：结构体
来源：http://fk.jianghongdianzi.cn

struct P { var x: Int }
来源：http://ip.haigaiapp.cn

[T26] Swift：类与重写
来源：http://ku.gzmigu.cn

class A: Base { override func f() {} }
来源：http://cy.newstarts.cn

[T27] Swift：错误处理
来源：http://mi.szsharing.cn

do { try f() } catch { print(error) }
来源：http://mx.nszjky.cn

[T28] Swift：枚举
来源：http://qk.bookmarksfly.cn

enum Color { case red, green }
来源：http://zd.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://gq.hahajie.cn

guard let x = opt else { return }
来源：http://on.gzmigu.cn

[T30] Swift：协议
来源：http://ki.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://ff.yuexingan06.cn

[T31] Lua：Hello World
来源：http://do.lnxyls.cn

print("Hello")
来源：http://qb.shxzskj.cn

[T32] Lua：局部变量
来源：http://jv.colortex.cn

local a = 1
来源：http://zy.colortex.cn

[T33] Lua：表（数组）
来源：http://se.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hs.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://tj.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dp.jctech888.com.cn

[T35] Lua：字典表
来源：http://zg.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://ik.chemitech.net.cn

[T36] Lua：函数
来源：http://xk.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://yu.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://lw.521024.cn

"a" .. "b"
来源：http://wp.szxytkj.cn

[T38] Lua：条件
来源：http://yz.szsharing.cn

if x > 0 then print("正") end
来源：http://mf.huanxung.cn

[T39] Lua：模式匹配
来源：http://rj.bookmarksfly.cn

string.find(s, "%d+")
来源：http://lm.hnjuh.cn

[T40] Lua：元表
来源：http://mn.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://ee.shtwfgs.cn

[T41] Perl：Hello World
来源：http://qx.lnxyls.cn

print "Hello\n";
来源：http://qz.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://rq.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wg.521024.cn

[T43] Perl：字符串插值
来源：http://pt.lnxyls.cn

"值: $a"
来源：http://sh.jianghongdianzi.cn

[T44] Perl：条件
来源：http://wc.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://bt.lnxyls.cn

[T45] Perl：数组遍历
来源：http://it.colortex.cn

for my $x (@arr) { print $x; }
来源：http://xs.szsharing.cn

[T46] Perl：哈希操作
来源：http://qq.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pl.nicolike.cn

[T47] Perl：正则捕获
来源：http://na.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vn.szsharing.cn

[T48] Perl：正则替换
来源：http://yg.521024.cn

$s =~ s/old/new/g;
来源：http://hs.muxihuayi.cn

[T49] Perl：函数
来源：http://ny.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yk.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://dr.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ao.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://lx.shxzukj.cn

[T51] Scala：Hello World
来源：http://hg.jctech888.com.cn

println("Hello")
来源：http://uz.shxzskj.cn

[T52] Scala：变量
来源：http://os.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://ja.szxytkj.cn

[T53] Scala：字符串插值
来源：http://th.jctech888.com.cn

s"值: $b"
来源：http://co.newstarts.cn

[T54] Scala：集合映射
来源：http://hy.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://be.panjiajie.cn

[T55] Scala：集合过滤
来源：http://gf.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vv.bookmarksfly.cn

[T56] Scala：样例类
来源：http://jx.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://ev.shxzskj.cn

[T57] Scala：模式匹配
来源：http://oy.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cw.bjjhwx.cn

[T58] Scala：函数定义
来源：http://en.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://su.bjjhwx.cn

[T59] Scala：循环
来源：http://ys.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://ng.szxytkj.cn

[T60] Scala：折叠
来源：http://hi.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://to.lnxyls.cn

================================================================================
来源：http://xm.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://id.hnjuh.cn

================================================================================
来源：http://jb.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://vl.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lk.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://mo.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hw.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://lg.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gb.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://la.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wy.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://za.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://uk.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://ad.szxytkj.cn

{**a, **b}
来源：http://cl.lnxyls.cn

[U07] Py：反转字典键值
来源：http://jg.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://gh.huanxung.cn

[U08] Py：展平二维列表
来源：http://sp.szxytkj.cn

[y for x in nested for y in x]
来源：http://qx.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://kg.nszjky.cn

max(d, key=d.get)
来源：http://la.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://xl.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ge.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://ee.newstarts.cn

(x * 2 for x in arr)
来源：http://gs.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qo.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://kr.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://sf.asd995.cn

deque(maxlen=10)
来源：http://dp.huanxung.cn

[U14] Py：分组收集到列表
来源：http://ip.yuexingan06.cn

defaultdict(list)
来源：http://rm.shxzukj.cn

[U15] Py：高精度计时
来源：http://jh.haigaiapp.cn

t = time.perf_counter()
来源：http://gm.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://kn.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hu.521024.cn

[U17] Py：初始化日志
来源：http://ta.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://im.jctech888.com.cn

[U18] Py：预编译正则
来源：http://gi.newstarts.cn

pat = re.compile(r"\d+")
来源：http://gs.nicolike.cn

[U19] Py：正则替换带回调
来源：http://lb.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fs.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://bl.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://lf.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://fe.szxytkj.cn

@contextlib.contextmanager
来源：http://nw.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://di.gzmigu.cn

list(zip(*m))
来源：http://yv.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://jp.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xm.szsharing.cn

[U24] Py：路径操作
来源：http://oz.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cq.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://kr.muxihuayi.cn

csv.DictReader(f)
来源：http://gp.nszjky.cn

[U26] Py：并发下载
来源：http://nw.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xn.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://eb.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://ee.yuexingan06.cn

[U28] Py：类型别名
来源：http://pi.newstarts.cn

UserId = int
来源：http://ga.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://pi.gzmigu.cn

@property 与 @x.setter 配合
来源：http://vx.wgjwhj.cn

[U30] Py：数据类
来源：http://mv.colortex.cn

@dataclass(slots=True)
来源：http://nw.yuntaijiaju.cn

[U31] Py：单测
来源：http://xr.jctech888.com.cn

python -m pytest -q
来源：http://uw.521024.cn

[U32] Py：代码格式化
来源：http://wo.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://xn.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://fm.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://ev.chemitech.net.cn

[U34] Py：判断编码
来源：http://ky.jctech888.com.cn

chardet.detect(raw)
来源：http://uq.newstarts.cn

[U35] Py：发送邮件
来源：http://gz.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://so.asd995.cn

[U36] Py：定时任务
来源：http://vm.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://ge.asd995.cn

[U37] Py：读写 Excel
来源：http://ac.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dx.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://ie.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://md.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://oo.shtwfgs.cn

sys.stdout.isatty()
来源：http://aj.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://ed.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://vi.bjjhwx.cn

[U41] PHP：初始化 Composer 项目
来源：http://gd.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cm.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://co.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ys.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://yi.colortex.cn

namespace App\Http;
来源：http://aa.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://aw.huixiangedu.cn

declare(strict_types=1);
来源：http://qf.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://bx.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tx.wgjwhj.cn

[U46] PHP：可空类型
来源：http://gq.muxihuayi.cn

?string $name = null
来源：http://hh.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://mj.nicolike.cn

int|string $id
来源：http://ca.9csxet.cn

[U48] PHP：纯枚举
来源：http://ma.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lf.huixiangedu.cn

[U49] PHP：只读属性
来源：http://ep.panjiajie.cn

public readonly string $name
来源：http://cv.asd995.cn

[U50] PHP：构造器属性提升
来源：http://lp.szxytkj.cn

public function __construct(private int $id) {}
来源：http://td.asd995.cn

[U51] PHP：数组解构
来源：http://cb.huixiangedu.cn

[$a, $b] = $arr;
来源：http://la.shxzskj.cn

[U52] PHP：箭头函数
来源：http://tn.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://ss.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://vl.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://fn.shxzskj.cn

[U54] PHP：空安全调用
来源：http://sa.lnxyls.cn

$obj?->method()
来源：http://ur.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://ys.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qa.shxzukj.cn

[U56] PHP：命名参数
来源：http://df.huixiangedu.cn

f(a: 1, b: 2)
来源：http://ex.nicolike.cn

[U57] PHP：字符串插值
来源：http://wf.panjiajie.cn

"值: {$a}"
来源：http://iw.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://hp.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lv.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://kb.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://if.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://eb.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://of.yuexingan06.cn

[U61] PHP：正则
来源：http://zw.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qy.bjjhwx.cn

[U62] PHP：日期对象
来源：http://av.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yf.shtwfgs.cn

[U63] PHP：文件读写
来源：http://ei.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ew.hahajie.cn

[U64] PHP：目录遍历
来源：http://hg.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://ue.newstarts.cn

[U65] PHP：会话
来源：http://wm.gzmigu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ga.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://kb.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ew.hahajie.cn

[U67] PHP：处理文件上传
来源：http://om.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ne.szsharing.cn

[U68] PHP：PDO 连接
来源：http://lo.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bv.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://hv.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://io.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://um.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cc.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://bi.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://zu.521024.cn

[U72] PHP：写错误日志
来源：http://xj.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://yh.hahajie.cn


<!-- 参考信息 -->