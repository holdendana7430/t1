代发 wailian999

#include <iostream>
来源：http://zv.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://ke.jctech888.com.cn

[S32] C++：字符串
来源：http://ie.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://xa.lnxyls.cn

[S33] C++：vector 增删
来源：http://tr.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ie.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://qu.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://wz.521024.cn

[S35] C++：map
来源：http://kq.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iv.huixiangedu.cn

[S36] C++：unordered_map
来源：http://xn.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wy.shxzukj.cn

[S37] C++：set
来源：http://do.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kx.jianghongdianzi.cn

[S38] C++：排序
来源：http://yp.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://mg.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://gf.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gi.haigaiapp.cn

[S40] C++：查找元素
来源：http://ht.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://is.nszjky.cn

[S41] C++：类与构造函数
来源：http://jn.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qt.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://iy.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://ab.haigaiapp.cn

[S43] C++：智能指针
来源：http://gt.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://oc.nszjky.cn

[S44] C++：引用传参
来源：http://cc.hahajie.cn

void inc(int &x) { ++x; }
来源：http://kc.muxihuayi.cn

[S45] C++：lambda
来源：http://jn.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rz.521024.cn

[S46] C++：函数模板
来源：http://kd.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oy.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://sh.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fr.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://lz.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ew.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://ba.huixinmuqiang.cn

[S49] C++：写文件
来源：http://be.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ir.huixiangedu.cn

[S50] C++：格式化数字
来源：http://zo.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gq.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://wi.521024.cn

static_cast<double>(a) / b
来源：http://wm.asd995.cn

[S52] C++：const 与 noexcept
来源：http://fp.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://rw.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://rp.colortex.cn

std::vector<int> w = std::move(v);
来源：http://au.colortex.cn

[S54] C++：异常处理
来源：http://ot.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aw.521024.cn

[S55] C++：结构化绑定
来源：http://fl.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rw.gzmigu.cn

[S56] C++：optional
来源：http://pz.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ba.shxzukj.cn

[S57] C++：编译期常量
来源：http://nh.szxytkj.cn

constexpr int N = 10;
来源：http://fg.521024.cn

[S58] C++：命名空间
来源：http://gd.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://ns.gzmigu.cn

[S59] C++：静态断言
来源：http://hc.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ly.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://lc.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zz.huixiangedu.cn

================================================================================
来源：http://qd.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dc.hnjuh.cn

================================================================================
来源：http://ob.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://gd.wgjwhj.cn

println("Hello")
来源：http://vq.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://sw.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bd.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://oy.bjjhwx.cn

"值: $b"
来源：http://qp.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://il.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://fv.asd995.cn

[T05] Kotlin：when 表达式
来源：http://qa.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hl.nicolike.cn

[T06] Kotlin：集合映射
来源：http://as.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ok.521024.cn

[T07] Kotlin：集合过滤
来源：http://kj.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ne.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://ca.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://tk.521024.cn

[T09] Kotlin：扩展函数
来源：http://in.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://zw.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://zi.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ti.shxzukj.cn

[T11] Kotlin：协程
来源：http://gk.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fm.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://gu.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://sx.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://qc.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://ms.wgjwhj.cn

[T14] Kotlin：循环
来源：http://ls.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://tz.shtwfgs.cn

[T15] Kotlin：接口
来源：http://da.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://bu.lnxyls.cn

[T16] Swift：Hello World
来源：http://zw.gzmigu.cn

print("Hello")
来源：http://op.asd995.cn

[T17] Swift：变量与常量
来源：http://ad.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://cc.hahajie.cn

[T18] Swift：字符串插值
来源：http://qp.wgjwhj.cn

"值: \(b)"
来源：http://jp.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://hi.gzmigu.cn

if let n = opt { print(n) }
来源：http://ed.shxzskj.cn

[T20] Swift：数组操作
来源：http://pi.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bf.shxzukj.cn

[T21] Swift：遍历
来源：http://hn.newstarts.cn

for x in a { print(x) }
来源：http://nv.shtwfgs.cn

