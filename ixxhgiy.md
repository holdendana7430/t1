代发 wailian999

#include <iostream>
来源：http://ub.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://rl.shtwfgs.cn

[S32] C++：字符串
来源：http://tk.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://uv.nszjky.cn

[S33] C++：vector 增删
来源：http://fc.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://my.hahajie.cn

[S34] C++：遍历 vector
来源：http://cu.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://qz.9csxet.cn

[S35] C++：map
来源：http://xq.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cs.szxytkj.cn

[S36] C++：unordered_map
来源：http://dq.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://si.szsharing.cn

[S37] C++：set
来源：http://im.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jn.wgjwhj.cn

[S38] C++：排序
来源：http://jh.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://xs.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://rc.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://no.hahajie.cn

[S40] C++：查找元素
来源：http://tm.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vc.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://si.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://za.nicolike.cn

[S42] C++：继承与虚函数
来源：http://nl.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://uy.shxzskj.cn

[S43] C++：智能指针
来源：http://cj.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://hd.wgjwhj.cn

[S44] C++：引用传参
来源：http://mb.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://pa.hahajie.cn

[S45] C++：lambda
来源：http://an.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uw.colortex.cn

[S46] C++：函数模板
来源：http://yg.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zm.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://ly.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ha.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://dm.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kp.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://as.lnxyls.cn

[S49] C++：写文件
来源：http://wu.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://co.chemitech.net.cn

[S50] C++：格式化数字
来源：http://cf.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gi.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://cq.colortex.cn

static_cast<double>(a) / b
来源：http://no.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://cv.asd995.cn

int size() const noexcept { return n_; }
来源：http://yr.shxzukj.cn

[S53] C++：移动语义
来源：http://xg.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://eg.haigaiapp.cn

[S54] C++：异常处理
来源：http://up.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gs.gzmigu.cn

[S55] C++：结构化绑定
来源：http://wp.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xd.huixiangedu.cn

[S56] C++：optional
来源：http://za.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rm.lnxyls.cn

[S57] C++：编译期常量
来源：http://cc.newstarts.cn

constexpr int N = 10;
来源：http://sm.szsharing.cn

[S58] C++：命名空间
来源：http://qe.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://cy.panjiajie.cn

[S59] C++：静态断言
来源：http://wd.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eo.521024.cn

[S60] C++：遍历并删除元素
来源：http://bv.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qh.yuntaijiaju.cn

================================================================================
来源：http://ek.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vd.jctech888.com.cn

================================================================================
来源：http://vt.9csxet.cn

[T01] Kotlin：Hello World
来源：http://tx.shtwfgs.cn

println("Hello")
来源：http://vu.shtwfgs.cn

[T02] Kotlin：变量
来源：http://ml.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nm.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://wy.panjiajie.cn

"值: $b"
来源：http://yr.nszjky.cn

[T04] Kotlin：空安全
来源：http://rl.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://ij.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://nd.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bx.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://fy.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mu.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://qi.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lw.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://nj.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://is.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://iu.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://sk.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://at.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rq.gzmigu.cn

[T11] Kotlin：协程
来源：http://pn.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dg.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://pb.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://sr.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://up.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://gm.asd995.cn

[T14] Kotlin：循环
来源：http://kp.hahajie.cn

for (i in 1..10) println(i)
来源：http://jc.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://tn.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://zm.yuexingan06.cn

[T16] Swift：Hello World
来源：http://og.shxzukj.cn

print("Hello")
来源：http://yq.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://nr.gzmigu.cn

var a = 1;  let b = 2
来源：http://qe.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://hh.gzmigu.cn

"值: \(b)"
来源：http://cx.panjiajie.cn

[T19] Swift：可选绑定
来源：http://pz.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://bd.haigaiapp.cn

[T20] Swift：数组操作
来源：http://gg.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jy.521024.cn

[T21] Swift：遍历
来源：http://wy.panjiajie.cn

for x in a { print(x) }
来源：http://oy.bjjhwx.cn

[T22] Swift：字典
来源：http://au.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xd.nicolike.cn

[T23] Swift：函数
来源：http://ac.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ns.yuexingan06.cn

