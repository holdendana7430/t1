代发 wailian999

#ifndef X_H
来源：http://ls.szsharing.cn

#define X_H
来源：http://ow.yuexingan06.cn

#endif
来源：http://mm.shxzskj.cn

[S31] C++：Hello World
来源：http://hz.yuexingan06.cn

#include <iostream>
来源：http://wl.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://iv.chemitech.net.cn

[S32] C++：字符串
来源：http://ez.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://og.szxytkj.cn

[S33] C++：vector 增删
来源：http://um.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qx.szsharing.cn

[S34] C++：遍历 vector
来源：http://rj.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://oa.hahajie.cn

[S35] C++：map
来源：http://ic.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vn.newstarts.cn

[S36] C++：unordered_map
来源：http://jh.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dg.hnjuh.cn

[S37] C++：set
来源：http://is.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fr.muxihuayi.cn

[S38] C++：排序
来源：http://ka.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://ga.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://tf.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rr.huixiangedu.cn

[S40] C++：查找元素
来源：http://nb.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oq.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://yy.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ig.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://eb.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://ai.shxzukj.cn

[S43] C++：智能指针
来源：http://it.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://uk.szxytkj.cn

[S44] C++：引用传参
来源：http://bo.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://xr.colortex.cn

[S45] C++：lambda
来源：http://ii.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pq.muxihuayi.cn

[S46] C++：函数模板
来源：http://mx.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ve.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://fb.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bb.asd995.cn

[S48] C++：逐行读文件
来源：http://by.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nt.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://ye.yuntaijiaju.cn

[S49] C++：写文件
来源：http://hb.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ju.szsharing.cn

[S50] C++：格式化数字
来源：http://go.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sw.9csxet.cn

[S51] C++：显式类型转换
来源：http://wt.shtwfgs.cn

static_cast<double>(a) / b
来源：http://rc.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://xi.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://yp.szxytkj.cn

[S53] C++：移动语义
来源：http://xy.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://rg.szxytkj.cn

[S54] C++：异常处理
来源：http://zu.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rt.shxzukj.cn

[S55] C++：结构化绑定
来源：http://cg.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lf.szxytkj.cn

[S56] C++：optional
来源：http://xu.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cr.shxzskj.cn

[S57] C++：编译期常量
来源：http://mw.szsharing.cn

constexpr int N = 10;
来源：http://ge.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://oq.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://dg.lnxyls.cn

[S59] C++：静态断言
来源：http://tq.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gt.521024.cn

[S60] C++：遍历并删除元素
来源：http://ko.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ch.huixiangedu.cn

================================================================================
来源：http://lj.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hf.asd995.cn

================================================================================
来源：http://wi.colortex.cn

[T01] Kotlin：Hello World
来源：http://xv.szxytkj.cn

println("Hello")
来源：http://kc.bjjhwx.cn

[T02] Kotlin：变量
来源：http://ll.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oa.521024.cn

[T03] Kotlin：字符串模板
来源：http://tz.hahajie.cn

"值: $b"
来源：http://ht.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://pi.huanxung.cn

val n: String? = null;  n?.length
来源：http://ba.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://qc.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ra.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://ev.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sf.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://hy.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://je.hnjuh.cn

[T08] Kotlin：数据类
来源：http://ka.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://fw.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://ut.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://du.nicolike.cn

[T10] Kotlin：默认参数
来源：http://ue.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hj.shxzukj.cn

[T11] Kotlin：协程
来源：http://xb.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://el.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://lj.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://yu.asd995.cn

[T13] Kotlin：只读 Map
来源：http://rv.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://vi.colortex.cn

[T14] Kotlin：循环
来源：http://mi.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://iu.jctech888.com.cn

[T15] Kotlin：接口
来源：http://ws.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://wi.nszjky.cn

[T16] Swift：Hello World
来源：http://py.szxytkj.cn

print("Hello")
来源：http://vd.colortex.cn

[T17] Swift：变量与常量
来源：http://bs.shxzukj.cn

var a = 1;  let b = 2
来源：http://iv.hahajie.cn

[T18] Swift：字符串插值
来源：http://em.huixinmuqiang.cn

"值: \(b)"
来源：http://ii.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://sr.shtwfgs.cn