[T22] Swift：字典
来源：http://ze.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yp.gzmigu.cn

[T23] Swift：函数
来源：http://fr.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pg.huanxung.cn

[T24] Swift：闭包
来源：http://mp.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hh.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://oq.wgjwhj.cn

struct P { var x: Int }
来源：http://kh.9csxet.cn

[T26] Swift：类与重写
来源：http://md.nicolike.cn

class A: Base { override func f() {} }
来源：http://th.gzmigu.cn

[T27] Swift：错误处理
来源：http://dj.asd995.cn

do { try f() } catch { print(error) }
来源：http://wr.nszjky.cn

[T28] Swift：枚举
来源：http://up.lnxyls.cn

enum Color { case red, green }
来源：http://ic.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://qk.asd995.cn

guard let x = opt else { return }
来源：http://vg.newstarts.cn

[T30] Swift：协议
来源：http://tq.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://ct.shxzukj.cn

[T31] Lua：Hello World
来源：http://wr.jctech888.com.cn

print("Hello")
来源：http://fd.shxzskj.cn

[T32] Lua：局部变量
来源：http://ok.jctech888.com.cn

local a = 1
来源：http://ed.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://zh.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kv.newstarts.cn

[T34] Lua：遍历表
来源：http://zx.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zu.gzmigu.cn

[T35] Lua：字典表
来源：http://in.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://zj.panjiajie.cn

[T36] Lua：函数
来源：http://fa.521024.cn

function add(a, b) return a + b end
来源：http://dz.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://wd.muxihuayi.cn

"a" .. "b"
来源：http://sa.haigaiapp.cn

[T38] Lua：条件
来源：http://cf.szxytkj.cn

if x > 0 then print("正") end
来源：http://cl.newstarts.cn

[T39] Lua：模式匹配
来源：http://iu.newstarts.cn

string.find(s, "%d+")
来源：http://cz.chemitech.net.cn

[T40] Lua：元表
来源：http://bi.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://vk.szxytkj.cn

[T41] Perl：Hello World
来源：http://yz.bookmarksfly.cn

print "Hello\n";
来源：http://wb.hnjuh.cn

[T42] Perl：变量类型
来源：http://yn.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sd.lnxyls.cn

[T43] Perl：字符串插值
来源：http://qv.jctech888.com.cn

"值: $a"
来源：http://mx.bookmarksfly.cn

[T44] Perl：条件
来源：http://hl.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://xh.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://ez.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://oq.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://qy.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hn.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://ew.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://of.haigaiapp.cn

[T48] Perl：正则替换
来源：http://bg.panjiajie.cn

$s =~ s/old/new/g;
来源：http://xm.yuexingan06.cn

[T49] Perl：函数
来源：http://mg.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xc.9csxet.cn

[T50] Perl：逐行读文件
来源：http://yw.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lh.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://jp.jctech888.com.cn

[T51] Scala：Hello World
来源：http://jo.huixinmuqiang.cn

println("Hello")
来源：http://rz.colortex.cn

[T52] Scala：变量
来源：http://lr.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://so.hahajie.cn

[T53] Scala：字符串插值
来源：http://fg.bookmarksfly.cn

s"值: $b"
来源：http://fq.gzmigu.cn

[T54] Scala：集合映射
来源：http://cj.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://wb.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://ag.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wt.jctech888.com.cn

[T56] Scala：样例类
来源：http://sw.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://ka.colortex.cn

[T57] Scala：模式匹配
来源：http://cv.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fs.newstarts.cn

[T58] Scala：函数定义
来源：http://xj.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://km.muxihuayi.cn

[T59] Scala：循环
来源：http://ac.521024.cn

for (i <- 1 to 10) println(i)
来源：http://lh.muxihuayi.cn

[T60] Scala：折叠
来源：http://kk.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yc.huixiangedu.cn

================================================================================
来源：http://sn.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bg.chemitech.net.cn

================================================================================
来源：http://ht.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://qm.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lg.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://rg.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oq.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://af.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vn.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://gl.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kq.hahajie.cn

