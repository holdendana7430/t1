代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zy.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://zh.colortex.cn

static_cast<double>(a) / b
来源：http://lj.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://nx.nszjky.cn

int size() const noexcept { return n_; }
来源：http://ns.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://sg.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://cj.szxytkj.cn

[S54] C++：异常处理
来源：http://zc.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kn.shxzukj.cn

[S55] C++：结构化绑定
来源：http://mj.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mj.shxzukj.cn

[S56] C++：optional
来源：http://ij.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kz.asd995.cn

[S57] C++：编译期常量
来源：http://lg.hahajie.cn

constexpr int N = 10;
来源：http://xa.wgjwhj.cn

[S58] C++：命名空间
来源：http://bg.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://ir.szxytkj.cn

[S59] C++：静态断言
来源：http://nj.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vs.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://vc.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jj.lnxyls.cn

================================================================================
来源：http://xc.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gn.huanxung.cn

================================================================================
来源：http://iw.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://hx.hahajie.cn

println("Hello")
来源：http://oa.szxytkj.cn

[T02] Kotlin：变量
来源：http://yf.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ar.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://ma.huanxung.cn

"值: $b"
来源：http://gy.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://bh.asd995.cn

val n: String? = null;  n?.length
来源：http://jc.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://bx.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gz.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://oc.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rl.colortex.cn

[T07] Kotlin：集合过滤
来源：http://yi.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jx.hnjuh.cn

[T08] Kotlin：数据类
来源：http://sz.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://kq.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://wo.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://tp.szsharing.cn

[T10] Kotlin：默认参数
来源：http://oa.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ak.newstarts.cn

[T11] Kotlin：协程
来源：http://ev.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yo.huanxung.cn

[T12] Kotlin：解构声明
来源：http://pz.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://uq.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://zg.nicolike.cn

val m = mapOf("a" to 1)
来源：http://zb.muxihuayi.cn

[T14] Kotlin：循环
来源：http://oh.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://ui.colortex.cn

[T15] Kotlin：接口
来源：http://ib.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://zk.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://wd.haigaiapp.cn

print("Hello")
来源：http://ju.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://gh.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://mb.nicolike.cn

[T18] Swift：字符串插值
来源：http://fz.hahajie.cn

"值: \(b)"
来源：http://ac.nicolike.cn

[T19] Swift：可选绑定
来源：http://ur.521024.cn

if let n = opt { print(n) }
来源：http://ta.shxzukj.cn

[T20] Swift：数组操作
来源：http://ov.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oc.szxytkj.cn

[T21] Swift：遍历
来源：http://uy.huixiangedu.cn

for x in a { print(x) }
来源：http://yh.9csxet.cn

[T22] Swift：字典
来源：http://rp.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sd.colortex.cn

[T23] Swift：函数
来源：http://ns.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tg.shxzskj.cn

[T24] Swift：闭包
来源：http://vh.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://an.hahajie.cn

[T25] Swift：结构体
来源：http://br.lnxyls.cn

struct P { var x: Int }
来源：http://cb.lnxyls.cn

[T26] Swift：类与重写
来源：http://rm.lnxyls.cn

class A: Base { override func f() {} }
来源：http://fk.colortex.cn

[T27] Swift：错误处理
来源：http://pz.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://ev.szxytkj.cn

[T28] Swift：枚举
来源：http://hc.shtwfgs.cn

enum Color { case red, green }
来源：http://av.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://cs.shxzskj.cn

guard let x = opt else { return }
来源：http://dw.huixinmuqiang.cn

[T30] Swift：协议
来源：http://fz.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://kb.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://mm.chemitech.net.cn

print("Hello")
来源：http://vu.szxytkj.cn

[T32] Lua：局部变量
来源：http://qq.lnxyls.cn

local a = 1
来源：http://th.hnjuh.cn

[T33] Lua：表（数组）
来源：http://um.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ul.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://yv.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wk.521024.cn

[T35] Lua：字典表
来源：http://hm.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://hb.huixinmuqiang.cn

[T36] Lua：函数
来源：http://ab.gzmigu.cn