if let n = opt { print(n) }
来源：http://jz.bjjhwx.cn

[T20] Swift：数组操作
来源：http://ur.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hj.lnxyls.cn

[T21] Swift：遍历
来源：http://cb.muxihuayi.cn

for x in a { print(x) }
来源：http://to.9csxet.cn

[T22] Swift：字典
来源：http://vb.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dj.yuntaijiaju.cn

[T23] Swift：函数
来源：http://vt.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ch.colortex.cn

[T24] Swift：闭包
来源：http://gy.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://eq.hnjuh.cn

[T25] Swift：结构体
来源：http://kj.szsharing.cn

struct P { var x: Int }
来源：http://sb.521024.cn

[T26] Swift：类与重写
来源：http://yx.szxytkj.cn

class A: Base { override func f() {} }
来源：http://jo.asd995.cn

[T27] Swift：错误处理
来源：http://by.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://dk.jctech888.com.cn

[T28] Swift：枚举
来源：http://rw.bjjhwx.cn

enum Color { case red, green }
来源：http://ls.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://on.hnjuh.cn

guard let x = opt else { return }
来源：http://vg.muxihuayi.cn

[T30] Swift：协议
来源：http://og.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://dp.521024.cn

[T31] Lua：Hello World
来源：http://jn.bjjhwx.cn

print("Hello")
来源：http://lq.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://yu.huanxung.cn

local a = 1
来源：http://gn.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://fr.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mr.jctech888.com.cn

[T34] Lua：遍历表
来源：http://za.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://is.shxzskj.cn

[T35] Lua：字典表
来源：http://jh.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://eh.yuntaijiaju.cn

[T36] Lua：函数
来源：http://re.wgjwhj.cn

function add(a, b) return a + b end
来源：http://hy.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://mn.yuexingan06.cn

"a" .. "b"
来源：http://mt.hnjuh.cn

[T38] Lua：条件
来源：http://fv.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://za.panjiajie.cn

[T39] Lua：模式匹配
来源：http://jw.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://oq.wgjwhj.cn

[T40] Lua：元表
来源：http://gu.asd995.cn

setmetatable({}, { __index = base })
来源：http://ot.asd995.cn

[T41] Perl：Hello World
来源：http://as.shxzukj.cn

print "Hello\n";
来源：http://do.bjjhwx.cn

[T42] Perl：变量类型
来源：http://xo.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nr.szsharing.cn

[T43] Perl：字符串插值
来源：http://kt.shxzskj.cn

"值: $a"
来源：http://by.chemitech.net.cn

[T44] Perl：条件
来源：http://es.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://ke.huanxung.cn

[T45] Perl：数组遍历
来源：http://vm.jianghongdianzi.cn

for my $x (@arr) { print $x; }
来源：http://gv.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://gm.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bz.gzmigu.cn

[T47] Perl：正则捕获
来源：http://bw.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vq.shxzskj.cn

[T48] Perl：正则替换
来源：http://xp.szxytkj.cn

$s =~ s/old/new/g;
来源：http://ts.jctech888.com.cn

[T49] Perl：函数
来源：http://os.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ba.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://bq.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zy.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://vb.muxihuayi.cn

[T51] Scala：Hello World
来源：http://oa.asd995.cn

println("Hello")
来源：http://uv.shtwfgs.cn

[T52] Scala：变量
来源：http://cg.gzmigu.cn

val a = 1;  var b = 2
来源：http://if.shxzskj.cn

[T53] Scala：字符串插值
来源：http://aa.jianghongdianzi.cn

s"值: $b"
来源：http://zz.huanxung.cn

[T54] Scala：集合映射
来源：http://kq.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://tz.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://nl.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bw.yuexingan06.cn

[T56] Scala：样例类
来源：http://wf.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://ok.nszjky.cn

[T57] Scala：模式匹配
来源：http://rx.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fs.panjiajie.cn

[T58] Scala：函数定义
来源：http://wc.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sa.yuexingan06.cn

[T59] Scala：循环
来源：http://mb.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://gz.jctech888.com.cn

[T60] Scala：折叠
来源：http://hr.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ud.chemitech.net.cn

================================================================================
来源：http://um.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ot.huixiangedu.cn

