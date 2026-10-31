代发 wailian999

while (std::getline(in, line)) { }
来源：http://ki.panjiajie.cn

[S49] C++：写文件
来源：http://yp.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fi.hnjuh.cn

[S50] C++：格式化数字
来源：http://jo.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sc.gzmigu.cn

[S51] C++：显式类型转换
来源：http://bj.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://bq.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://jl.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://uh.newstarts.cn

[S53] C++：移动语义
来源：http://jh.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://or.jctech888.com.cn

[S54] C++：异常处理
来源：http://nn.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qc.gzmigu.cn

[S55] C++：结构化绑定
来源：http://xa.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://du.shxzukj.cn

[S56] C++：optional
来源：http://oa.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xy.shtwfgs.cn

[S57] C++：编译期常量
来源：http://vj.haigaiapp.cn

constexpr int N = 10;
来源：http://rc.yuexingan06.cn

[S58] C++：命名空间
来源：http://xb.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://wm.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://df.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://li.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://er.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ov.jctech888.com.cn

================================================================================
来源：http://hd.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://za.shxzskj.cn

================================================================================
来源：http://fo.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://ul.nicolike.cn

println("Hello")
来源：http://jd.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://dx.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wg.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://bh.chemitech.net.cn

"值: $b"
来源：http://le.colortex.cn

[T04] Kotlin：空安全
来源：http://jr.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://ut.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://wc.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vg.asd995.cn

[T06] Kotlin：集合映射
来源：http://gs.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mc.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://nt.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pm.panjiajie.cn

[T08] Kotlin：数据类
来源：http://qs.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://na.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://gm.colortex.cn

fun String.exclaim() = this + "!"
来源：http://nk.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://vq.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://eq.nszjky.cn

[T11] Kotlin：协程
来源：http://tu.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zx.nicolike.cn

[T12] Kotlin：解构声明
来源：http://av.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://pe.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://cd.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://lu.colortex.cn

[T14] Kotlin：循环
来源：http://fl.nszjky.cn

for (i in 1..10) println(i)
来源：http://wq.panjiajie.cn

[T15] Kotlin：接口
来源：http://ot.colortex.cn

interface Shape { fun area(): Double }
来源：http://tf.szsharing.cn

[T16] Swift：Hello World
来源：http://ol.gzmigu.cn

print("Hello")
来源：http://ra.huanxung.cn

[T17] Swift：变量与常量
来源：http://ax.nicolike.cn

var a = 1;  let b = 2
来源：http://jd.asd995.cn

[T18] Swift：字符串插值
来源：http://ek.bookmarksfly.cn

"值: \(b)"
来源：http://vb.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://ce.gzmigu.cn

if let n = opt { print(n) }
来源：http://qg.shxzskj.cn

[T20] Swift：数组操作
来源：http://ly.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fa.yuexingan06.cn

[T21] Swift：遍历
来源：http://mv.shxzskj.cn

for x in a { print(x) }
来源：http://hh.szxytkj.cn

[T22] Swift：字典
来源：http://rw.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ty.szsharing.cn

[T23] Swift：函数
来源：http://zc.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pp.gzmigu.cn

[T24] Swift：闭包
来源：http://hz.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vd.jctech888.com.cn

[T25] Swift：结构体
来源：http://gj.panjiajie.cn

struct P { var x: Int }
来源：http://xe.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://ay.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://qt.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://gy.9csxet.cn

do { try f() } catch { print(error) }
来源：http://zl.hnjuh.cn

[T28] Swift：枚举
来源：http://io.shxzukj.cn

enum Color { case red, green }
来源：http://de.asd995.cn

[T29] Swift：guard 提前返回
来源：http://sb.9csxet.cn

guard let x = opt else { return }
来源：http://if.yuexingan06.cn

[T30] Swift：协议
来源：http://su.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://bz.wgjwhj.cn

[T31] Lua：Hello World
来源：http://ta.huanxung.cn

print("Hello")
来源：http://sn.newstarts.cn

[T32] Lua：局部变量
来源：http://ih.colortex.cn

local a = 1
来源：http://xc.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://jd.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bm.huanxung.cn

[T34] Lua：遍历表
来源：http://fk.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ac.szxytkj.cn