[U05] Py：列表去重且保序
来源：http://jw.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://fy.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://ki.9csxet.cn

{**a, **b}
来源：http://eo.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://vq.colortex.cn

{v: k for k, v in d.items()}
来源：http://wv.colortex.cn

[U08] Py：展平二维列表
来源：http://up.muxihuayi.cn

[y for x in nested for y in x]
来源：http://nc.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://tu.yuexingan06.cn

max(d, key=d.get)
来源：http://pr.nicolike.cn

[U10] Py：按值排序字典
来源：http://nf.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tw.nicolike.cn

[U11] Py：生成器表达式
来源：http://mw.9csxet.cn

(x * 2 for x in arr)
来源：http://ol.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ve.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://hi.gzmigu.cn

[U13] Py：固定长度队列
来源：http://ws.9csxet.cn

deque(maxlen=10)
来源：http://ab.nicolike.cn

[U14] Py：分组收集到列表
来源：http://tz.huixiangedu.cn

defaultdict(list)
来源：http://yx.asd995.cn

[U15] Py：高精度计时
来源：http://ko.521024.cn

t = time.perf_counter()
来源：http://ui.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://kl.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ju.shxzukj.cn

[U17] Py：初始化日志
来源：http://rk.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://bt.huixiangedu.cn

[U18] Py：预编译正则
来源：http://db.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://cm.hahajie.cn

[U19] Py：正则替换带回调
来源：http://nn.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ak.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://zw.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://qg.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://cq.shxzukj.cn

@contextlib.contextmanager
来源：http://fm.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://hu.521024.cn

list(zip(*m))
来源：http://br.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://hm.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ha.521024.cn

[U24] Py：路径操作
来源：http://zr.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wj.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://zk.newstarts.cn

csv.DictReader(f)
来源：http://mn.colortex.cn

[U26] Py：并发下载
来源：http://tg.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ha.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://zo.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://jh.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://tw.521024.cn

UserId = int
来源：http://vj.jctech888.com.cn

[U29] Py：属性校验
来源：http://ng.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://du.shxzukj.cn

[U30] Py：数据类
来源：http://ve.jctech888.com.cn

@dataclass(slots=True)
来源：http://eg.huixinmuqiang.cn

[U31] Py：单测
来源：http://ve.hnjuh.cn

python -m pytest -q
来源：http://zx.hnjuh.cn

[U32] Py：代码格式化
来源：http://hd.asd995.cn

ruff format . && ruff check --fix .
来源：http://jc.newstarts.cn

[U33] Py：打包发布
来源：http://lj.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://bd.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://du.colortex.cn

chardet.detect(raw)
来源：http://zm.szsharing.cn

[U35] Py：发送邮件
来源：http://wi.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://au.szsharing.cn

[U36] Py：定时任务
来源：http://bs.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://iz.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://de.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qn.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://cc.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://cb.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://mq.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://vo.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://xe.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://bc.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://pe.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ch.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://dj.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://va.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://oo.wgjwhj.cn

namespace App\Http;
来源：http://ym.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://os.nszjky.cn

declare(strict_types=1);
来源：http://fy.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://wa.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lj.hahajie.cn

[U46] PHP：可空类型
来源：http://st.hahajie.cn

?string $name = null
来源：http://dn.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://ib.lnxyls.cn

int|string $id
来源：http://qx.hahajie.cn

[U48] PHP：纯枚举
来源：http://dg.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eg.huanxung.cn

[U49] PHP：只读属性
来源：http://ee.yuexingan06.cn

public readonly string $name
来源：http://ji.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://vh.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://ow.9csxet.cn

[U51] PHP：数组解构
来源：http://ui.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://uc.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://ix.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://ex.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://vx.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://io.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://kg.nszjky.cn

$obj?->method()
来源：http://ca.shxzskj.cn

[U55] PHP：match 表达式
来源：http://jv.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fw.szxytkj.cn

[U56] PHP：命名参数
来源：http://lz.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://iq.shtwfgs.cn


<!-- 参考信息 -->