================================================================================
来源：http://jw.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://nm.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zh.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://bo.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cn.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://zb.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qz.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://sf.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ip.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://dw.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://oj.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://pk.lnxyls.cn

{**a, **b}
来源：http://xo.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://rs.szsharing.cn

{v: k for k, v in d.items()}
来源：http://yq.nszjky.cn

[U08] Py：展平二维列表
来源：http://oj.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://jk.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://cv.haigaiapp.cn

max(d, key=d.get)
来源：http://ax.szsharing.cn

[U10] Py：按值排序字典
来源：http://ji.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gz.newstarts.cn

[U11] Py：生成器表达式
来源：http://cp.wgjwhj.cn

(x * 2 for x in arr)
来源：http://nn.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cb.hahajie.cn

Counter(arr).most_common(3)
来源：http://aq.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://rt.bookmarksfly.cn

deque(maxlen=10)
来源：http://zu.newstarts.cn

[U14] Py：分组收集到列表
来源：http://hc.bjjhwx.cn

defaultdict(list)
来源：http://wa.wgjwhj.cn

[U15] Py：高精度计时
来源：http://au.gzmigu.cn

t = time.perf_counter()
来源：http://ra.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://ej.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gf.wgjwhj.cn

[U17] Py：初始化日志
来源：http://xd.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://ka.gzmigu.cn

[U18] Py：预编译正则
来源：http://mm.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://cp.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://fs.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://po.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://ma.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://gg.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://ji.bookmarksfly.cn

@contextlib.contextmanager
来源：http://ll.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://ac.9csxet.cn

list(zip(*m))
来源：http://iy.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://ad.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cb.shxzukj.cn

[U24] Py：路径操作
来源：http://rt.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yu.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://aq.jctech888.com.cn

csv.DictReader(f)
来源：http://rg.bookmarksfly.cn

[U26] Py：并发下载
来源：http://fh.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cx.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://de.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://pb.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://rk.nicolike.cn

UserId = int
来源：http://qb.gzmigu.cn

[U29] Py：属性校验
来源：http://of.521024.cn

@property 与 @x.setter 配合
来源：http://qw.lnxyls.cn

[U30] Py：数据类
来源：http://xk.shxzukj.cn

@dataclass(slots=True)
来源：http://sq.yuexingan06.cn

[U31] Py：单测
来源：http://ve.nicolike.cn

python -m pytest -q
来源：http://pq.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://mq.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://jz.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://mr.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://jt.asd995.cn

[U34] Py：判断编码
来源：http://xw.bjjhwx.cn

chardet.detect(raw)
来源：http://nr.9csxet.cn

[U35] Py：发送邮件
来源：http://jj.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wq.panjiajie.cn

[U36] Py：定时任务
来源：http://xo.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://xy.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://dp.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jl.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://na.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://wj.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://pv.szxytkj.cn

sys.stdout.isatty()
来源：http://kq.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://jg.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://em.bjjhwx.cn

[U41] PHP：初始化 Composer 项目
来源：http://pe.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uz.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://lf.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ow.newstarts.cn

[U43] PHP：声明命名空间
来源：http://gg.chemitech.net.cn

namespace App\Http;
来源：http://zd.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://fs.huanxung.cn

declare(strict_types=1);
来源：http://ry.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://nf.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xz.lnxyls.cn

[U46] PHP：可空类型
来源：http://hr.jctech888.com.cn

?string $name = null
来源：http://rg.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://mw.nicolike.cn

int|string $id
来源：http://hk.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://wm.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hy.lnxyls.cn

[U49] PHP：只读属性
来源：http://fs.shxzukj.cn

public readonly string $name
来源：http://pg.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://pr.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://jv.colortex.cn

[U51] PHP：数组解构
来源：http://hq.panjiajie.cn

[$a, $b] = $arr;
来源：http://hr.nicolike.cn

[U52] PHP：箭头函数
来源：http://ul.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://dp.521024.cn

[U53] PHP：空合并运算符
来源：http://fr.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://ie.huanxung.cn

[U54] PHP：空安全调用
来源：http://rd.huanxung.cn

$obj?->method()
来源：http://vt.lnxyls.cn


<!-- 参考信息 -->