function add(a, b) return a + b end
来源：http://zi.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://lw.shxzukj.cn

"a" .. "b"
来源：http://xo.521024.cn

[T38] Lua：条件
来源：http://rm.gzmigu.cn

if x > 0 then print("正") end
来源：http://zm.shxzukj.cn

[T39] Lua：模式匹配
来源：http://px.shxzukj.cn

string.find(s, "%d+")
来源：http://cj.newstarts.cn

[T40] Lua：元表
来源：http://or.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://zw.wgjwhj.cn

[T41] Perl：Hello World
来源：http://yk.lnxyls.cn

print "Hello\n";
来源：http://dw.shtwfgs.cn

[T42] Perl：变量类型
来源：http://oa.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jc.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://si.chemitech.net.cn

"值: $a"
来源：http://tc.yuntaijiaju.cn

[T44] Perl：条件
来源：http://aj.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://nr.nszjky.cn

[T45] Perl：数组遍历
来源：http://nr.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://cs.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://tt.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ax.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://hw.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bn.huanxung.cn

[T48] Perl：正则替换
来源：http://fs.nszjky.cn

$s =~ s/old/new/g;
来源：http://la.haigaiapp.cn

[T49] Perl：函数
来源：http://ti.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://el.hahajie.cn

[T50] Perl：逐行读文件
来源：http://dd.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yd.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://vh.521024.cn

[T51] Scala：Hello World
来源：http://st.szsharing.cn

println("Hello")
来源：http://dp.9csxet.cn

[T52] Scala：变量
来源：http://di.shtwfgs.cn

val a = 1;  var b = 2
来源：http://tr.shxzukj.cn

[T53] Scala：字符串插值
来源：http://cc.jianghongdianzi.cn

s"值: $b"
来源：http://eb.chemitech.net.cn

[T54] Scala：集合映射
来源：http://zz.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://ax.hahajie.cn

[T55] Scala：集合过滤
来源：http://vh.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ij.521024.cn

[T56] Scala：样例类
来源：http://vf.panjiajie.cn

case class User(name: String, age: Int)
来源：http://xh.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://vo.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ei.huixiangedu.cn

[T58] Scala：函数定义
来源：http://di.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sk.szsharing.cn

[T59] Scala：循环
来源：http://lx.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://qs.haigaiapp.cn

[T60] Scala：折叠
来源：http://es.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sy.jianghongdianzi.cn

================================================================================
来源：http://yx.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ks.nszjky.cn

================================================================================
来源：http://bo.colortex.cn

[U01] Py：创建虚拟环境
来源：http://tw.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fk.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://st.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iu.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://yu.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oc.521024.cn

[U04] Py：变量调试打印
来源：http://ap.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mn.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://eu.hnjuh.cn

list(dict.fromkeys(arr))
来源：http://ir.panjiajie.cn

[U06] Py：合并两个字典
来源：http://ie.yuexingan06.cn

{**a, **b}
来源：http://mt.shxzukj.cn

[U07] Py：反转字典键值
来源：http://in.hahajie.cn

{v: k for k, v in d.items()}
来源：http://sa.szsharing.cn

[U08] Py：展平二维列表
来源：http://rp.haigaiapp.cn

[y for x in nested for y in x]
来源：http://zy.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://gt.bookmarksfly.cn

max(d, key=d.get)
来源：http://nt.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://nx.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hl.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://ah.shtwfgs.cn

(x * 2 for x in arr)
来源：http://eu.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fp.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://ub.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://fg.shtwfgs.cn

deque(maxlen=10)
来源：http://qg.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://df.colortex.cn

defaultdict(list)
来源：http://jc.colortex.cn

[U15] Py：高精度计时
来源：http://sa.shxzskj.cn

t = time.perf_counter()
来源：http://ml.9csxet.cn

[U16] Py：命令行参数解析
来源：http://gb.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sv.9csxet.cn

[U17] Py：初始化日志
来源：http://fn.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://lv.shxzskj.cn

[U18] Py：预编译正则
来源：http://yc.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://au.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://cc.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xv.hahajie.cn

[U20] Py：缓存函数结果
来源：http://oy.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://au.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://yh.muxihuayi.cn