[T35] Lua：字典表
来源：http://mx.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://us.nszjky.cn

[T36] Lua：函数
来源：http://qu.9csxet.cn

function add(a, b) return a + b end
来源：http://bo.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://wz.huanxung.cn

"a" .. "b"
来源：http://jf.wgjwhj.cn

[T38] Lua：条件
来源：http://wj.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://ug.newstarts.cn

[T39] Lua：模式匹配
来源：http://zu.huixiangedu.cn

string.find(s, "%d+")
来源：http://ep.yuexingan06.cn

[T40] Lua：元表
来源：http://gp.huanxung.cn

setmetatable({}, { __index = base })
来源：http://vg.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://ps.panjiajie.cn

print "Hello\n";
来源：http://an.szxytkj.cn

[T42] Perl：变量类型
来源：http://nh.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xi.panjiajie.cn

[T43] Perl：字符串插值
来源：http://sk.nicolike.cn

"值: $a"
来源：http://wx.haigaiapp.cn

[T44] Perl：条件
来源：http://ov.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://uu.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://ls.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://nc.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://zl.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bi.szsharing.cn

[T47] Perl：正则捕获
来源：http://wo.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://eh.huixiangedu.cn

[T48] Perl：正则替换
来源：http://ld.hahajie.cn

$s =~ s/old/new/g;
来源：http://xj.521024.cn

[T49] Perl：函数
来源：http://hg.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vf.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://rn.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wf.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://cl.szxytkj.cn

[T51] Scala：Hello World
来源：http://qx.jianghongdianzi.cn

println("Hello")
来源：http://kf.jianghongdianzi.cn

[T52] Scala：变量
来源：http://fd.521024.cn

val a = 1;  var b = 2
来源：http://tr.nszjky.cn

[T53] Scala：字符串插值
来源：http://aq.jctech888.com.cn

s"值: $b"
来源：http://zc.hahajie.cn

[T54] Scala：集合映射
来源：http://dq.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ho.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://tt.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ey.huanxung.cn

[T56] Scala：样例类
来源：http://ha.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://kg.panjiajie.cn

[T57] Scala：模式匹配
来源：http://av.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qz.nicolike.cn

[T58] Scala：函数定义
来源：http://zx.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bu.wgjwhj.cn

[T59] Scala：循环
来源：http://hu.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://hb.jctech888.com.cn

[T60] Scala：折叠
来源：http://qq.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lv.nszjky.cn

================================================================================
来源：http://se.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sb.wgjwhj.cn

================================================================================
来源：http://ke.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://so.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ik.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://gt.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cz.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://rd.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bk.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://ub.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xr.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://kp.521024.cn

list(dict.fromkeys(arr))
来源：http://aw.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://sj.nicolike.cn

{**a, **b}
来源：http://hd.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://km.hahajie.cn

{v: k for k, v in d.items()}
来源：http://gs.nicolike.cn

[U08] Py：展平二维列表
来源：http://nk.chemitech.net.cn

[y for x in nested for y in x]
来源：http://nw.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://ei.chemitech.net.cn

max(d, key=d.get)
来源：http://ia.shxzukj.cn

[U10] Py：按值排序字典
来源：http://mi.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sw.shxzskj.cn

[U11] Py：生成器表达式
来源：http://sr.colortex.cn

(x * 2 for x in arr)
来源：http://py.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ci.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://wh.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://lp.szxytkj.cn

deque(maxlen=10)
来源：http://zj.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://pm.nicolike.cn

defaultdict(list)
来源：http://ia.chemitech.net.cn

[U15] Py：高精度计时
来源：http://gy.nszjky.cn

t = time.perf_counter()
来源：http://kf.521024.cn

[U16] Py：命令行参数解析
来源：http://xi.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jl.muxihuayi.cn

[U17] Py：初始化日志
来源：http://jj.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://dz.panjiajie.cn

[U18] Py：预编译正则
来源：http://jj.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://jv.asd995.cn

[U19] Py：正则替换带回调
来源：http://yf.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zj.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://mp.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://fy.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://wu.hahajie.cn

@contextlib.contextmanager
来源：http://sj.nszjky.cn