[T24] Swift：闭包
来源：http://ga.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ba.shxzukj.cn

[T25] Swift：结构体
来源：http://ny.jctech888.com.cn

struct P { var x: Int }
来源：http://xx.huixiangedu.cn

[T26] Swift：类与重写
来源：http://kw.asd995.cn

class A: Base { override func f() {} }
来源：http://qk.haigaiapp.cn

[T27] Swift：错误处理
来源：http://jg.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://sf.chemitech.net.cn

[T28] Swift：枚举
来源：http://bs.huixiangedu.cn

enum Color { case red, green }
来源：http://pn.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://bj.bookmarksfly.cn

guard let x = opt else { return }
来源：http://nz.wgjwhj.cn

[T30] Swift：协议
来源：http://hb.colortex.cn

protocol Shape { func area() -> Double }
来源：http://yt.szxytkj.cn

[T31] Lua：Hello World
来源：http://ll.muxihuayi.cn

print("Hello")
来源：http://dj.hahajie.cn

[T32] Lua：局部变量
来源：http://hy.huixiangedu.cn

local a = 1
来源：http://ar.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://qi.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jc.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://ry.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lu.chemitech.net.cn

[T35] Lua：字典表
来源：http://ej.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://jb.szsharing.cn

[T36] Lua：函数
来源：http://uk.shxzukj.cn

function add(a, b) return a + b end
来源：http://qb.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://hb.colortex.cn

"a" .. "b"
来源：http://ps.colortex.cn

[T38] Lua：条件
来源：http://rk.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://ke.lnxyls.cn

[T39] Lua：模式匹配
来源：http://bc.colortex.cn

string.find(s, "%d+")
来源：http://dt.gzmigu.cn

[T40] Lua：元表
来源：http://gg.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://nx.haigaiapp.cn

[T41] Perl：Hello World
来源：http://tj.nicolike.cn

print "Hello\n";
来源：http://xi.hahajie.cn

[T42] Perl：变量类型
来源：http://qh.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://by.szsharing.cn

[T43] Perl：字符串插值
来源：http://cz.shxzukj.cn

"值: $a"
来源：http://rg.yuntaijiaju.cn

[T44] Perl：条件
来源：http://cz.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://yq.hnjuh.cn

[T45] Perl：数组遍历
来源：http://jg.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://ba.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://cm.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pr.asd995.cn

[T47] Perl：正则捕获
来源：http://ia.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wg.chemitech.net.cn

[T48] Perl：正则替换
来源：http://hk.newstarts.cn

$s =~ s/old/new/g;
来源：http://yj.szsharing.cn

[T49] Perl：函数
来源：http://fc.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hg.colortex.cn

[T50] Perl：逐行读文件
来源：http://ah.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rm.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://rn.gzmigu.cn

[T51] Scala：Hello World
来源：http://ho.hahajie.cn

println("Hello")
来源：http://fu.bjjhwx.cn

[T52] Scala：变量
来源：http://vh.9csxet.cn

val a = 1;  var b = 2
来源：http://qq.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://zb.shxzskj.cn

s"值: $b"
来源：http://ce.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://cm.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://sp.colortex.cn

[T55] Scala：集合过滤
来源：http://ul.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oa.bjjhwx.cn

[T56] Scala：样例类
来源：http://dp.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://yg.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://nv.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qo.panjiajie.cn

[T58] Scala：函数定义
来源：http://qi.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sz.hahajie.cn

[T59] Scala：循环
来源：http://lu.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://wq.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://hx.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://le.nicolike.cn

================================================================================
来源：http://jq.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ek.nszjky.cn

================================================================================
来源：http://gy.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://pv.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bz.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://kc.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ls.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://wz.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ox.panjiajie.cn

[U04] Py：变量调试打印
来源：http://cf.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gx.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://rp.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://nw.shxzukj.cn

[U06] Py：合并两个字典
来源：http://vq.newstarts.cn

{**a, **b}
来源：http://yc.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://ov.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://po.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://gz.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://na.asd995.cn

[U09] Py：字典取最大值的键
来源：http://zv.panjiajie.cn

max(d, key=d.get)
来源：http://nq.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://pp.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vz.shxzukj.cn