@contextlib.contextmanager
来源：http://fb.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://rf.shtwfgs.cn

list(zip(*m))
来源：http://fl.nicolike.cn

[U23] Py：分块读取大文件
来源：http://hf.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rb.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://un.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://do.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://dx.newstarts.cn

csv.DictReader(f)
来源：http://vb.nszjky.cn

[U26] Py：并发下载
来源：http://il.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rf.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://tu.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://yr.chemitech.net.cn

[U28] Py：类型别名
来源：http://bp.lnxyls.cn

UserId = int
来源：http://rm.hahajie.cn

[U29] Py：属性校验
来源：http://rp.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://sc.yuntaijiaju.cn

[U30] Py：数据类
来源：http://uj.9csxet.cn

@dataclass(slots=True)
来源：http://kj.panjiajie.cn

[U31] Py：单测
来源：http://ui.chemitech.net.cn

python -m pytest -q
来源：http://sb.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://iz.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://yy.gzmigu.cn

[U33] Py：打包发布
来源：http://ky.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://na.9csxet.cn

[U34] Py：判断编码
来源：http://dm.szsharing.cn

chardet.detect(raw)
来源：http://xa.lnxyls.cn

[U35] Py：发送邮件
来源：http://un.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wx.asd995.cn

[U36] Py：定时任务
来源：http://pc.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://ux.lnxyls.cn

[U37] Py：读写 Excel
来源：http://na.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ma.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://pd.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://bc.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://in.newstarts.cn

sys.stdout.isatty()
来源：http://ia.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://yb.asd995.cn

print("err", file=sys.stderr)
来源：http://wq.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://xf.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wd.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://qq.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hj.nicolike.cn

[U43] PHP：声明命名空间
来源：http://av.jctech888.com.cn

namespace App\Http;
来源：http://gf.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://va.huixinmuqiang.cn

declare(strict_types=1);
来源：http://ym.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://cz.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fq.asd995.cn

[U46] PHP：可空类型
来源：http://fr.shtwfgs.cn

?string $name = null
来源：http://fo.muxihuayi.cn

[U47] PHP：联合类型
来源：http://bz.shtwfgs.cn

int|string $id
来源：http://gs.9csxet.cn

[U48] PHP：纯枚举
来源：http://uu.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uf.chemitech.net.cn

[U49] PHP：只读属性
来源：http://gf.panjiajie.cn

public readonly string $name
来源：http://iy.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://ly.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://sg.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://zd.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://ed.szsharing.cn

[U52] PHP：箭头函数
来源：http://xr.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://qy.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://pz.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://xh.shxzukj.cn

[U54] PHP：空安全调用
来源：http://ba.yuntaijiaju.cn

$obj?->method()
来源：http://oi.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://kt.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sa.szxytkj.cn

[U56] PHP：命名参数
来源：http://mc.521024.cn

f(a: 1, b: 2)
来源：http://ik.gzmigu.cn

[U57] PHP：字符串插值
来源：http://dc.lnxyls.cn

"值: {$a}"
来源：http://ah.gzmigu.cn

[U58] PHP：数组三件套
来源：http://wk.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gp.shxzskj.cn

[U59] PHP：自定义排序
来源：http://ve.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ho.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://bb.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ew.chemitech.net.cn

[U61] PHP：正则
来源：http://xp.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ij.lnxyls.cn

[U62] PHP：日期对象
来源：http://et.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pc.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://pi.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rj.521024.cn

[U64] PHP：目录遍历
来源：http://cp.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://ua.jctech888.com.cn

[U65] PHP：会话
来源：http://jz.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gc.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://rv.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uh.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://vw.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zy.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://jh.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wq.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://kl.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://op.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://cj.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oq.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://eh.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://ts.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://wt.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://ia.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://ds.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://ec.newstarts.cn

[U74] PHP：读取环境变量
来源：http://mm.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://ps.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://gr.huixiangedu.cn

composer require psr/container
来源：http://rw.shxzukj.cn

[U76] PHP：简单路由
来源：http://ci.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://as.yuntaijiaju.cn


<!-- 参考信息 -->