[U22] Py：矩阵转置
来源：http://sh.nicolike.cn

list(zip(*m))
来源：http://ml.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://qr.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bw.szsharing.cn

[U24] Py：路径操作
来源：http://ke.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://us.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://uu.huixiangedu.cn

csv.DictReader(f)
来源：http://ew.colortex.cn

[U26] Py：并发下载
来源：http://oz.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qx.newstarts.cn

[U27] Py：异步 HTTP
来源：http://kb.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://uz.chemitech.net.cn

[U28] Py：类型别名
来源：http://qp.bookmarksfly.cn

UserId = int
来源：http://oa.wgjwhj.cn

[U29] Py：属性校验
来源：http://ed.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://ze.bookmarksfly.cn

[U30] Py：数据类
来源：http://tk.hahajie.cn

@dataclass(slots=True)
来源：http://af.jianghongdianzi.cn

[U31] Py：单测
来源：http://wt.bjjhwx.cn

python -m pytest -q
来源：http://zw.gzmigu.cn

[U32] Py：代码格式化
来源：http://uz.asd995.cn

ruff format . && ruff check --fix .
来源：http://qw.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://wr.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://uc.521024.cn

[U34] Py：判断编码
来源：http://vl.szxytkj.cn

chardet.detect(raw)
来源：http://wp.panjiajie.cn

[U35] Py：发送邮件
来源：http://uj.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ag.newstarts.cn

[U36] Py：定时任务
来源：http://mp.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://eu.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://bi.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fo.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://vd.hahajie.cn

Path(__file__).resolve().parent
来源：http://sz.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://fu.hahajie.cn

sys.stdout.isatty()
来源：http://xc.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://dw.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://kk.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://ss.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wo.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://ep.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sx.huanxung.cn

[U43] PHP：声明命名空间
来源：http://qv.yuexingan06.cn

namespace App\Http;
来源：http://wg.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://vc.muxihuayi.cn

declare(strict_types=1);
来源：http://tp.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://tx.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gv.colortex.cn

[U46] PHP：可空类型
来源：http://vg.wgjwhj.cn

?string $name = null
来源：http://sr.newstarts.cn

[U47] PHP：联合类型
来源：http://uy.panjiajie.cn

int|string $id
来源：http://ob.lnxyls.cn

[U48] PHP：纯枚举
来源：http://si.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rs.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://cp.lnxyls.cn

public readonly string $name
来源：http://bv.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://iv.hahajie.cn

public function __construct(private int $id) {}
来源：http://fn.wgjwhj.cn

[U51] PHP：数组解构
来源：http://kr.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://ux.521024.cn

[U52] PHP：箭头函数
来源：http://he.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://bm.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://wc.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://pz.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://bb.wgjwhj.cn

$obj?->method()
来源：http://ty.szsharing.cn

[U55] PHP：match 表达式
来源：http://qa.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dl.hnjuh.cn

[U56] PHP：命名参数
来源：http://tp.9csxet.cn

f(a: 1, b: 2)
来源：http://kq.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://ww.9csxet.cn

"值: {$a}"
来源：http://ev.panjiajie.cn

[U58] PHP：数组三件套
来源：http://co.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gr.szxytkj.cn

[U59] PHP：自定义排序
来源：http://ku.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xf.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://tk.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bl.bookmarksfly.cn

[U61] PHP：正则
来源：http://je.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jt.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://cn.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iz.huixiangedu.cn

[U63] PHP：文件读写
来源：http://pm.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rd.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://it.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://bb.hahajie.cn

[U65] PHP：会话
来源：http://uf.yuexingan06.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nh.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://oe.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zt.nicolike.cn

[U67] PHP：处理文件上传
来源：http://wb.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tk.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://hr.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://en.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://lk.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cl.asd995.cn

[U70] PHP：PDO 事务
来源：http://at.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://az.nicolike.cn

[U71] PHP：抛出异常
来源：http://mb.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://br.hnjuh.cn

[U72] PHP：写错误日志
来源：http://mk.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://hh.szsharing.cn

[U73] PHP：读取 ini 配置
来源：http://zi.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://wv.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://ti.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://se.shtwfgs.cn


<!-- 参考信息 -->