[U11] Py：生成器表达式
来源：http://ut.nicolike.cn

(x * 2 for x in arr)
来源：http://ja.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yo.gzmigu.cn

Counter(arr).most_common(3)
来源：http://kc.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://ig.yuexingan06.cn

deque(maxlen=10)
来源：http://rl.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://qw.gzmigu.cn

defaultdict(list)
来源：http://uw.chemitech.net.cn

[U15] Py：高精度计时
来源：http://fi.hahajie.cn

t = time.perf_counter()
来源：http://ju.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://ma.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oe.shxzskj.cn

[U17] Py：初始化日志
来源：http://ml.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://vf.szxytkj.cn

[U18] Py：预编译正则
来源：http://nd.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://bu.asd995.cn

[U19] Py：正则替换带回调
来源：http://sg.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ko.colortex.cn

[U20] Py：缓存函数结果
来源：http://ft.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://xd.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://pr.521024.cn

@contextlib.contextmanager
来源：http://qc.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://wn.bjjhwx.cn

list(zip(*m))
来源：http://rb.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://lu.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lr.muxihuayi.cn

[U24] Py：路径操作
来源：http://gd.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nf.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://pu.wgjwhj.cn

csv.DictReader(f)
来源：http://sn.huanxung.cn

[U26] Py：并发下载
来源：http://al.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://de.hahajie.cn

[U27] Py：异步 HTTP
来源：http://dt.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://wq.chemitech.net.cn

[U28] Py：类型别名
来源：http://ou.chemitech.net.cn

UserId = int
来源：http://bt.szsharing.cn

[U29] Py：属性校验
来源：http://ae.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://vp.haigaiapp.cn

[U30] Py：数据类
来源：http://gd.shxzukj.cn

@dataclass(slots=True)
来源：http://ok.jianghongdianzi.cn

[U31] Py：单测
来源：http://hm.bookmarksfly.cn

python -m pytest -q
来源：http://ya.wgjwhj.cn

[U32] Py：代码格式化
来源：http://kj.nicolike.cn

ruff format . && ruff check --fix .
来源：http://vl.521024.cn

[U33] Py：打包发布
来源：http://eb.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://dl.colortex.cn

[U34] Py：判断编码
来源：http://xy.lnxyls.cn

chardet.detect(raw)
来源：http://dh.jctech888.com.cn

[U35] Py：发送邮件
来源：http://dj.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://am.jctech888.com.cn

[U36] Py：定时任务
来源：http://ue.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://hl.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://fl.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yy.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://pi.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://ct.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://rx.chemitech.net.cn

sys.stdout.isatty()
来源：http://in.521024.cn

[U40] Py：打印到标准错误
来源：http://dk.huanxung.cn

print("err", file=sys.stderr)
来源：http://wf.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://wh.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bf.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://xo.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vn.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://ui.huixiangedu.cn

namespace App\Http;
来源：http://mk.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://pu.bookmarksfly.cn

declare(strict_types=1);
来源：http://zr.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://za.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ap.shxzukj.cn

[U46] PHP：可空类型
来源：http://gr.panjiajie.cn

?string $name = null
来源：http://iq.hahajie.cn

[U47] PHP：联合类型
来源：http://yd.gzmigu.cn

int|string $id
来源：http://vp.hahajie.cn

[U48] PHP：纯枚举
来源：http://zq.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hc.panjiajie.cn

[U49] PHP：只读属性
来源：http://cf.bookmarksfly.cn

public readonly string $name
来源：http://ry.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://yh.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://uj.huanxung.cn

[U51] PHP：数组解构
来源：http://fa.haigaiapp.cn

[$a, $b] = $arr;
来源：http://cu.colortex.cn

[U52] PHP：箭头函数
来源：http://ms.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://zg.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://kd.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://ox.lnxyls.cn

[U54] PHP：空安全调用
来源：http://uc.bookmarksfly.cn

$obj?->method()
来源：http://du.hahajie.cn

[U55] PHP：match 表达式
来源：http://al.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mo.newstarts.cn

[U56] PHP：命名参数
来源：http://bz.gzmigu.cn

f(a: 1, b: 2)
来源：http://eg.hnjuh.cn


<!-- 参考信息 -->